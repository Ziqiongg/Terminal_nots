# Command Line

#### 1.pwd

pwd        show your current directory, this is where you are.

if you cannot remember the file name or directory name, use tab 

#### 2. ls(list)

ls             -- （list）列出当前文件夹下所有文件以及文件夹

ls -l         all extra information about these directory 

ls -a         shows more hiden files, some of these files opening with dot, which means those are unable to search using normal way 

ls -al      combine both ls-l and ls-a

#### 3. cd(change)

cd         --back to the home directory  cd ~ 也有同效果

cd Downloads                                  -- 切换到下载文件夹

cd ..                                            -- 返回上一级文件夹 （..代表上一级）

cd documents/lovemaofolder/lovemaofile

cd ～/balabala         去到任意文件夹

#### 4. mkdir(create new directory)

mkdir                 - (create a new directory) 新建文件夹

mkdir name         新建一个name为名的文件夹

#### 5. touch(create new file)

touch file_name.txt              create a txt file 

touch file_name                    without file extention is ok

using mkdir and touch, you can create many files or directory one time 

Eg.  tough file1 file2

open file_name            open this file 

open -a Atom file_name.txt         using Atom to open this file

code file-name              use Visual Studio App to open it 

#### 6. mv(move)

mv my_picture.png pictures                     move the png file to the picture floder

mv another_file another_file.xlsx                 if the second part(folder part) doesn't exist, you will rename the first part, which is rename another_file as another_file.xlsx

#### 7. rm

| rm -i [file] | Remove with confirmation           |
| ------------ | ---------------------------------- |
| rm -r [dir]  | Remove a directory and contents    |
| rm -f [file] | Force removal without confirmation |

尽量少用吧 容易彻底删除

#### 8. cp(copy)

| cp [file] [newfile] | Copy file to file      |
| ------------------- | ---------------------- |
| cp [file] [dir]     | Copy file to directory |



在terminal里移动光标， 按住option然后点你想去的位置

control+A 光标回到这一行的最开始

control+E 光标回到这一行的最结尾

control + U 删掉这一整行

直接点上下箭头可以回到上一指令或下一指令



# Git

#### 1. git clone

git clone https://github.com/Ziqiongg/The-Turtle-Crossing-Project.git

链接是选code- clone-ssh

复制远程github代码到本地，（此步会生成一个文件夹）

而且git clone 自动将本地repo与远程github repo 连接起来

你在该文件夹中所做的修改 才对应着相对的远程 repo

#### 2. git init

git init : 在本地创建一个本地repo 

用此方法新建repo时 创建完之后， 需要 自己将 本地 与远程repo连接起来 

git remote add origin https://github.com/Ziqiongg/The-Turtle-Crossing-Project.git 

**以上两点为初次建立repository时使用**

#### 3. git fetch

git fetch : 更新本地repo使其与远程repo同步 (而不会对本地代码做任何修改)

我老师强调这一步很关键，每一次休息后首先来个git fetch

#### 4. git pull

git pull : 将远程代码复制到本地 （此步会修改本地代码，而且容易产生冲突conflicts）

#### 5.git status

git status : 检查并提示你当前本地代码与本地repo的区别 （是否增加或修改或删除files）

#### 6. git add

git add file.py : 添加**某个**文件以备后续通过commit来更新本地repo （注意仅此步不会做任何修改，须通过7.进一步更新）

git add .   这样会将当前所有修改全部一次性添加

#### 7. git commit

git commit -m "message" : 此步与6.结合起来，将6.中添加过的文件全部更新到本地repo中 （message里写一些便于队友理解的信息，解释你这次commit主要干了什么）

eg.    git commit -m "fixed qiongqiong cant eat maomao bug"

#### 8. git push

git push : 将本地repo上传到远程repo中，这样你的队友才能看到你的commit以及你做的修改。

#### 9. git log

就检查一下一共多少条commit，刚刚那条commit有没有传上去，看完之后点q 就能回到之前的界面（会显示所有的commit）







### 

先用2 创建新的本地repo

让你的电脑和本地连接，记住你的id//

npx git-setup              Press enter 

测试链接是否成功         ssh git@github.com     // 

在GitHub上创建新的repo， get ssh，让他们链接起来

git remote add origin git@github.comsshaddressxxxx

git push origin main



![截屏2022-04-18 00.20.19](/Users/ziqidoc/Documents/截屏2022-04-18 00.20.19.png)



