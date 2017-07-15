### setup time in utc
`timedatectl set-timezone UTC`
### Git on the server 
`$ mkdir project.git
 $ cd project.git
 $ git init`
### Git on the client
`$ cd local_project
 $ git init
 $ git add .
 $ git commit -m 'message'
 $ git remote add origin git@gitserver:/srv/git/project.git`
 #### Git for pushing
 `$ git push origin master`
 #### Git for download
 `$ git clone git@gitserver:/srv/git/project.git`
