1. Find the folder you wish to operate as a repository  

2. git init   - initialize the folder in order to make it into a git repository  

3. Go to github.com and create your github account or simply sign into your github existing account, create corresponding github repository   

4. Get back to your local folder and generate ssh access by ssh-keygen so you can bypass the username and passwd and sign into your github account easily and safely   

5. ssh-keygen -t rsa -C "michaelxuan@hotmail.com"   

6. Go ~/.ssh/id_rsa.pub find the generated ssh pub-key and copy it then paste it on the github account ssh
  setting section  

7. git remote add xxx git@github.com:username/git_name.git    

  ##TWO THINGS:   

  __a__. xxx means the alias of git@github.com:username/git_name.git, so when you push you can simply type git push -u xxx master instead of the while url    

  __b__. git_name is the corresponding git repository name   

8. git add file_you_wish_to_push    -  

9. git commit -m "msg"   -  decide what to push and create a log message    

10. git push -u xxx master  