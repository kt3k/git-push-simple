# git-push-simple

> `git push` with push.default == simple

One purpose of this command is to prevent [this kind of incident](https://news.ycombinator.com/item?id=6713742).

## Usage

Put the script `git-push-simple` anywhere in your $PATH.

Then:

```
$ git push-simple
```

This performs the command like `git push origin HEAD` if the upstream's branch name is the same as the current branch. This behaviour is the same as `git push` without parameter with `push.default` set to `simple`. (This configuration will be default in Git 2.0).

## :cd: Install

```sh
# Downdloads script
curl https://raw.githubusercontent.com/kt3k/git-push-simple/master/git-push-simple -o git-push-simple

# Make it executable
chmod 755 git-push-simple

# Move it somewhere in $PATH
sudo mv git-push-simple /usr/local/bin/
```

## License

MIT
