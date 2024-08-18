CPPFLAGS=-Wall -pthread -ggdb3 -Wall -Werror -pedantic -std=gnu++11

proxy: proxy.o
	g++ -o proxy $(CPPFLAGS) $<

%.o: %.cpp
	g++ $(CPPFLAGS) -c $<

.PHONY: clean
clean:
	rm -f *~ proxy *.o *.dSYM

# DO NOT DELETE
proxy.o: Cache.hpp Request.hpp Response.hpp Log.hpp Parser.hpp Socket.hpp
