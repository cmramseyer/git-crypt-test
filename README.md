## git-crypt

store secret (not risky) files: agents, skills, specs, todos, etc.


### install
```
sudo apt install git-crypt
```

### init
```
git-crypt init
```

### set rules
```
# .gitattributes

secretfile filter=git-crypt diff=git-crypt
*.key filter=git-crypt diff=git-crypt
secretdir/** filter=git-crypt diff=git-crypt
```

### export key
```
git-crypt export-key ~/path/to/my.key
```

