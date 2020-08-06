---
date: 2020-08-06
tags:
  - git
---

# Using git amend

## Amending the last commit message

```
  git commit --amend
```
    
## Amending any other commit message

For example, if the commit message you want to modify is 4 commits back, then first REBASE your repository to the last 4 commit:

```
  git rebase -i HEAD~4
```

This will open up the commits in `$EDITOR`. Change the first word on the line which corresponds to the commit you want to modify from `pick` to `reword`.

Then modify the commit message as required.

Finally `git push --force` to send your amended commits upstream.

### Reference:

  - [https://www.w3docs.com/snippets/git/how-to-change-commit-message.html](https://www.w3docs.com/snippets/git/how-to-change-commit-message.html)
  - [https://gist.github.com/nepsilon/156387acf9e1e72d48fa35c4fabef0b4](https://gist.github.com/nepsilon/156387acf9e1e72d48fa35c4fabef0b4)