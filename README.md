<h1 align="center">Libft</h1>
<h4>This is the first project as a student in 42. In this project you will have to replicate a few functions that alredy exist in standard c libraries, and create some of your own.</h4>

## 📖 Content 📖

### 📚 Libc Functions 📚

| Functions | Type | Prototype | What it does? |
| --------- | ---- | --------- | ------------- |
| [isalnum](./src/ft_isalnum.c)| Type | int ft_isalnum(int c) | if c is a digit or a letter returns 1, else return 0 |
| [isalpha](./src/ft_isalpha.c)| Type | int ft_isalpha(int c) | if `c` is a letter returns 1, else return 0. |
| [isascii](./src/ft_isascii.c)| Type | int ft_isascii(int c) | if `c` is in ascci table return 1, else return 0. |
| [isdigit](./src/ft_isdigit.c)| Type | int ft_isdigit(int c) | if `c` is a digit returns 1, else return 0. |
| [isprint](./src/ft_isprint.c)| Type | int ft_isprint(int c) | if `c` is printeabel returns 1, else return 0. |
| [toupper](./src/ft_toupper.c)| Type | int ft_toupper(int c) | if `c` is a lower case letter, turns it upper case. |
| [tolower](./src/ft_tolower.c)| Type | int ft_tolower(int c) | if `c` is a upper case letter, turns it lower case. |
| [atoi](./src/ft_atoi.c)      | String | int ft_atoi(const char *s) | Converts the string `s` to an integer (int). |
| [strchr](./src/ft_strchr.c)  | String | char *ft_strchr(const char *s, int c) | Searches for the first occurrence of the character `c` (an unsigned char) in the string pointed to by the argument `s`. |
| [strdup](./src/ft_strdup.c)  | String | char *ft_strdup(const char *s) | Returns a pointer to a null-terminated byte string, which is a duplicate of the string pointed to by `s`. |
| [strlcat](./src/ft_strlcat.c)| String | int	ft_strlcat(char *dst, const char *src, size_t n) | Appends string `src` to the end of `dst`. It will append at most `n` – strlen(dst) – 1 characters, and returns the combined length of both `src` and `dst` strings. |
| [strlcpy](./src/ft_strlcpy.c)| String | int	ft_strlcpy(char *dst, const char *src, unsigned long int n) | Copies up to `n` - 1 characters from the NUL-terminated string `src` to `dst`, NUL-terminating the result. |
| [strlen](./src/ft_strlen.c)  | String | size_t	ft_strlen(const char *s) | Takes a string `s` as an argument and returns its length. |
| [strncmp](./src/ft_strncmp.c)| String | int	ft_strncmp(const char *s1, const char *s2, size_t n) | Compares at most the first `n` bytes of `str1` and `str2`. |
| [strnstr](./src/ft_strnstr.c)| String | char	*ft_strnstr(const char *haystack, const char *needle, size_t len) | locates the	first occurrence of the	null-terminated string `needle` in the	string `haystack` , where not more than	`n` characters are searched. |
| [strrchr](./src/ft_strrchr.c)| String | char	*ft_strrchr(const char *s, int c) | Searches for the last occurrence of the character `c` (an unsigned char) in the string pointed to by the argument `s`. |
| [bzero](./src/ft_bzero.c)    | Memory | void	ft_bzero(void *s, size_t n) | Erases the data in the `n` bytes of the memory starting at the location pointed to by `s`, by writing zeros (bytes containing '\0') to that area. |
| [memchr](./src/ft_memchr.c)  | Memory | void	*ft_memchr(const void *s, int c, size_t n) | Searches for the first occurrence of the character `c` (an unsigned char) in the first `n` bytes of the string pointed to, by the argument `s`. |
| [memcmp](./src/ft_memcmp.c)  | Memory | int	ft_memcmp(const void *s1, const void *s2, size_t n) | Compares the first `n` bytes of memory area `s1` and memory area `s2`. |
| [memcpy](./src/ft_memcpy.c)  | Memory | void	*ft_memcpy(void *dest, const void *src, size_t n) | Copies `n` characters from memory area `src` to memory area `dest`. |
| [memmove](./src/ft_memmove.c)| Memory | void	*ft_memmove(void *dest, const void *src, size_t n) | Copies `n` characters from `src` to `dest`, but for overlapping memory blocks, memmove() is a safer approach than memcpy(). |
| [memset](./src/ft_memset.c)  | Memory | void	*ft_memset(void *b, int c, size_t n) | Copies the character `c` (an unsigned char) to the first `n` characters of the string pointed to, by the argument `b`. |
| [calloc](./src/ft_calloc.c)  | Memory | void	*ft_calloc(size_t count, size_t size) | Allocates the requested memory and returns a pointer to it. |

### ✍️ Aditional Functions ✍️

