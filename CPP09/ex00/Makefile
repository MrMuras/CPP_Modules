CXX = g++
CXXFLAGS = -Wall -Wextra -Werror -std=c++98
NAME = btc
SOURCES = main.cpp BitcoinExchange.cpp
HDRS = BitcoinExchange.hpp
OBJECTS = $(SOURCES:.cpp=.o)

all: $(NAME)

$(NAME): $(OBJECTS)
	$(CXX) $(CXXFLAGS) -o $(NAME) $(OBJECTS)

%.o: %.cpp $(HDRS)
	$(CXX) $(CXXFLAGS) -c $< -o $@

clean:
	rm -f $(OBJECTS)

fclean:
	rm -f $(NAME) $(OBJECTS)

re: fclean all

.PHONY: all clean fclean re