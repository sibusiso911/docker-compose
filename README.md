### Open Terminal on linux🐧/macOS🍏
##### Ensure you have an SSH Key Set Up

##### First Check if your Already have an SSH Key:
```
ls ~/.ssh/id_rsa.pub
```
##### If not generate one:
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

##### View public key & Copy it :
```
cat ~./ssh/"name.pub"
```

##### Create a folder where you want to clone your Repository
```
git clone git@github.com:username/repository.git
```
### 🗔Windows (Git Bash or PowerShell):
-Open Git Bash
-Generate a new SSH Key 
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
#### Start the ssh-agent and add your key
```
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_ed25519
```
#### Copy your public key 

```
clip < ~/.ssh/id_ed25519.pub
```


### Test the Connection 
```
ssh -T git@github.com
```

### ADD the key to GitHub
-Go to GitHub → Settings → SSH and GPG keys

-Click "New SSH Key"

-Paste your public key

-Give it a title (e.g., “My SSH KEY”)

-Click "Add SSH Key"



