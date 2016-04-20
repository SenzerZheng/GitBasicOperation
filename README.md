 - **Command line instructions**

**一．SSH keys** <br>
ssh -keygen -t rsa -C "888@qq.com <br>
*open C:\Users\pc\.ssh\id_rsa.pub* <br>
*copy the content and paste to the server places* <br>

**二．Git global setup** <br>
git config --global user.name "smileisgood" <br>
git config --global user.email 888@qq.com <br>

***（一）Create a new repository*** <br>
git clone git@192.168.1.1:smilesigood/Hello.git <br>
cd Hello <br>
touch README.md <br>
git add README.md <br>
git commit -m "add README" <br>
git push -u origin master <br>

***（二）Existing folder or Git repository*** <br>
cd existing_folder <br>
git init <br>
git remote add origin git@192.168.1.1:smilesigood/Hello.git <br>
git add . <br>
git commit <br>
git push -u origin master <br>

**三．Merge** <br>
***（一）Merge from branch(develop) to trunk(master)*** <br>
git checkout master <br>
git merge develop *// merge from develop to master, the current code is master* <br>
 
start . *// explore the app* <br>
or start app/.../network/HelloUrl 			*// explore the HttpUrl.java* <br>
 
**Explain Image: delete the code between <<< to ===** <br>
 
**Explain Image: result** <br>
 
git commit –a / git commit <br>
  
git push *// push the remote* <br>

**（二）Merge from Hello.java to Hello.java in develop** <br>
git status <br>
git add . <br>
git status <br>
git commit –a / git commit <br>
git pull <br>
start . / start app/.../network/HelloUrl 		<br>

**Explain Image: delete the code between <<< to ===** <br>
 
**Explain Image: result** <br>
 
git commit –a / git commit <br>
git push *// push the remote* <br>
