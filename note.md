任务1
我用了claude code(连glm 5.1),安装配置过程是我先在powershell输入命令安装claude code，然后在官网下载cc-switch，在智谱官网注册后新建API key，让claude code连接上glm 5.1，然后就可以使用了。

我先让cc阅读我之前的git 仓库，它的回答大致如下：
README.md 内容要点

  README 中记录了作者学习 Git 的完整过程和笔记，涵盖以下知识点：

  1. 仓库建立 — git init  
  2. 加入版本库 — git add + git commit -m ""  
  3. 查看状态 — git status（红色=未跟踪，绿色=暂存，消失=已提交）  
  4. 查看历史 — git log / git log --pretty=oneline  
  5. 查看修改 — git diff / git diff HEAD -- 文件  
  6. 版本回退 — git reset --hard HEAD~n / 通过版本号回退  
  7. 撤销修改 — git restore / git restore --staged  
  8. 同步到 GitHub — git remote add origin + git push -u origin main  

然后我让它修改本文件所在仓库中的readme，删除"qwerty",