| Functions | Type | Prototype | What it does? |
| --------- | ---- | --------- | ------------- |
| [itoa](./src/ft_itoa.c)        | String | char	*ft_itoa(int n)                                           | Allocate (with malloc(3)) and returns a “fresh” string ending with ’\0’ representing the integer `n` given as argument. Negative numbers must be supported. If the allocation fails, the function returns NULL. |
| [split](./src/ft_split.c)      | String | char	**ft_split(char const *s, char c)                         | Allocates (with malloc(3)) and returns an array of “fresh” strings (all ending with ’\0’, including the array itself) obtained by spliting `s` using the character `c` as a delimiter. If the allocation fails the function returns NULL. |
| [striteri](./src/ft_striteri.c)| String | void	ft_striteri(char *s, void (*f)(unsigned int, char*))      | Applies the function `f` to each character of the string `s` passed as argument, and passing its index as first argument. Each character is passed by address to `f` to be modified if necessary. |
| [strjoin](./src/ft_strjoin.c)  | String | char	*ft_strjoin(char *s1, char *s2)                           | Allocates (with malloc(3)) and returns a “fresh” string ending with ’\0’, result of the concatenation of `s1` and `s2`. If the allocation fails the function returns NULL. |
| [strmapi](./src/ft_strmapi.c)  | String | char	*ft_strmapi(char const *s, char (*f)(unsigned int, char)) | Applies the function `f` to each character of the string `s` passed as argument by giving its index as first argument to create a “fresh” new string (with malloc(3)) resulting from the successive applications of `f`. |
| [strtrim](./src/ft_strtrim.c)  | String | char	*ft_strtrim(char const *s1, char const *set)              | Allocates (with malloc(3)) and returns a copy of the string `s1` given as argument without the characters given as `set` at the beginning or at the end of the string. If `s1` has no `set` characters at the beginning or at the end, the function returns a copy of `s1`. If the allocation fails the function returns NULL. |
| [substr](./src/ft_substr.c)    | String | char	*ft_substr(char const *s, unsigned int start, size_t len) | Allocates (with malloc(3)) and returns a “fresh” substring from the string `s` given as argument. The substring begins at indexstart and is of size `len`. If `start` and `len` aren’t refering to a valid substring, the behavior is undefined. If the allocation fails, the function returns NULL |
| [`putchar`](./src/ft_putchar_fd.c)| Print | void	ft_putchar_fd(char c, int fd) | Writes the `c` character on the file descriptor given |
| [`putendl`](./src/ft_putendl_fd.c)| Print | void	ft_putendl_fd(char *s, int fd)| Writes the `s` string on the file descriptor given followed by a new endline |
| [`putnbr`](./src/ft_putnbr_fd.c)  | Print | void	ft_putnbr_fd(int nbr, int fd) | Writes the `nbr` number on the file descriptor given |
| [`putstr`](./src/ft_putstr_fd.c)  | Print | void	ft_putstr_fd(char *s, int fd) | Writes the `s` string on the file descriptor given |

### 🚀 Bonus Functions 🚀

| Functions | Type | Prototype | What it does? |
| --------- | ---- | --------- | ------------- |
| [`lstaddback`](./src/ft_lstaddback.c)  | Struct | void ft_lstadd_back(t_list **lst, t_list *new) | Adds the `new` elemnt to the end of the `lst` list|
| [`lstaddfront`](./src/ft_lstaddfront.c)| Struct | void ft_lstadd_front(t_list **lst, t_list *new) | Adds the `new` elemnt to the start of the `lst` list |
| [`lstclear`](./src/ft_lstclear.c)      | Struct | void ft_lstclear(t_list **lst, void (*del)(void*)) | Deletes and frees every element of the list `lst` using the `del` function and free(3). Last pointer of the list must be set to NULL. |
| [`lstdelone`](./src/ft_lstdelone.c)    | Struct | void ft_lstdelone(t_list *lst, void (*del)(void*)) | Takes as a parameter a link’s pointer address and frees the memory of the link’s content using the function `del` given as a parameter, then frees the link’s memory using free(3). The memory of next must not be freed under any circumstance. Finally, the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel in the mandatory part). |
| [`lstiter`](./src/ft_lstiter.c)        | Struct | void ft_lstiter(t_list *lst, void (*f)(void *)) | Iterates the list lst and applies the function `f` to each link. |
| [`lstlast`](./src/ft_lstlast.c)        | Struct | t_list *ft_lstlast(t_list *lst) |
| [`lstmap`](./src/ft_lstmap.c)          | Struct | t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *)) | Iterates a list lst and applies the function f to each link to create a “fresh” list (using malloc(3)) resulting from the successive applications of f. If the allocation fails, the function returns NULL. |
| [`lstnew`](./src/ft_lstnew.c)          | Struct | t_list *ft_lstnew(void *content) | Allocates (with malloc(3)) and returns a “fresh” link. The variables content and content_size of the new link are initialized by copy of the parameters of the function. If the parameter content is nul, the variable content is initialized to NULL and the variable content_size is initialized to 0 even if the parameter content_size isn’t. The variable next is initialized to NULL. If the allocation fails, the function returns NULL. |
| [`lstsize`](./src/ft_lstsize.c)        | Struct | int ft_lstsize(t_list *lst) | Count the number of elements in the list `lst` |

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
