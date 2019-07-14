How to use the handbook
=======================

For whom this book is written
-----------------------------

The DataLad handbook is not the DataLad documentation, and it is also
not an explanation of the computational magic that happens in the background.
Instead, it is a procedurally oriented, hands-on crash-course that invites
you to fire up your terminal and follow along.

**If you are interested in learning how to use DataLad, this handbook is for you.**

You do not need to be a programmer, computer scientist, or Linux-crank.
If you have never touched your computers shell before, you will be fine.
No knowledge about :term:`git` or :term:`git-annex` is required or necessary.
Regardless of your background and personal use cases for DataLad, the
handbook will show you the principles of DataLad, and from chapter 1 onwards
you will be using them.

How to read this book
---------------------

First of all: Be excited. DataLad can help you to manage your digital data
workflow in various ways, and in this book you will use many of them right
from the start.
There are many topics you can explore, if you wish:
Local or collaborative workflows, reproducible analyses, data publishing, ... .
If anything seems particulary exciting, you can go ahead, read it, *and do it*.
Therefore, **grab your computer, and be ready to use it**.

Every chapter will give you different challenges, starting from basic local
workflows to more advanced commands, and you will see your skills increase
with each. While learning, it will be easy to
**find use cases in your own work for the commands you come across**.

As the handbook is to be a practical guide it includes as many hands-on examples
as we can fit into it. Code snippets look like this, and you should
**copy them into your own terminal to try them out**, but you can also
**modify them to fit your custom needs in your own use cases**.
Note in the example below that shows the creation of a DataLad dataset how
we distinguish ``comments (#)`` from ``commands ($)`` and their output:

.. code-block:: bash

   # this is a comment used for additional explanations. Anything preceded by $ is a command to try.
   # if the line starts with neither # nor $, its the output of a command
   $ datalad create myfirstrepo
   [INFO   ] Creating a new annex repo at /home/adina/DataLad-101
   create(ok): /home/adina/DataLad-101 (dataset)
   
   ## display is off

The following two chapters have two different goals: All of the *Basics* sections
will show you the core DataLad functionality and challenge you to use it.
In *use cases* you will find concrete examples of DataLad applications for
general inspiration. We recommend to read the Basics first. Afterwards,
you might even consider :ref:`contribute` to this book by sharing your own use case.

Note that many challenges can have straightforward and basic solutions,
but a lot of additional options or improvements are possible.
Sometimes one could get lost in all of the available DataLad functionality.
For this reason we put all of the basics in plain sight, and those basics
will let you master a given task and get along comfortably.
Having the basics will be your multi-purpose swiss army knife.
But if you want to have the special knowledge for a very peculiar type
of problem set or that extra increase in skill,
you'll have to do a detour into some of the *hidden* parts of the book:
When there are command options that go beyond basics and
best practices, we hide them in foldable book sections in order
to not be too distracting for anyone only interested in the basics.
You can decide for yourself whether you want to check them out:

.. container:: toggle

    .. container:: header

       **Additional Content: Click here to show/hide further commands**

    Sections like this contain content that goes beyond the basics
    necessary to complete a challenge.

Note further that...

.. admonition:: Note for git-users

   DataLad uses :term:`git` and :term:`git-annex` underneath the hood. Readers that
   are familiar with these tools can find occasional notes on how a DataLad
   command links to a git(-annex) command or concept in boxes like this.
   There is, however, absolutely no knowledge of git or git-annex necessary
   to follow this book.

Apart from core DataLad commands (introduced in the second section of this book),
DataLad also comes with many extensions and advanced commands not (yet) referenced
in this handbook. The development of many of these features
is ongoing, and this handbook will incorporate all DataLad commands and extensions
*once they are stable* (that is, once the command(-structure) is likely to not
change in the future anymore). If you are looking for a feature but cannot find it in this
handbook, please take a look at the `documentation <http://docs.datalad.org>`_,
`write <LinkThisToContributing>`_ or
`request <https://github.com/datalad-handbook/book/issues/new>`_
an additional chapter if you believe it's a worthwhile addition, or
`ask a question on Neurostars.org <https://neurostars.org/latest>`_
with a ``datalad`` tag if you need help.


The storyline
^^^^^^^^^^^^^

Most of the sections in the upcoming chapter follow a continous **narrative**.
This narrative aims to be as domain-agnostic and relatable as possible, but
it also needs to be able to showcase all of the principles and commands
of DataLad. Therefore, we will build up together a DataLad project for the
fictional educational course ``DataLad-101``.

Envision yourself in the last educational course you took or taught:
Probably, you've created some files with notes you took, a directory
with slides or books for further reading, and a place where you stored
assigments and their solutions in. This is what we will be doing as well.
This project will start with creating the necessary directory structures,
populating them by ``installing`` and ``creating`` several
:term:`DataLad subdataset`\s, adding files and changing their content,
and executing simple scripts with input data to create results we can
publish with DataLad.

If you don't want to follow along and only read, there will be a
finished DataLad-101 project for you to download and explore in the future.


Lets get going!
---------------

If you have DataLad installed, you can dive straight into chapter 1. (Todo: link).
For everyone new, there are the sections :ref:`howto` as a minimal tutorial
to using the shell and :ref:`install` to get your DataLad installation set up.
