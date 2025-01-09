__Guide to Using RegEx__

<h1><b>Periods .</b></h1>

Periods are like a wildstar but only for that specific character, for example 
searching for Apple you could do:

```Bash
cat RegexLearn.txt | grep "App.e"
```

This will return Apple

<h1><b>Caret ^</b></h1>

Carets are used to match the beginning of the stream, for example you could use

```Bash
cat RegexLearn.txt | grep "^B"
```

This will return 7 Different items that begin with B

<h1><b>Dolla Sign $</b></h1>

Doller signs are the same as Carets except it matches the end instead of the 
beginning for example you could search for every item that ends in e with:

```Bash
cat RegexLearn.txt | grep "e$"
```

This will return every item that ends with e

<h1><b>Asterick's Lol *</b></h1>

Astericks are wildstars and will find any item (mainly used to find inbetween text)
For example you could use:

```Bash
cat RegexLearn.txt | grep "A*le"
```

This with find Apple, Custard Apple, Pineapple ETC.

<h1><b>Backslash \ </b></h1>

This will search for special symbols, for example using \ will show every item 
with a space, for example:

```Bash
cat RegexLearn.txt | grep "\"
```

This will return multiple items with spaces

<h1><b>Parenthesis ()</b></h1>

Parenthesis are used to match a group of regex's, for example

```Bash
cat RegexLearn.txt | grep -E "(fruit)"
```

This will return every item that has the word fruit in it.

<h1><b>Question Mark ?</b><h1>

The question mark is used to match anything that has the exact words in it, for
example:

```Bash
cat RegexLearn.txt | grep -E "Ch?"
```

This will show every item that has Ch in it.
