HELL TEST SUITE

## Description
The aim of this project is to contribute with some tests for our partners Shells. Our test file covers every task you can find on 0x16. C - Simple Shell but we found especially useful to handle message errors.
## Content

[hsh_vs_sh](https://github.com/MatiasMtz/holberton-system_engineering-devops/tree/main/0x00-shell_basics) Text file has four sections: 
- Basic tests: Here you can find tests like typing random letters, pressing "enter" or "tab" buttons, handling dots, among others
- Absolute Path tests: As the name says the Absolute Path main function is to check commands with the full directory path plus the file name. An example could be: /usr/bin/ls
- Relative Path tests: First, we have to define Relative Paths, mainly, they are the path related to the present working directory. So, our tests checks if commands introduced in this way also works properly. Taking the previous example about Absolute Paths, the Relative Path of "/usr/bin/ls" is "ls".
- Advanced Tasks tests: Last but not least, Advanced Tasks tests contains many commands to check 0x16. C - Simple Shell advanced tasks such as: alias, setenv, unsetenv and many others. 

## How to use

- Clone our directory to your working space or copy the content of hsh_vs_sh into a text file.

```bash
  git clone 
```

- Compile your Shell code this way

```bash
  gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -g -o hsh 
```

- Move the file "hsh_vs_sh" from the folder you clone in previous steps to the folder where you compile (or use absolute paths to execute the "cat" command)
- Introduce the following command

```bash
   cat hsh_vs_sh | valgrind --track-origins=yes --leak-check=full ./hsh
```

This way you are going to be checking your shell behaviour but also if there is any memory leak or error in the process.

If you want to compare your results with the ones of sh you should just run the test but against sh

```bash
   cat hsh_vs_sh | sh
```
## References

| TEXT                | DESCRIPTION                                                        |
| ------------------- | ------------------------------------------------------------------ |
| ##### COMMAND ##### | The command which is going to be executed |

## Authors

[Axel Bouvier](https://github.com/AxelBouvierM) and [Matías Martínez](https://github.com/MatiasMtz) from Holberton School cohorte #17.


