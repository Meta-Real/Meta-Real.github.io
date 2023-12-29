---
sidebar_position: 2
---

# What is MPM?

**MPM** or **MetaReal Package Manager** is a set of tools for organizing, downloading, and uploading MetaReal projects and packages. \
It directly interacts with the MetaReal main repository and can download packages to improve your project quality. \
Packages are MetaReal projects created by programmers globally to simplify specific tasks and help programmers focus more on their program logic rather than its implementation. \
To start, let's get the installed MPM version.

```bash
$ mpm --version
MPM (MetaReal Package Manager) version 1.0.0
MPM is running on MetaReal version 1.0.0
```

Or you can use the command down below.

```bash
$ metareal --mpm --version
MPM (MetaReal Package Manager) version 1.0.0
MPM is running on MetaReal version 1.0.0
```

MPM's reason for existence is:

1. To download available packages from the MetaReal online repository.
2. To upload packages that you created to the MetaReal online repository.
3. To organize, update, and link your installed packages.

## Install Packages

Let's install a sample MetaReal project to see the MPM in action.

:::tip
To install the package properly, check your network connection. \
If the MPM fails to download the project due to network issues, MPM will schedule your installation request until it finds a stable network connection.
:::

We will install `mr_sample`. It is a sample package that includes various functions and data structures. \
Use the following command to install the `mr_sample` package.

```bash
$ mpm --install mr_sample
...
downloading process
...
MPM: "mr_sample" package installed successfully
```

To check if the package installation is complete, type down the following command that displays the package information.

```bash
$ mpm --info mr_sample
Library:      mr_sample
Version:      1.0.0
Last Update:  29/12/2023 9:27:30
Author:       MetaReal
Description:
mr_sample is a sample library that features all of MetaReal's capabilities.
```

## Write The Code

We will write a simple program that uses the `mr_sample` library.

```mr title="mpm.mr"
import mr_sample

mr_sample.say("Hello World")
```

The `import` is a MetaReal keyword that imports definitions of a library into your program. \
You can access a particular definition with the following syntax: `<library name>.<definition>`.
If you compile it, you get a `Hello World` message, just like the print function.

```bash
$ metareal mpm.mr
$ ./mpm
Hello World
```

A summary of what you learned:

* MPM and its use cases
* `mpm --version`, `mpm --install`, and `mpm --info` commands
* `mr_sample` library
* The `import` keyword
* Accessing definitions of a library

This section was a quick but useful guide about the powerful MetaReal Package Manager. \
We will return to the MPM for more complicated installations and when we want to create our project and upload it into the MetaReal repository. \
But as for now, let's start learning the MetaReal, for real.
