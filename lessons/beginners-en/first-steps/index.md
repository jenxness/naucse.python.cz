## First commands in Python

Let's see if we installed `Python` successfully!

First open your terminal and we can now start Python (specifically, the Python console).
To do that, just write `python3` or `py` or `python` into the terminal:

``` plain
$ python3
Python 3.8.1 (default, Dec 24 2019, 17:02:07) 
[GCC 9.2.1 20191008] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

This command will print some information. In the first line, it shows which version of Python you have (you should have Python 3.8+).

The command line starts with a `>>>` symbol. This way Python prompts (asks) you for instructions. This is the same as the standard command line, but instead of commands like `cd` or `mkdir`, you write Python specific commands.

> [warning] What if previous command returns something else?
> If you are on Windows, the command to run is sometimes called `py` or `python` instead of `python3`, try that instead. If that does not work either:
> 
> Then most probably the Python installation `was not successful or complete`.
> 
> Please go back to [Python Installation]({{ lesson_url('beginners-en/install_vienna') }}) and try installing Python again according to the instructions for your operating system.
> 
> If something unexpected happened or you need help, please raise a hand and ask for a mentor support.
>
> It is very important that this first step works for all of you.
>
> If you are on `Mac` or `Linux` the `python` command will usually run `python version 2` which is `not` what we want - if `python3` works, perfect, if not, please try reinstalling the newest `python` or ask a mentor for help.

## Quick task 

If you have the terminal ready don't waste time! Type `print("Hello, world!")` in the Python terminal! 

{% filter solution %}

What happened? Python "printed out" `Hello, world!` for you. It's an old programming tradition, going back to 1970s. It is a traditional first command executed by people who are learning a given programming language, which illustrates the basic syntax of the language.

In Python one can simply execute `print("Hello, world!")`. In other programming languages it might not be that simple! Feel free to search for examples of a "Hello world" code in C++, Java, HTML, JavaScript or other languages. 

{% endfilter %}

## Python basics

Python can work as a simple calculator. Try running following commands in your Python and you should see these responses.

```pycon
>>> 1
1
>>> 42 + 3
45
>>> -1.1 + 12
10.9
>>> 2/3
0.6666666666666666
>>> 3*5
15
>>> 2**4
16
>>> 1e3 + 222
1222.0
>>> -8.3 + 2
-6.300000000000001
>>> 15%4
3
>>> 10_000 + 155
10155
>>> 17//3
5
>>> 2 + 3 * 4
14
>>> (2+3) * 4
20
```

> [note]
> Python prints the greater-than signs `>>>` and the answer by itself!
> You just write number and press Enter.

Notice that commands from the standard command line do not work here, although the window looks similar:

```pycon
>>> whoami
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'whoami' is not defined
```

This is an *error message* which appears every time when you do anything wrong. You will see a lot of them during the course. Have a look at it carefully so you can recognise it later.

If you got this far, congratulations! You have installed Python and it works. You can now quit the Python console and close the command prompt.

To quit, just type `exit()` with empty parentheses


<div class="highlight"><pre>
<span class="gp">&gt;&gt;&gt;</span> exit()
<span class="gp">$</span>
</pre></div>

The greater-than signs `>>>` change back to `$` or `>`. This tells you that you're back on the system prompt. Now commands like `whoami` and `cd` work again, but Python commands like `1 + 2` won't work. You can re-activate the Python prompt anytime you want by simply typing `python3`  


The terminal can be closed by typing `exit` or press `CTRL+D`.

```console
$ exit
```

As a last exercise, try to run the Python console again

- open the command prompt (the terminal)
- run Python
