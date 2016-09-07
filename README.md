# elm-location

This is a fork of [elm-community/elm-history](http://package.elm-lang.org/packages/elm-community/elm-history/latest),
specifically splitting out the `Location` module to make it independent and usable with Elm `0.17`.

## API

`location`: get the current location as a record that reflects the various parts of the URL.

`reload`: reload the current location

`assign`: change to a new location, pushing the previous location to history

`replace`: replace the current location with a new one.

**Note:** The difference between `assign` and `replace` is that `replace` removes the URL of the
current document from the history, meaning that it is not possible to use the `back` button
to navigate back to the original document.
