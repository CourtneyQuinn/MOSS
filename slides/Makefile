COMMENT=${warning MAKING $@ out of $+ because of $?}
###################

%.pdf: %.eps
	epstopdf --autorotate=All $<
# %.dvi: %.tex nots_TS.tex macros_TS.tex
# 	${COMMENT}
# 	latex $<
%.raweps: %.dvi
	${COMMENT}
	dvips -E -i -p 1 -o $* $<
#       $(DVIPS) -E -i -K -p 1 -o $* $< # -K options seems to make %.raweps +non-readable
	mv $*001 $@
%.eps: %.raweps
	${COMMENT}
	epstool --copy --bbox $< $@
###################

figures: ryr-inst.pdf ryr-tr.pdf


ryr-inst.dvi: ryr-inst.tex nots_TS.tex macros_TS.tex auxInstIn-ryrOone_x_off_4.8_5.8_0.4_0.8.eps auxTRRyR-AP.eps
	${COMMENT}
	latex $<

ryr-tr.dvi: ryr-tr.tex nots_TS.tex macros_TS.tex auxTRRyR-AP.eps
	${COMMENT}
	latex $<

# mc.dvi: mc.tex nots_TS.tex macros_TS.tex ryrmc.tex icalmc.tex
# 	${COMMENT}
# 	latex $<

