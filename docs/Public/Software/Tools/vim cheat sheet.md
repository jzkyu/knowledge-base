[site](https://vim.rtorr.com/)
### Motion

`w` - jump forwards to start of word
`e` - jump forwards to end of word
`b` - jump backwards to start of word
`ge` - jump backwards to end of word

`0` - jump to the start of the line
`$` - jump to the end of the line

`10j` - jump down 10 lines

`{ / }` - jump to prev / next paragraph
### Command

`fx` - jump to next occurrence of `x` (including numbers)
`Fx` - jump to prev occurrence of `x`
`;` - repeat prev movement
`,` - repeat prev movement, backwards

`zz` - center cursor on screen

`u` - undo

`:%s/x/y/g`: Replace every instance of `x` with `y`

`:wq`: Exit and save
### Visual

`b` - select everything in a block

`vi"` - jumps to and highlights next instance of `"`

`v/foo` - select from curr pos to next instance of `foo`

### Exiting

`:w` - write file (save)

`:q` - quit (must save changes first)

``