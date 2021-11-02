>GIT => Setting => Dev setting => Personal access token => gen new token
rep. => generate token

### copy

```
"Any_token"
```

## config account
```bash
git config --global user.name ""
git config --global user.email ""
```
## list configered userNames
```bash
git config -l
```
## clone any repo
```bash
git clone repo name
```

## don't need to enter username and token again and again.

```bash
git config --global credential.helper.cache
git pull 
#userName 
#token
```
