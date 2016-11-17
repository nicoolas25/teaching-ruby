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

``` ruby
irb:01> 2
=> 2

irb:02> 2 + 3
=> 5

irb:03> "Hello Strings"
=> "Hello Strings"

irb:04> "Bob is turning #{25 + 1}!"
=> "Bob is turning 26!"
```

_I strongly encourage you to try to do thoses things in your own IRB session._

What just happened?

1. We wrote the expression `2`, and aksed IRB to evaluate it. The result was `2`.
2. We wrote a more complex expression `2 + 3`, IRB evaluate it to `5`. Finally something useful is happening!
3. We wrote a expression using Ruby _syntax_ for writing _string litterals_, Ruby evaluate it.
4. This is a more advanced _syntax_ for _string interpolation_.



## Side effects
