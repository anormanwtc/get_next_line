# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: anorman <marvin@42.fr>                     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/05/21 16:00:27 by anorman           #+#    #+#              #
#    Updated: 2019/08/30 09:44:30 by anorman          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FLAGS = -Wall -Werror -Wextra
NAME = libft.a
FILES = ft_strchr.c\
		ft_strlen.c\
		ft_strdel.c\
		ft_lstnew.c\
		ft_lstadd.c\
		ft_lstaddend.c\
		ft_lstcat.c\
		ft_lstdel.c\
		ft_lstdelmid.c\
		ft_lstdelone.c\
		ft_strjoin.c\
	   	ft_strsub.c\
		ft_strcat.c\
		ft_memcpy.c

OBJ = $(FILES:%.c=%.o)

SRCDIR = srcs

HEADER = -I includes

all: $(NAME)

$(NAME):
	@gcc -c $(FLAGS) -I includes $(FILES:%=$(SRCDIR)/%)
	@echo "gcc -c $(FLAGS) -I includes FILES"
	@ar -rcs $(NAME) $(OBJ)
	@echo "ar -rcs $(NAME) OBJ"

clean:
	@rm -f $(OBJ)
	@echo "rm -f OBJ"

fclean: clean
	@rm -f $(NAME)
	@echo "rm -f $(NAME)"

re: fclean all
