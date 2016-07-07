# Getting Started with ReasonML and BuckleScript

2016-07-01

## Installation

### Mac OS X

**Install the OCaml package manager:**

```
brew install opam
opam init
```

(Note: If you don't have `brew` installed yet, see [brew.sh](http://brew.sh/))

**Install an OCaml version modified for BuckleScript:**

```
opam pin add BetterErrors https://github.com/chenglou/BetterErrors.git
opam switch 4.02.3+buckle-1
eval `opam config env`
```

**Install the ReasonML syntax for OCaml:**

```
opam update
opam pin add -y merlin 'https://github.com/the-lambda-church/merlin.git#reason-0.0.1'
opam pin add -y merlin_extend 'https://github.com/let-def/merlin-extend.git#reason-0.0.1'
opam pin add -y reason 'https://github.com/facebook/reason.git#0.0.6'
```

**Install NodeJS:**

See http://blog.teamtreehouse.com/install-node-js-npm-mac

**Finally, create and run a Hello World app:**

```
mkdir helloreason && cd helloreason
echo "{}" > package.json
npm install --save bs-platform # <-- takes a while to compile
echo 'let _ = Js.log "hello bucklescript!"' > hello.re
`npm bin`/bsc -pp refmt -impl hello.re
node hello.js
```