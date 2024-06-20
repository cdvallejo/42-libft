<h1 align="center">
🕹 LIBFT - 42 Proyect
</h1>

<p align="center">
	<b><i>The first and necessary project, your best friend</i></b><br>
</p>

<p align="center">
	<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/Falitomal/Libft-42?color=lightblue" />
	<img alt="Code language count" src="https://img.shields.io/github/languages/count/Falitomal/Libft-42?color=yellow" />
	<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/Falitomal/Libft-42?color=blue" />
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/Falitomal/Libft-42?color=green" />
</p>

My library prepared for get next line and printf, with which I have obtained the 125 points.

This is a essential cursus library, with a focus on safety and some extra functions that do stuff like return the absolute value, return the power of an int, return whether a string will overflow an int if passed to atoi and free a pointer and point it to NULL.

## Description 
Creation of my own library (libft.a) with standard C functions, as well as some additional useful functions.

* Project developed in C language.
* The project compiles with the 'norma' (Norminette).
* Makefile is included which compiles the files source to the required output (.a) with the -Wall, -Werror and -Wextra flags.


### Mandatory Functions to replicate

| Function | Description |
| :------: | :---------: |
| ``ft_atoi`` | Reads a String, and, after ignoring spaces with ``ft_isspace``, saves the string into an integer |
| ``ft_bzero`` | Writes ``n`` zeroes to the string ``s`` |
| ``ft_calloc`` | Reserves ``x`` blocks of ``y`` bits of memory |
| ``ft_isalnum`` | Returns ``1`` if the input is a number or a letter in the ``ASCII`` table |
| ``ft_isalpha`` | Returns ``1`` if the input is a letter in the ``ASCII`` table |
| ``ft_isascii`` | Returns whether or not a value belongs to the ``ASCII`` table |
| ``ft_isdigit`` | Returns ``1`` if the input is a number in the ``ASCII`` table |
| ``ft_isprint`` | Returns whether a character is printable |
| ``ft_itoa`` | Saves the given number as a string (char array) |
| ``ft_memccpy`` | Copies from one memory point to another, until the specified character is copied or until ``n`` bytes are copied |
| ``ft_memchr`` | Looks for a matching character inside a part of the memory |
| ``ft_memcmp`` | Compares two parts of memory, returning ``0`` if they're the same, or else a nonzero value |
| ``ft_memcpy`` | Copies from one part of memory to another, ignoring possible overlaps |
| ``ft_memmove`` | Copies from one part of memory to another, preventing possible overlaps |
| ``ft_memset`` | Assigns a character ``n`` times to a part of the memory |
| ``ft_putchar_fd`` | Prints a character to the given file descriptor |
| ``ft_putendl_fd`` | Prints a string followed by a new line ``\n`` to a given file descriptor |
| ``ft_putnbr_fd`` | Prints number to the given file descriptor |
| ``ft_putstr_fd`` | Prints string to the given file descriptor |
| ``ft_split`` | Splits a string according to a given separator character |
| ``ft_strchr`` | Looks for a specific character inside a given string |
| ``ft_strdup`` | Saves enoug space and duplicates a string |
| ``ft_strjoin`` | Concatenates two strings allocating enough space first |
| ``ft_strlcat`` | Concatenates two strings ensuring it ends with ``\0`` |
| ``ft_strlcpy`` | Copies ``n - 1`` bytes from a source string to a destination string |
| ``ft_strlen`` | Returns length of a string |
| ``ft_strmapi`` | Applies a function (mapping) to every element in a string |
| ``ft_strncmp`` | Compares two strings up to the n-th character |
| ``ft_strnstr`` | Tries to find a substring (``needle``) in a second string (``haystack``) before the n-th char is reached |
| ``ft_strrchr`` | Looks for a given character in a string, reading it from back to front |
| ``ft_strtrim`` | Removes occurrences of characters in a string from the start and end of another one |
| ``ft_substr`` | Copies from the n-th char of a string |
| ``ft_tolower`` | Makes every uppercase character in a string lowercase |
| ``ft_toupper`` | Makes every lowercase character in a string uppercase |

## Bonus
For this part we implemented a struct defining the well-known linked lists
```C
typedef	struct	s_list
{
	void		*content;
	struct	s_list	*next;
}			t_list;
```

Bonus functions to implement

| Bonus Function | Description |
| :------------: | :---------: |
| ``ft_lstnew`` | Creates new node allocating with ``malloc`` |
| ``ft_lstadd_front`` | Adds new node at the beginning of the linked list |
| ``ft_lstsize`` | Returns number of elements of linked list |
| ``ft_lstlast`` | Retrieves last node of the list |
| ``ft_lstadd_back`` | Adds new node at the end of the linked list |
| ``ft_lstdelone`` | Deletes, frees, and applies function del to content of a given node |
| ``ft_lstclear`` | Deletes a given element and every element after that |
| ``ft_lstiter`` | Applies a function to the content of every node of the linked list |
| ``ft_lstmap`` | Applies function to a copy of the list, freeing when necessary |
| ``ft_lstget_at`` | ``[EXTRA]`` Retrieves linked list node at idex ``i``, or ``NULL``|


The bonus rule created in the Makefile allows to compile the functions to manipulate linked lists.
The defnition of the struct is:

<img width="288" alt="Screen Shot 2023-03-16 at 6 05 58 PM" src="https://user-images.githubusercontent.com/121127625/225697467-b31a601a-62e8-40e8-a6d2-f1545a043612.png">


All the bonus functions are named like ft_function_bonus.c

```
make all		Compiles the libft.a file
make bonus		Compiles all bonus files instead of the mandatory ones
make norminette		Checks Norm for all .c and .h files in the libft/ folder	
```

