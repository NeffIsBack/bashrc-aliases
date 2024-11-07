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
sudo apt install bat -y
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

For displaying branches put this exactly before `\n` in the zshrc file:
```bash
$(__git_ps1)
```
And execute the following for git completion:
```bash
curl -L https://raw.github.com/git/git/master/contrib/completion/git-prompt.sh >> ~/.zshrc
```
