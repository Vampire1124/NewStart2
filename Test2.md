1. 在本地选个地方建个文件夹  F：/GitHub
2. 打开 Git Bash，或切换到这个文件夹，cd 切换到 GitHub 文件夹
3. git status 查看这个文件夹还不是一个仓库
4. git init   执行完这个文件夹就是一个仓库
5. 在 GitHub 文件夹中创建文件 Test2.md
6. git add Test2.md
7. git commit -m 'first commit' 进行提交
8. git remote add origin git@github.com:Vampire1124/NewStart2.git
   - 给本地的项目添加一个远程仓库，origin 是给这个远程仓库起的名字，名字可以随便起。大家公认只有一个远程仓库名字就是 origin。
9. git remote -v 查看当前项目有哪些远程仓库
10. git push origin master 向对应的远程仓库提交代码，而这个代码是在 master 分支上。也可以提交到指定分支。
    - 此处报错。操作是，在 github 上创建项目，然后本地 git init ,没有 git pull -f -all ,就 add ,commit ,push ,导致 github 上的 readme 文件和本地版本冲突。
    - 解决办法：git push  -u origin master -f
    - 一般我们在 push 之前，都先 pull ,这样不容易导致冲突