# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: yfontene <yfontene@student.42porto.com>    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/05/11 09:21:07 by yfontene          #+#    #+#              #
#    Updated: 2023/05/23 15:52:41 by yfontene         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

BLUE	=	\033[0;34m
GREEN	=	\033[0;32m
PURPLE	=	\033[0;35m
END		=	\033[0m
IYELLOW	=	\033[0;93m

CC		= 	cc
CFLAGS	=	-Wall -Wextra -Werror

HEADER	=	ft_printf.h
NAME 	= 	libftprintf.a 

SRCS	= 	ft_printf_base.c ft_printf.c ft_printf_type.c ft_printf_hexp.c\

RM		=	rm -rf
AR		=	ar rcs

OBJS	=	$(SRCS:.c=.o)

all:		$(NAME)

$(NAME): 		$(OBJS)
				echo "$(BLUE)Compiling Libft...$(END)"
				$(AR) $(NAME) $(OBJS)
				@echo "$(GREEN)Libft succesfully compiled!$(END)"

clean: 		
				@rm -rf $(OBJS)
				@echo "$(PURPLE)Libft objects deleted!$(END)"

fclean: 		clean
				@rm -rf $(NAME)
				@echo "$(RED)Libft lib deleted!$(END)"

re:				fclean	all

author: 
				@echo "$(IYELLOW)'yfontene'$(END)"

.PHONY: 		all clean fclean re