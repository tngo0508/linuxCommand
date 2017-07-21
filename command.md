### setup time in utc
`timedatectl set-timezone UTC`
### Git on the server
```sh
 $ mkdir project.git
 $ cd project.git
 $ git init
```
### Git on the client
```sh
 $ cd local_project
 $ git init
 $ git add .
 $ git commit -m 'message'
 $ git remote add origin git@gitserver:/srv/git/project.git
 ```
 #### Git for pushing
 `$ git push origin master`
 #### Git for download
 `$ git clone git@gitserver:/srv/git/project.git`
 #### Git auto-completion
 ```
 $ curl -OL https://github.com/git/git/raw/master/contrib/completion/git-completion.bash
 $ mv ~/git-completion.bash ~/.git-completion.bash
 ```
 Go to .bashrc or .bash_profile and add following codes
 ```bash
 if [ -f ~/.git-completion.bash ]; then
    source ~/.git-completion.bash
 if
 ```
 #### Vim find and replace patterns/words across mutiple files
 
  All *.cpp files in current directory.
 `:arg *.cpp` 	
 
  And all *.h files.
  
`:argadd *.h` 	

  Optional: Display the current arglist.
  
 `:arg`
 
  Search and replace in all files in arglist.
  
 `:argdo %s/pattern/replace/ge | update`
 
