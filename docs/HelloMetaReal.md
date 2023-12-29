---
sidebar_position: 1
---

# Hello MetaReal

## Install MetaReal

First, you need to [install](../install) MetaReal. \
If you installed MetaReal correctly, the following command should display the installed compiler version.

```bash
$ metareal --version
MetaReal compiler version 1.0.0
MetaReal core verified as mr-core, version 1.0.0
MetaReal port verified as mr-port, version 1.0.0
```

Once you installed it, create a file named `start.mr` and start coding your first MetaReal program. \
By the way, the default MetaReal file extension is `.mr`.

## Say Hello

We start simple. A program that prints out the `Hello MetaReal` message into terminal.
Our program would be like this. There are no dependencies or libraries and no `main` function. Just one line of code!

```mr title="start.mr"
print("Hello MetaReal")
```

Now, save the file and go back to the terminal window.
On Linux or macOS, enter the following commands to compile and run the file:

```bash
$ metareal start.mr
$ ./start
Hello MetaReal
```

And on Windows:

```batch
> metareal start.mr
> .\start
Hello MetaReal
```

And you have it! The first program that you wrote in MetaReal programming language. \
There are three essential concepts in this code to consider:

1. The MetaReal programming language has no `main` function (even though it's a compiler language). \
All written codes are considered part of the `main` function by default (except the definitions). Unless the programmer explicitly wants to define it.
2. The `print` function displays a message in the terminal window. \
It's a built-in function. And you don't have to import any library to use it.
3. The `"Hello MetaReal"` is called a **string**. \
You can work with textual data via string data type. We will take a closer look at these objects in later chapters.

## One Step Further

Let's go one step further. A program that gets user's name and greets them.

```mr title="start.mr"
name = input("Enter your name: ")
print("Hello " + name + "!")
```

Compile and run it like before, and you will see the following result:

```bash
Enter your name: Foo
Hello Foo!
```

In this example, there were three new things:

1. The `input` function gets a string from the user. \
Also, it prints out the prompt given to it as a parameter. `"Enter your name: "` in this case.
2. The `name =` part is called a **variable assignment**. \
It creates a new variable called `name` and stores result of the `input` function (user's input). You can access the stored data by calling name of the variable.
3. The `+` operator concatenates two strings and unifies them into one.

We will study these concepts in more detail in later sections! But as for now, you are ready to start learning the MetaReal programming language. \
A summary of what you learned:

* The `print` and `input` functions
* String data type
* Variable assignment and variable access
* String concatenation via the `+` operator
* Compiling MetaReal code

Next, we will introduce one of the most useful MetaReal features: \
**mpm** or **MetaReal Package Manager**.
