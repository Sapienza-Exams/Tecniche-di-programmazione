FILE_NAME_TEST=e7_test
FILE_NAME_ESERCIZIO=functions
FILE_NAME_CORRETTORE=e7_correttore

all: $(FILE_NAME_TEST)

$(FILE_NAME_TEST): $(FILE_NAME_TEST).o $(FILE_NAME_ESERCIZIO).o $(FILE_NAME_CORRETTORE).o
	g++ -o $(FILE_NAME_TEST) $(FILE_NAME_TEST).o $(FILE_NAME_ESERCIZIO).o $(FILE_NAME_CORRETTORE).o

$(FILE_NAME_TEST).o: $(FILE_NAME_TEST).c $(FILE_NAME_ESERCIZIO).h 
	g++ -c $(FILE_NAME_TEST).c

$(FILE_NAME_ESERCIZIO).o: $(FILE_NAME_ESERCIZIO).c $(FILE_NAME_ESERCIZIO).h 
	g++ -c $(FILE_NAME_ESERCIZIO).c -lm

#ds TODO remove this line for the exam code
#$(FILE_NAME_CORRETTORE).o: $(FILE_NAME_CORRETTORE).c $(FILE_NAME_CORRETTORE).h
#	g++ -c $(FILE_NAME_CORRETTORE).c

clean:
	rm -rf $(FILE_NAME_TEST).o $(FILE_NAME_TEST) $(FILE_NAME_ESERCIZIO).o *~
