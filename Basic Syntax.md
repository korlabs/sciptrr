***THIS IS NOT YET COMPLETE. IF YOU HAVE ANY IDEAS, SUBMIT A PULL REQUEST!***



# Scriptrr Syntax Guide

***Scriptrr is distributed under License Creative Commons Attribution 4.0 International.***

Scriptrr's syntax is similar to Ruby on Rails and PHP, with a simplistic approach.

To signify the start of a Scriptrr block of code, you must call this function:

```
start.scriptrr
```

To end a block of Scriptrr code you must call:

```
end.scriptrr
```

Now that we know how to start and end a block of Scriptrr code, what can we put between these tags?


The equivalent to the print() function in PHP in Scriptrr is the show.text: function. Here's an example:

```
start.scriptrr
show.text:"Hello world!" # commonly code represents variables as plain letters, and for printing words you'd need quotes.
end.scriptrr```
```

This will display on the screen:

```
Hello world!
```

However, what good is a bit of text on your screen? I mean, sure it can teach people stuff but that's not as cool or useful as a link, or a button.

So let's make a link to http://example.com/ with Scriptrr.

First we start a block:

```
start.scriptrr
```

Then we need to show the user a link by calling the link function. Can you guess how to do this?

```
show.link:http://example.com/
```

Then end the block, so as not to cause errors.
So altogether, that's:

```
start.scriptrr
show.link:http://example.com/ #uris like these can be enclosed in () or in ""
end.scriptrr
```

Wow. Pretty easy, huh?

See, this will link a user to http://example.com/, but on the page it will show the URL to the users too. This can be great if you're listing a bunch of links, but what if you want a polished webpage, showing text in place of the URL?

Here's what you do:

```
start.scriptrr
show.text:Example Link
&
show.link:http://example.com/
end.scriptrr
```

It's really that easy. You don't use semicolons, complicated link schemes... you literally take the two and add them together.
Ditching the semicolon is nice, however, how does it know when to shift ideas?

```
start.scriptrr show.txt Example Link & show.link:http:/example.com/ end.scriptrr
```


***THIS IS NOT YET COMPLETE. IF YOU HAVE ANY IDEAS, SUBMIT A PULL REQUEST!***

> Thoughts...is this a visual language or intended to be an application language?
