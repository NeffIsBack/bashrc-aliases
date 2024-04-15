# Bash aliases for copy&pasting into new environments:
All-in-one solution:
```bash
echo 'alias gapa="git add --patch"
alias gaa="git add --all"
alias gcmsg="git commit -m"
alias gl="git pull"
alias gp="git push"
alias gss="git status -s"
alias gcb="git checkout - "' >> ~/.zshrc
curl -L https://raw.github.com/git/git/master/contrib/completion/git-prompt.sh >> ~/.zshrc
sed -i 's/\\n└─/ \$\(__git_ps1\)\\n└─/g' ~/.zshrc
#  Install and link bat to cat
sudo apt install bat
sudo ln -s /usr/bin/batcat /usr/local/bin/cat
```

Git aliases:
```bash
alias gapa="git add --patch"
alias gaa="git add --all"
alias gcmsg="git commit -m"
alias gl="git pull"
alias gp="git push"
alias gss="git status -s"
alias gcb="git checkout - "
```

Für branch in prompt genau vor `\n` einfügen:
```bash
$(__git_ps1)
```
Und das folgende ausführen:
```bash
curl -L https://raw.github.com/git/git/master/contrib/completion/git-prompt.sh >> ~/.zshrc
```
