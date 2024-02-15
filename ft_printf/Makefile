# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: pablogon <pablogon@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/01/30 19:18:54 by pablogon          #+#    #+#              #
#    Updated: 2024/02/09 23:34:33 by pablogon         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

LIB = ar rcs
RM = rm -f

CC = cc
CFLAGS = -Wall -Wextra -Werror

NAME = libftprintf.a

SRCS = ft_printf.c ft_hexa_mayus.c ft_hexa_min.c ft_num_nosign.c ft_punt_hexa.c \
ft_putchar.c ft_putnbr.c ft_putstr.c ft_strlen.c

OFILES = $(SRCS:.c=.o)
INCLUDE = ft_printf.h

all: $(NAME)

$(NAME):$(OFILES) $(INCLUDE)
	$(LIB) $(NAME) $(OFILES) 

.c.o:
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	$(RM) $(OFILES)

fclean: clean
	$(RM) $(NAME)

re: fclean all
.PHONY: all clean fclean re ar bonus
