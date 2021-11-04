# Now We Know Julia

## Shortcuts 
; shell REPL
] package manager
? interactive help

rand([0, 1], 4)

If we square the norm, it's a sum of squares of the members...

### Language Features
- multi-paradigm (procedural, functiona, object-oriented)
- multiple dispatch (runtime method overloading, since overloading is compile time)

### REPL Modes
- From julia repl, do `?` to enter help mode.
- From julia repl, do `]` to enter the package manager mode
- From julia repl, do `;`, to enter shell mode
- See https://docs.julialang.org/en/v1/stdlib/REPL/index.html for more modes


### Prompt Pasting Feature
Julia features "prompt pasting". Try it out. Copy and paste the following block into the Julia repl. It will run! Super neat!

```
julia> using Dates 
 
julia> Dates.now() 
2018-09-02T21:13:03.122 
julia> ans 
2018-09-02T21:13:03.122 
```

### Tab completion
`pri` followed by tab will show functions that start with `pri`
`\pi` followed by tab will generate `π`
`\` followed by tab shows all of the special character options, so we have LaTeX autocomplete, too


### Built-In Functions
- typeof returns the type
- methods (tells us about the multiple dispatch setups)
- print vs println

### Time operations with the Time Macro
```
@time begin
	whatever code or expressions
end
```

### Collection Mutation 	Methods
push!
append!
sizehint!
empty!
