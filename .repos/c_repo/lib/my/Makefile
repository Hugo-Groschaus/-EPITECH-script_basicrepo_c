##
## EPITECH PROJECT, 2022
## Makefile lib
## File description:
## makefile
##

SRC	=	main.c

CC	=	gcc

RM	=	rm -f

OBJ	=	$(SRC:.c=.o)

NAME	=	lib

all:	$(NAME)

$(NAME):	$(OBJ)
	$(CC) -o $(NAME) $(OBJ)
	ar rc libmy.a $(OBJ)
	cp libmy.a ../../
	cp my.h ../../includes/

clean:
	$(RM) $(OBJ)

fclean:	clean
		$(RM) $(NAME)
		$(RM) libmy.a
		$(RM) ../../libmy.a

re: fclean all

.PHONY: all clean fclean re