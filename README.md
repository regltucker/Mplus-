# Mplus-
TITLE:	CFA for Entrepreneurial Possible-Self
!3 factor model

DATA:	file = epscfa.txt;
	listwise = on;

VARIABLE:	NAMES ARE eps1-eps9;
	missing are .;

ANALYSIS: type = general;

MODEL:	f1 BY eps1-eps3;
	f2 BY eps4-eps6;
	f3 BY eps7-eps9;
	
OUTPUT:	sampstat stdyx;


