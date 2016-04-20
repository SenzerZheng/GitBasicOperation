 - **Command line instructions**

**一．SSH keys**
ssh -keygen -t rsa -C "888@qq.com
*open C:\Users\pc\.ssh\id_rsa.pub*
*copy the content and paste to the server places*

**二．Git global setup**
git config --global user.name "smileisgood"
git config --global user.email 888@qq.com

***（一）Create a new repository***
git clone git@192.168.1.1:smilesigood/Hello.git
cd Hello
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

***（二）Existing folder or Git repository***
cd existing_folder
git init
git remote add origin git@192.168.1.1:smilesigood/Hello.git
git add .
git commit
git push -u origin master

**三．Merge**
***（一）Merge from branch(develop) to trunk(master)***
git checkout master
git merge develop *// merge from develop to master, the current code is master*
 
start . *// explore the app*
or start app/.../network/HelloUrl 			*// explore the HttpUrl.java*
 
**Explain Image: delete the code between <<< to ===**
 
**Explain Image: result**
 
git commit –a / git commit
  
git push *// push the remote*

**（二）Merge from Hello.java to Hello.java in develop**
git status
git add .
git status
git commit –a / git commit
git pull
start . / start app/.../network/HelloUrl 			
 
**Explain Image: delete the code between <<< to ===**
 
**Explain Image: result**
 
git commit –a / git commit
git push *// push the remote*
