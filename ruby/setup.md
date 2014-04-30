Installing RVM
---------------
Use RVM to manage versions of Ruby and Gemsets.

```
\curl -L https://get.rvm.io | bash -s stable
source .bashrc
source .bash_profile
```

If the line: 
```[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm"```
is in .bash_profile, move it to .bashrc.  Otherwise gems won't be found 
when you open a new terminal, unless you source .bash_profile.


Install a Version of Ruby
-------------------------
```rvm install 1.9.3```

Create a Gemset
---------------
Create a Gemset called mygems and make it the default:
```
rvm use 1.9.3@mygems --create --default
```