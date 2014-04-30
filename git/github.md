Put an existing project on GitHub
---------------------------------
* Create the repository on Github
* Attach local project to the Github repo:
```
        git remote add origin [url from Github]
```
* Configure merge in .git/config:
```
[branch "master"]
        remote = origin
        merge = refs/heads/master
```
* Do a pull to get README, etc.  
* Push master branch:
```
        git push origin master
```