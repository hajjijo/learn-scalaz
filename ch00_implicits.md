# The implications of implicit keyword in scala !
Scala syntax is very simple and straightforward, that is if we ignore the infamous `implicit` keyword ! This bad reputation comes from the fact that not only it's a little confusing, it is used in couple of different ways to perform different tasks. But we can summarize it in one simple concept: __Extending the language__. Let's face it step by step.

## implicit conversion
Since nothing beats the clarity of good code, let's start by an example:
```SCALA
implicit def jsStyleBoolean(a: Int): Boolean = a != 0
if (2) println("Ok!")
```

