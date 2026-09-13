任务1
我用了claude code(连glm 5.1),安装配置过程是我先在powershell输入命令安装claude code，然后在官网下载cc-switch，在智谱官网注册后新建API key，让claude code连接上glm 5.1，充值，然后就可以使用了。

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

然后我让它修改本文件所在仓库中的readme，删除末尾的"assist",并上传到远端，AI找到了本地文件并删除，我在git diff中看到了修改，然后我让它提交并上传远端，我在git log中看到它Remove assist from end of README.md，Github上也确实看不到assist了，最终结果符合我的预期，就是速度比我预想的慢了一点。

任务2

1.AI Agent有调用来读写文件、执行命令等的工具的能力，普通聊天 AI 仅能处理用户在网页上上传的文本/图片等内容，没有本地系统访问权限。

2.Tool帮助AI操作电脑，AI通过调用这些Tool完成读文件、跑命令和搜网页等动作。

3.因为AI来到项目时可能不知道这个项目是干什么的、文件应该放在哪里、有什么开发规范、修改之后要不要测试和哪些东西不能乱动等规则，这份“员工手册”可以告诉AI项目规范，边界和禁忌，避免其胡乱操作。

4.因为和AI进行对话、Tool返回结果等都需要占用它的上下文，上下文窗口是有限的，所以旧内容科能会被挤出。Agent的额度一般按使用时输入输出总token消耗来计算，不过也有些模型额度按调用次数。

5.
