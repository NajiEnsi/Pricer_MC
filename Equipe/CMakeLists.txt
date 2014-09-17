CXX = g++
CXXFLAGS = -g -Wall
LDFLAGS =
EXECUTABLE = test
SOURCES = test.cxx
OBJETS = $(SOURCES:.cxx=.o)
$(EXECUTABLE) : $(OBJETS)
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LDFLAGS)
.cxx.o:
	$(CXX) $(CXXFLAGS) $< -o $@
clean:
	rm -f $(EXECUTABLE) $(OBJETS)
