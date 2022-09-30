## Multiple remotes

### Setup multiple remotes

1. Create a bitbucket project
2. Create a github project
3. Add both remotes to your local project
```bash
git remote add bitbucket git@bitbucket.org:iolaru/test-multiple-remotes.git
git remote add github git@github.com:IonOlaru/test-multiple-remotes.git
```
4. Verify remotes
```bash
git remote -v
bitbucket	git@bitbucket.org:iolaru/test-multiple-remotes.git (fetch)
bitbucket	git@bitbucket.org:iolaru/test-multiple-remotes.git (push)
github	git@github.com:IonOlaru/test-multiple-remotes.git (fetch)
github	git@github.com:IonOlaru/test-multiple-remotes.git (push)
```
5. Commit some code 
```bash
echo | date >> ./text.txt
```
6. Commit all changes  
```bash
git add -A
git commit -m 'another random commit' 
```
7. Push the code into one of the remotes
```bash
git push bitbucket master
```
8. Sync remotes
```bash
./sync.sh
```

### Repeat 
Repeat steps `5-8` until you discover the meaning of life, or untill you can answer the question **Why are we here?**  
