# Bash aliases for copy&pasting into new environments:

```bash
alias gapa='git add --patch'
alias gaa='git add --all'
alias gcmsg='git commit -m'
alias gl='git pull'
alias gp='git push'
alias gss='git status -s'
alias gcb='git checkout -'
```

Für branch in prompt genau vor `\n` einfügen:
```bash
$(__git_ps1)
```
Und das folgende ausführen:
```bash
curl -L https://raw.github.com/git/git/master/contrib/completion/git-prompt.sh >> ~/.zshrc
```
