# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: bdebbie <marvin@42.fr>                     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/01/12 03:20:54 by bdebbie           #+#    #+#              #
#    Updated: 2020/01/13 07:15:53 by bdebbie          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRC = actions.c \
	  print.c \
	  ft_itoa.c \
	  checker.c \
	  ft_atoi.c \
	  ft_strcmp.c \
	  parse.c
OBJ = $(patsubst %.c,%.o, $(SRC))
NAME = checker
INC = checker.h

all: $(NAME)

$(NAME): $(OBJ)
	@gcc -Wall -Wextra -Werror -o $(NAME) $(OBJ) -I $(INC)
	@echo "\033[92m***CHECKER SUCCESSFULLY COMPILED***\033[39m"

$(OBJ): %.o:%.c
	@gcc -Wall -Wextra -Werror -c $< -I $(INC)

clean:
	@rm -rf $(OBJ)

fclean: clean
	@rm -rf $(NAME)

re: fclean all
