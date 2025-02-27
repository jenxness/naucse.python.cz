# My First Program

```pycon
>>> 3 + 4
7
```

You can issue commands in the *Python interactive console*. 
But it has a disadvantage:
The program that you type is lost when the session ends.
It is good for trying simple commands. 
Very often however, you need a way to save more complex programs somewhere. 

Open your editor
(You should have an editor installed. If not, follow the instructions in 
[Editor installation]({{ lesson_url('beginners-en/install-editor')}}).)

Create a new file in your editor and type the following code:

```python
print("Hello world!")
```

{% if var('pyladies') -%}
{% set rootname = 'pyladies' %}
{%- else -%}
{% set rootname = 'naucse-python' %}
{%- endif %}

Then save the file as `hello.py`.
* You have to create the subdirectory named `02` in the `pyladies`
(or whatever folder name you've created last lecture) directory.
* Then you can store the file as `hello.py` in it.

If you can choose the *encoding* in your editor, you should use `UTF-8`.
If you can choose the file type, use `.py` or `All Formats`.

Some operating systems or editors hide extensions or add their own extensions.
You can check the real name using the command line.
Open your command line and change your current directory to the subdirectory you created -
for example by using the `cd` command to `~/pyladies/02`.

List what is in the directory using the command `ls` (Mac or Linux) or `dir` (Windows) 
and check that the filename is really `hello.py` and not, for example, `hello.py.txt`.

## Executing Your Program

Open the command line.
Change to the `~/pyladies/02` directory and issue the following command:

```console
python3 hello.py
```

> [note]
> You have learned about the command line in 
> a [previous lesson]({{ lesson_url('beginners-en/cmdline')}}) which shows how to change the current directory 
> using the `cd` command.


After you run `python3 hello.py` you should see the program responding with writing `Hello world!` into the terminal.

If it does not work, make sure that:

* You are in the correct directory: `~/pyladies/02`
  (you need to replace `~/pyladies` with the directory that you have created previously).
* The `hello.py` file contains the correct command, including quotes and parentheses.
* Do not type `$` or `>` character in the command line – it is there to indicate that this is a command line.
  It is printed by the operating system after any program has finished.
  You should type only: `python3 hello.py`.

If it still does not work, **ask your coach for help!**


> [style-note] Note about code style
>
> It does not usually matter where you use space in Python inside a command. 
> The command `print("Hello world!")` has the same effect as:
>
> ```python
> print      (   "Hello world!"     )
> ```
>
> It is however a good practice to follow some typical guidelines.
> In English, we do not write a space after an opening parenthesis.
> In Python, we do not write a space even between `print` and `(`.
> The recommended style is:
>
> ```python
> print("Hello world!")
> ```
>
> The spaces between the quotes have a meaning: If you type
> `"    Hello      world!"`, then the extra spaces are printed.
