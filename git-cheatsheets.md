# Git cheatsheet

## Delete file

To stage deleted file after deleting it

`git rm <filename>`

To stage deleted file without deleting it

`git rm --cached <filename>`

## Overwrite pushed commit

To overwrite pushed commit, amend and push using `--force-with-lease`.

`--force-with-lease` fails when local ref does not match with remote ref,
so making sure it doesnot overwrite someone else's changes.

```bash
git amend
git push --force-with-lease origin <branch-name>
```

