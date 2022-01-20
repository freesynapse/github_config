## Setup of githubs new crappy 2FA system

To make it work, I first followed the instructions on https://github.com/settings/tokens. Then, Git Credential Manager (installed from .deb -- [link](https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)). GPG and pass was used to store the authentication credentials ([GCM](https://github.com/GitCredentialManager/git-credential-manager/blob/main/docs/credstores.md)).


## To make git command line work:
I used git config --global push.default simple (to make 'git push' push main -> main). Then create an empty repository and copy the address.
```
git clone <URL>
git add .
git commit -m "message"
git push
```
These commands, in conjunction with the global settings for push.default, will push to main.


