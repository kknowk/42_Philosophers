NAME = philo
CC = cc

CFLAGS = -Wall -Wextra -Werror
# CFLAGS += -g -fsanitize=address
CFLAGS += -g -fsanitize=thread

SRCS = philo_init.c \
	main.c \
	philo_death.c \
	philo_routine.c \
	utils.c \
	utils_err.c

OBJS = $(SRCS:.c=.o)

all: $(NAME)

$(NAME): $(OBJS)
	$(CC) $(CFLAGS) $(OBJS) -o $(NAME)

clean:
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(NAME)

re: fclean all

.PHONY: all clean fclean re
