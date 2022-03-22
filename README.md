<h1 align="center">Libft</h1>
<h4>This is the first project as a student in 42. In this project you will have to replicate a few functions that alredy exist in standard c libraries, and create some of your own.</h4>

## 📖 Content 📖

### 📚 Libc Functions 📚

- **Type Functions** : [`isalnum`](./src/ft_isalnum.c) [`isalpha`](./src/ft_isalpha.c) [`isascii`](./src/ft_isascii.c) [`isdigit`](./src/ft_isdigit.c) [`isprint`](./src/ft_print.c) [`toupper`](./src/ft_toupper.c) [`tolower`](./src/ft_tolower.c)

- **String Functions** : [`atoi`](./src/ft_atoi.c) [`strchr`](./src/ft_strchr.c) [`strdup`](./src/ft_strdup.c) [`strlcat`](./src/ft_strlcat.c) [`strlcpy`](./src/ft_strlcpy.c) [`strlen`](./src/ft_strlen.c) [`strncmp`](./src/ft_strncmp.c) [`strnstr`](./src/ft_strnstr.c) [`strrchr`](./src/ft_strrchr.c)

- **Memory Functions** : [`bzero`](./src/ft_bzero.c) [`memchr`](./src/ft_memchr.c) [`memcmp`](./src/ft_memcmp.c) [`memcpy`](./src/ft_memcpy.c) [`memmove`](./src/ft_memmove.c) [`memset`](./src/ft_memset.c) [`calloc`](./src/ft_calloc.c)

### ✍️ Aditional Functions ✍️

- **String Functions** : [`itoa`](./src/ft_itoa.c) [`split`](./src/ft_split.c) [`striteri`](./src/ft_striteri.c) [`strjoin`](./src/ft_strjoin.c) [`strmapi`](./src/ft_strmapi.c) [`strtrim`](./src/ft_strtrim.c) [`substr`](./src/ft_substr.c)

- **Print Functions** : [`putchar`](./src/ft_putchar_fd.c) [`putendl`](./src/ft_putendl_fd.c) [`putnbr`](./src/ft_putnbr_fd.c) [`putstr`](./src/ft_putstr_fd.c)

### 🚀 Bonus Functions 🚀

- **Struct Functions** : [`lstaddback`](./src/ft_lstaddback.c) [`lstaddfront`](./src/ft_lstaddfront.c) [`lstclear`](./src/ft_lstclear.c) [`lstdelone`](./src/ft_lstdelone.c) [`lstiter`](./src/ft_lstiter.c) [`lstlast`](./src/ft_lstlast.c) [`lstmap`](./src/ft_lstmap.c) [`lstnew`](./src/ft_lstnew.c) [`lst`](./src/ft_lstsize.c)

## 💣 Adding Libft to your project 💣

#### To add Libft in your project you should add this lines on your Makefile:

`LIBS_DIR	= libs`

`LIBS			= $(LIBS_DIR)/Libft/libft.a \`

`LIBS_HEADERS	= -I $(LIBS_DIR)/Libft/include/ \`

#### Add in your `CFLAGS` rule:

`CFLAGS		= -Wall -Wextra -Werror -g $(LIB_HEADERS)`

#### Add in your `$(NAME): $(OBJ)`:

`$(NAME): $(OBJ) $(LIBS)`

`⠀⠀⠀⠀⠀⠀⠀⠀@$(CC) $(OBJ) $(LIBS) -o $(NAME)`

#### Add in your `%.o:%.c` rule:

`@$(CC) -c $(CFLAGS) -o $@ $^`

#### And last thing is to add a new rule:

`$(LIBS_DIR)/Libft/libft.a:`

`⠀⠀⠀⠀⠀⠀⠀⠀@make -C $(LIBS_DIR)/Libft`

#### If you want to include your own libraries too:

`INC				= -I $("YOUR_INCLUDE_DIR") $(LIBS_HEADERS)`

`CFLAGS		= -Wall -Wextra -Werror -g $(INC)`

#### Anyway, I have some [`C templates`](https://github.com/Zsolt42/42_Cursus_zpalfi/tree/main/C_Templates) if you want to see more clearly how to do it 😄😄

## 💯 Mark 💯

<p align="center">
  <a align="center">
    <img src="./Addings/Mark.png">
  </a>
</p>
