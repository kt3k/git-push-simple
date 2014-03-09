# git-push-simple

> `git push` with push.default == simple

One purpose of this command is to prevent [this kind of incident](https://news.ycombinator.com/item?id=6713742).

## Usage

Put the script `git-push-simple` anywhere in $PATH.

Then:

```
$ git push-simple
```

This perform the command like `git push upstream HEAD`.
