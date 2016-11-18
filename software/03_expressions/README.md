# The evaluation of expressions

One fundamental thing in programming is understanding what an expression is,
what they could do. Lets start playing with expressions in you environment
right now!

## Diving in IRB: Interactive RuBy

When you installed Ruby, you also get a program called `irb`. If you type
`irb` in a new terminal, an discussion will start between you and Ruby:

![Launching IRB](TODO)

IRB will wait for you to type some _expressions_, once you type `Enter`, IRB
IRB will _evaluate_ them and give back to you the _result of the evaluation_.
Here is an example of an _IRB session_:

``` bash
$ irb
```

```
irb:001> 2
=> 2

irb:002> 2 + 3
=> 5

irb:003> "Hello Strings"
=> "Hello Strings"

irb:004> "Bob is turning #{25 + 1}!"
=> "Bob is turning 26!"
```

_I strongly encourage you to try to do thoses things in your own IRB session._

What just happened?

1. We wrote the expression `2`, and aksed IRB to evaluate it. The result was `2`.
2. We wrote a more complex expression `2 + 3`, IRB evaluate it to `5`. Finally something useful is happening!
3. We wrote a expression using Ruby _syntax_ for writing _string litterals_, Ruby evaluate it.
4. This is a more advanced _syntax_ for _string interpolation_.

## Syntax & errors

When you wrote to the IRB prompt, you wrote a list of characters. This list is
decomposed by Ruby following certain syntaxic rules. This set of rules is
included in the [specification of the Ruby language][ruby-iso].

Sometime we write something that isn't part of Ruby's syntax. For instance, let's
write this: `3 "Hello"` to IRB:

```
irb:002> 3 hello
SyntaxError: (irb):2: syntax error, unexpected tSTRING_BEG, expecting end-of-input
3 "hello"
  ^
        from ...
```

IRB didn't respond to us with the result of the evaluation but with an error. An
error is decomposed like this:

1. the _class_ of the error: `SyntaxError`,
2. the _place_ this error just happened: the second line of an IRB session ; `(irb):2`,
3. the _message_ related to the error: `syntax error, unexpected tIDENTIFIER, ...`
4. an reminder of the exact place where something strange happened (optional).
5. the _backtrace_, starting with `from`. We'll talk more about backtraces later.

Basically what this error mean is that Ruby don't know how to read `3 "hello"`.
In this case, you'll probably have to fix what you wrote because for some reason,
it wasn't Ruby code.

You'll have a lot of errors, especially while you're discovering Ruby's syntax.
Try to fully read and understand them, it will be of a great help. When you face
an error that you don't understand, you should ask arround.

## Side effects

[ruby-iso]: TODO
