
Detailed notes on experience https://stormasm.github.io/spec17

* Here is the **[spec-md](https://github.com/leebyron/spec-md)** repository.

So everything is intact from the
[spec-md repo](https://github.com/leebyron/spec-md)
and all I did was fork the repo
add a command to build my own personal blog / spec.

Initially out of the box when you run

```
yarn
```

the original spec17.md gets built...
Then if you want to modify or change your spec17.md simply run the command

```
npm run start
```

whose **start** tag is documented in package.json explaining exactly what it does.

Then you can push the changes in the out directory into the branch **gh-pages**.

## Nodemon

Run this command in one window...

```
alias npw='npm run watch'

"watch": "nodemon --exec './bin/spec-md -m spec/metadata.json > out/index.html' spec17.md"
```

Run this command in the other window

```
alias shs='/usr/bin/python -m SimpleHTTPServer 3000'

shs
```
