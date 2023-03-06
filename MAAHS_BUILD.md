# Building the Maahs Version of Go-Jira

- Sync the `main` branch of cmaahs/jira with the upstream

```zsh
# change to the cmaahs/jira repository directory
git checkout main
git fetch; git status; git pull
git checkout maahs
git merge main
# resolve conflicts & add
git push origin maahs
```

## Build

```zsh
git checkout maahs
make build 
./jira
cp ./jira ~/tbin
```

