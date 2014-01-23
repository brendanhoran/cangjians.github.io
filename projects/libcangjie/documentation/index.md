---
layout: default
title: libcangjie documentation
name: projects
project: libcangjie
sub: doc
---

libcangjie is a very simple library:

* there is only one header to include: `cangjie.h`
* everything happens by instantiating a `Cangjie` context, and then passing it
  to the various functions of the API.

These pages will document proper use of libcangjie. Although the interesting
part is the last of the list, we recommend you read them in order:

1. the possible [error codes](errors.html)
2. the supported [Cangjie versions](versions.html)
3. the [available output filters](filters.html)
4. the [`CangjieChar` structure](cangjiechar.html)
5. the [`CangjieCharList` character lists](cangjiecharlist.html)
6. the [`Cangjie` context](cangjie.html)

libcangjie also comes with a command-line tool, which can be seen as an
example of how to use the API, and is useful for testing/debugging purpose:
`libcangjie_cli`. Read [its documentation](cli.html) for details on how to use
it.
