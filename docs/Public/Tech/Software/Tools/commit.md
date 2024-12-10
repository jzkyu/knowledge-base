A *commit* is a [[command]] in [[git]] that takes a snapshot of all your changes in your directory.

It is good to follow conventions for writing *commits*, for readability and generating changelogs ([[changelog]]). [^1]

`<type>[optional scope]: <description`

- `feat`: (new feature for the user, not a new feature for build script)
- `fix`: (bug fix for the user, not a fix to a build script)
- `docs`: (changes to the documentation)
- `style`: (formatting, missing semi colons, etc; no production code change)
- `refactor`: (refactoring production code, eg. renaming a variable)
- `test`: (adding missing tests, refactoring tests; no production code change)
- `chore`: (updating grunt tasks etc; no production code change)

[^1]: https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716