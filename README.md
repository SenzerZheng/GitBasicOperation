**Command Line Instructions**
=================================== 

**Ⅰ．SSH keys** <br>
ssh -keygen -t rsa -C "888@qq.com <br>
*open C:\Users\pc\.ssh\id_rsa.pub* <br>
*copy the content and paste to the server places* <br>

**Ⅱ．Git global setup** <br>
git config --global user.name "SenZerZheng" <br>
git config --global user.email 888@qq.com <br>

***（Ⅰ）Create a new repository*** <br>
git clone git@192.168.1.1:SenZerZheng/Hello.git <br>
cd Hello <br>
touch README.md <br>
git add README.md <br>
git commit -m "add README" <br>
git push -u origin master <br>

***（Ⅱ）Existing folder or Git repository*** <br>
cd existing_folder <br>
git init <br>
git remote add origin git@192.168.1.1:SenZerZheng/Hello.git <br>
git add . <br>
git commit <br>
git push -u origin master <br>

**Ⅲ．Merge** <br>
***（Ⅰ）Merge from branch(develop) to trunk(master)*** <br>
git checkout master <br>
git merge develop *// merge from develop to master, the current code is master* <br>
 ![github](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_01.png "github") <br>
start . *// explore the app* <br>
or start app/.../network/HelloUrl 			*// explore the HelloUrl.java* <br>
![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_02.png) <br>
 
**Explain Image: delete the code between <<< to ===** <br>
 ![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_03.png) <br>
**Explain Image: result** <br>
 ![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_04.png) <br>
git commit –a / git commit <br>
  ![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_05.png) <br>
git push *// push the remote* <br>

***（Ⅱ）Merge from Hello.java to Hello.java in develop*** <br>
git status <br>
git add . <br>
git status <br>
git commit –a / git commit <br>
git pull <br>
start . / start app/.../network/HelloUrl 		<br>

**Explain Image: delete the code between <<< to ===** <br>
 ![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_06.png) <br>
**Explain Image: result** <br>
 ![image](https://github.com/SenzerZheng/GitBasicOperation/blob/master/samples/sample_07.png) <br>
git commit –a / git commit <br>
git push *// push the remote* <br>
