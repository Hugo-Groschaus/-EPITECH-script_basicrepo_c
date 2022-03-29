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

CFLAGS	=	-o

CPPFLAGS	=	-Wextra -Wall -iquote./includes/

CSFML	=	-l csfml-graphics -l csfml-system -l csfml-audio

LDFLAGS	=	-L.

LDLIBS	=	-lmy

all:	$(NAME)

$(NAME):	$(OBJ)
	$(MAKE) -C lib/my/
	$(CC) $(OBJ) $(CFLAGS) $(NAME) $(CPPFLAGS) $(LDFLAGS) $(LDLIBS)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)
	$(MAKE) fclean -C lib/my/

re:	fclean all

.PHONY: all clean fclean re
