# Meeting Ruby

To discover a programming language, you have to understand what are its
caracteristics. On the Ruby website, the language introduce itself like this:

> A dynamic, open source programming language with a focus on simplicity and
> productivity. It has an elegant syntax that is natural to read and easy to
> write.

Most of this description is subjective. The two objectives things here are:
dynamic and open source. We won't cover the open-source part so that leave us
with one thing...

## Being dynamic

There is two families of languages, dynamic and static. A dynamic language makes
it easy to alter its own behavior at _runtime_.

Each time I explain something, there is a new and unknown concept that is
showing up. You'll see this pattern quite often. Ok then what is runtime?

A piece of code writen in a given programming language goes through a few steps
before ending up in machine instructions. Here are those steps:

1. analysing the code, according to its syntax,
2. translating this code into other representations, easier to manipulate, and
3. being executed by the computer, to actually do what you wanted.

The last step is called the _runtime_, when your code actually _runs_.
Everything before this step can be called _compile-time_. _Compilation_ is the
translation of you code into something that can be executed by a machine. This
is why it's called compile-time.

You'll see later what altering the behavior of a program at runtime means.
Right now I'll give you an example showing how crazy, powerful, and dangerous it
is. When you're conceived your genes defines a lot of immutable - static - things
about you, your gender, the color of your eyes and so on. Imagine that you can
spot which gene is doing what and change it for as long as you want like getting
blue eyes just for a date. A dynamic language give you the keys to do that kind
of things, at the program's level...

## Writing Ruby programs, what you'll need

Code is written, mostly on computers. You'll need a _code editor_ to write code
as you need a text editor, like Microsoft Word, to write a letter. So first of
all, you'll need a code editor.

You'll also need a _Ruby implementation_. There is different tools that can
execute Ruby code. The Ruby language is a _specification_. This specification
tells you the syntax and the semantic (ie: the meaning) of Ruby code.
Implementations allows you to _run_ the code. There is a few implementations
of the Ruby programming language:

* the official one: MRI (Matz Ruby Implementation),
* the Java compatible one: JRuby,
* the tiny one: mruby,
* and more.

A code editor and a Ruby implementation are the two elements you need to start.
In the next chapter, we'll see what are the options to get those two things...
