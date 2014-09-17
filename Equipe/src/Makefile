CXX = g++
CXXFLAGS = -g -Wall
LDFLAGS =
EXECUTABLE = test
SOURCES = BS.cxx MonteCarlo.cxx Option.cxx test.cxx
OBJETS = $(SOURCES:.cxx=.o)
$(EXECUTABLE) : $(OBJETS)
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LDFLAGS)
.cxx.o:
	$(CXX) $(CXXFLAGS) $< -o $@
clean:
	rm -f $(EXECUTABLE) $(OBJETS)
