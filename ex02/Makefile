# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jinoh <jinoh@student.42seoul.kr>           +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/09/15 14:44:52 by jinoh             #+#    #+#              #
#    Updated: 2022/09/15 14:44:59 by jinoh            ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = tests
CC = c++
CFLAGS = -Wall -Wextra -Werror -std=c++98

SRCS =	tests.cpp \
		Account.cpp

OBJS = $(SRCS:%.cpp=%.o)

%.o: %.c
		$(CC) $(CFLAGS) -c $< -o $(<:.c=.o)

$(NAME): $(OBJS)
	$(CC) $(CFLAGS) $(OBJS) -o $(NAME)

all : $(NAME)

clean:
		@rm -rf $(OBJS)

fclean: clean
		@rm -rf $(NAME)

re:	fclean all

.PHONY: all clean fclean re
