CC:=g++
FLAGS:=-g
game: logic minimax
	$(CC) $(FLAGS) logic.cc minimax.cc game.cc -o $@
minimax: logic
	$(CC) $(FLAGS) -c logic.cc minimax.cc
test: logic minimax
	$(CC) $(FLAGS) logic.cc minimax.cc test.cc -o $@
logic:
	$(CC) $(FLAGS) -c logic.cc
clean: logic minimax test
	rm test game *.o

