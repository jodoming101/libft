# **************************************************************************** #
#                                                           LE - /             #
#                                                               /              #
#    Makefile                                         .::    .:/ .      .::    #
#                                                  +:+:+   +:    +:  +:+:+     #
#    By: jodoming <marvin@le-101.fr>                +:+   +:    +:    +:+      #
#                                                  #+#   #+    #+    #+#       #
#    Created: 2017/11/27 00:32:54 by jodoming     #+#   ##    ##    #+#        #
#    Updated: 2017/11/30 15:06:03 by jodoming    ###    #+. /#+    ###.fr      #
#                                                          /                   #
#                                                         /                    #
# **************************************************************************** #

NAME = libft.a

SRCS = ft_isalnum.c ft_putchar.c ft_putnbr_fd.c ft_strcmp.c ft_strncat.c \
	   ft_strstr.c ft_isalpha.c ft_putchar_fd.c ft_putstr.c ft_strcpy.c \
	   ft_strncmp.c ft_tolower.c ft_isascii.c ft_putendl.c ft_putstr_fd.c \
	   ft_strdup.c ft_strncpy.c ft_toupper.c ft_isdigit.c ft_putendl_fd.c \
	   ft_strcat.c ft_strlcat.c ft_strnstr.c ft_atoi.c ft_isprint.c \
	   ft_putnbr.c ft_strlen.c ft_strchr.c ft_strrchr.c ft_memset.c \
	   ft_bzero.c ft_memcpy.c ft_memccpy.c ft_memmove.c ft_memchr.c \
	   ft_memcmp.c ft_memalloc.c ft_memdel.c ft_strnew.c ft_strdel.c \
	   ft_strclr.c ft_striter.c ft_striteri.c ft_strmap.c ft_strmapi.c \
	   ft_strequ.c ft_strnequ.c ft_strsub.c ft_strjoin.c ft_strsplit.c \
	   ft_strtrim.c ft_itoa.c ft_lstnew.c ft_lstadd.c ft_lstdel.c \
	   ft_lstdelone.c ft_lstiter.c ft_lstmap.c ft_putstr_2d_fd.c ft_swap.c \
	   ft_isspace.c ft_match.c ft_strrev.c

INC = libft.h

OBJ = $(addprefix objects/, $(SRCS:.c=.o))

CFLAGS = -Wall -Werror -Wextra

all: $(NAME)

.PHONY: clean fclean re

objects:
	mkdir objects/

objects/%.o: ./%.c | objects
	gcc $(CFLAGS) -I $(INC) -c $< -o $@

$(NAME): $(OBJ)
	ar rcs $@ $(OBJ)

clean:
	/bin/rm -f $(OBJ)
	/bin/rm -rf objects

fclean: clean
	/bin/rm -f $(NAME)

re: fclean all
