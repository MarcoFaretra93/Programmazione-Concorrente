all: prog testprog 

prog: buffer.o msg.o list.o poison_pill.o provider_buffer.o provider.o reader_buffer.o reader.o reader_list.o accepter_buffer.o accepter.o dispatcher.o main.o  
	gcc -o prog -g buffer.o msg.o list.o poison_pill.o provider_buffer.o provider.o reader_buffer.o reader.o reader_list.o accepter_buffer.o accepter.o dispatcher.o main.o -lpthread
testprog: buffer.o msg.o list.o poison_pill.o provider_buffer.o provider.o reader_buffer.o reader.o reader_list.o accepter_buffer.o accepter.o dispatcher.o mainTest.o
	gcc -o testprog -g buffer.o msg.o list.o poison_pill.o provider_buffer.o provider.o reader_buffer.o reader.o reader_list.o accepter_buffer.o accepter.o dispatcher.o mainTest.o -lpthread -lcunit
clean:
	rm *.o
	rm testprog
	rm prog