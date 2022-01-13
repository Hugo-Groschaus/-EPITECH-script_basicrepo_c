##
## EPITECH PROJECT, 2022
## Makefile 
## File description:
## Makefile
##

CC      =       gcc

PTH     =       src/

SRC     =       $(PTH)main.c

OBJ     =       $(SRC:.c=.o)

NAME    =       navy

CFLAGS  =       -iquote ./includes/ -Wextra -Wall

all:    $(NAME)

$(NAME):        $(OBJ)
        $(CC) $(SRC) -o $(NAME) $(CFLAGS)

clean:
        rm -f $(OBJ)

fclean: clean
        rm -f $(NAME)

re:     fclean all

.PHONY: all clean fclean re
