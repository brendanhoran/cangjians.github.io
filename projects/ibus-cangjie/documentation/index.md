---
layout: default
title: IBus Cangjie documentation
name: projects
project: ibus-cangjie
pretty_project: IBus Cangjie
sub: doc
---

IBus Cangjie implements both the Cangjie and Quick input methods.

Please note that the screenshots on this page were all taken on GNOME 3.10. As
a result, things might look differently on your system.

## Available Characters

Cangjie and Quick are the two most widely used input methods in Hong Kong. In
addition, they are very rarely used in other regions.

As a result, our primary target audience for IBus Cangjie are Hong Kong
people.

This is the reason why, *by default*, IBus Cangjie will only let you type
characters which are common in Hong Kong.

This is especially important for Quick users, who would quickly be drowned
under thousands of results for each input code if we didn't filter the
characters available by default.

If you need additional characters, though, enable them in
[the settings](#additional-characters).

## Wildcards

Do you really know all the input codes for all the 70000+ Chinese characters?

No? Well don't worry, we thought about that.

Whenever you don't know the exact input code of a character, just try using a
wildcard.

For example, the Cangjie code for 你 is `onf`.

But if you only remember the beginning and end, just try typing `o*f`, and
we'll return it, along with 繁 (`okvif`), 煲 (`odf`) and all the characters
for which the code starts with an `o` and ends with an `f`.

## Halfwidth or Fullwidth Characters?

In written Chinese, some characters have both a **halfwidth** and a
**fullwidth** form. This is the case of *punctuation* and *numbers*, for
example.

We try to strive for correctness, and as a result, IBus Cangjie will input
fullwidth characters by default.

However, many people prefer to use halfwidth characters, and some people will
even want to switch regularly from one to the other, depending on whether they
are chatting with a friend, or typing a formal document.

IBus Cangjie provides a convenient option which can be changed easily while
typing, without having to go all the way to [the preferences](#preferences).

![Switching between halfwidth and fullwidth characters](/images/ibus-cangjie-half-full-property.png "Switching between halfwidth and fullwidth characters")

## <a name="preferences"></a> Preferences

IBus Cangjie comes with its preference dialog. Or rather it comes with two:
one for Cangjie, and one for Quick.

Below is a screenshot of the Cangjie preferences. The Quick dialog is
absolutely identical.

![Cangjie Preferences](/images/ibus-cangjie-preferences.png "Cangjie Preferences")

### Input Method Version

The first option is to set the **version** of the input method.

IBus Cangjie supports two versions:

* *version 3*, the most widely used, and the default one on Microsoft Windows;
* *version 5*, the newer and better one, but used less commonly.

If you don't know which version you normally use, then stay with the default.

### <a name="additional-characters"></a> Additional Characters

As mentioned previously, IBus Cangjie is primarily intended to Hong Kong
people, and as such it only lets you type the characters which are important
in the SAR by default.

But we know that some people will need to input other characters. That's why
we added those options, so that Taiwan people and scholars studying ancient
Chinese can type all those rare characters they need.

The *Zhuyin / Bopomofo* option allows you to input the characters from
Taiwan's phonetic alphabet.

The *Japanese* option will, unsurprisingly, allow you to type characters from
the 3 Japanese alphabets: Kanji, Katakana and Hiragana.

The *Rare Chinese characters* option will enable **all** Chinese characters,
in addition to the ones which can be inputted by default. That means
Simplified Chinese characters which aren't used commonly in Hong Kong, ancient
Chinese characters which have fallen into disuse, etc. Note that the term
"rare" here is to understand in the context of Hong Kong people: a frequent
character in Mainland China might be very rare in Hong Kong!

Finally, the *Symbols* option will let you type miscellaneous symbols, like
→ or ㈤. Very few people will want to enable this option, but it is there if
you ever need it.
