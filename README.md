# eggshells

Unix shells written in C++11, C99 and Rust, as a hobby.
These are all quite similar in functionality and mostly work in progresses that I update sporadically.

## [rsh](https://github.com/vrmiguel/rsh) - Rust implementation

![rsh](https://user-images.githubusercontent.com/36349314/87332790-82a29e00-c512-11ea-9345-8e96bb35c52b.png)

### Features

* Runs any program in `/bin` that does not require `sudo`;
* Piped commands, currently limited to a single pipe.
* Save the output of simple and piped commands to a file with `>`.
    * e.g. `ls -li | tr s x > output`
* Signal handler;
* Implements `cd`;
* Unwinds before exit, interrupted or not;
* Prompt similar to `bash`'s default.

## [minishell-2](https://github.com/vrmiguel/rsh) - C++11 implementation

![minishell-2](https://user-images.githubusercontent.com/36349314/87333022-e3ca7180-c512-11ea-984f-2dfd99ff1e14.png)

### Features

* Runs any program in `/bin` that does not require `sudo`;
* Piped commands, (10 pipes maximum, but that can be easily increased within the code)
* Signal handler;
* Implements `cd`;
* Unwinds before exit, interrupted or not;
* Prompt similar to `bash`'s default.

## [minishell](https://github.com/vrmiguel/minishell) - C99 implementation

![minishell](https://raw.githubusercontent.com/vrmiguel/miniShell/master/print.jpg)

Unix shell I made a loooong time ago as an university assignment. This is honestly not good and a new one in ANSI C is in the works.

Features:
* Simple commands, such as "ls", "ls -li", "clear", "help", etc;
* Piped commands, such as "ls -li | tr s x". Commands with more than two pipelines are also supported;
* Saving to file, such as "ls -li > file_list";
* Reading from file, such as "sort < file_list".
  

