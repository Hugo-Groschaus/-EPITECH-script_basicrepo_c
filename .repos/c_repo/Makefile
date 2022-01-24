
##
## EPITECH PROJECT, 2022
## Makefile
## File description:
## Makefile
##

CC	=	gcc

PTH	=	src/

SRC	=	$(PTH)main.c

OBJ	=	$(SRC:.c=.o)

NAME	=	exe

CFLAGS	=	-Wextra -Wall -iquote./includes/ -L. -lmy

all:	$(NAME)

$(NAME):	$(OBJ)
	$(MAKE) -C lib/my/
	$(CC) $(SRC) -o $(NAME) $(CFLAGS)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)
	$(MAKE) fclean -C lib/my/

re:	fclean all

.PHONY: all clean fclean re