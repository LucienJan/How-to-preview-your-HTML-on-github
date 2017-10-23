### 开始之前的准备工作
1.需要你自己写的网页文件  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/1.png)  
2.注册Github  
3.下载安装git。[下载地址](https://git-scm.com/downloads)

### 教程开始  
<strong style="color:blue;">步骤一:</strong>
登录到Github上，新建一个repo，命名为test，勾选 initialize this repository with a README，点击create repository。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/2.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/3.png)  
<br />
<strong style="color:blue;">步骤二:</strong>
打开settings，有一个Github Pages 的设置，点击 source 中的本来的 None ，使其变成 master 分支，也就是作为部署github pages 的分支，然后点击 save。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/4.png)  
<br />
<strong style="color:blue;">步骤三:</strong>
页面刷新之后，再看 github pages 设置框处，多了一行网址，就是你的 github pages 的网址了。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/5.png)  
点击这个链接  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/6.png)  
哇塞！一个test。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/7.jpg)  
好了，别激动了，真正让一个小白你发疯的阶段开始了，有了自己的网址，但页面显示是什么鬼？  
至此以上，github上要处理的操作告一段落，该上Git了！  
<br />
<strong style="color:blue;">步骤四:</strong>
打开此电脑，选择一个盘，比如F盘，右键空白处点击 git bash here。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/8.png)  
<br />
<strong style="color:blue;">步骤五:</strong>
输入如下命令，用来在 f 盘创建 test 文件放你的github上的test repository，克隆test repository到 test 文件中。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/9.png)  
这个时候你的 f 盘，就会多一个 test 文件，打开它，  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/10.png)  
会看到一个 README.md 的文件，这个文件是从哪来的呢？追溯到gihub上，你会发现 README 文件是来自 master 分支。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/11.jpg)  
<br />
<strong style="color:blue;">步骤六:</strong>
将自己的网页文件复制粘贴至 F 盘的 test 文件中  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/12.png)  
<br />
<strong style="color:blue;">步骤七:</strong>
执行如下命令  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/13.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/14.png)  
解释一下上面的命令：首先输入  git status   列出当前目录所有还没有被git管理的文件和被git管理且被修改但还未提交(git commit)的文件，也就是所有改动文件，红色字体标出。  
然后输入 git add .  (有个点) 表示添加当前目录下的所有文件和子目录，  
然后 再输入一次 git status 如果看见文件都变绿了 ，那么就代表 它们已经准备好了被提交（git commit）。
<br />
<strong style="color:blue;">步骤八:</strong>
输入如下命令，将你的文件上传至远程 master 分支  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/15.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/16.png)  
输入最后一行 git push，按回车，等一会，会有弹出框让你输入你的 github 账号和密码。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/17.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/18.png)  
ok之后耐心等待。  
当出现像下图中的语句之后，你已经完成了99%。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/19.png)  
<br />
<strong style="color:blue;">最后一步:</strong>
打开浏览器输入给你的网址加上你上传的 html 文件名 test.html，然后重重的按下回车。  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/20.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/21.png)  
![](https://github.com/LucienJan/How-to-preview-your-HTML-on-github/raw/master/images/22.png)
恭喜你，成功了！！！哦不，还差一步，不follow一下我？不fork一下文章？
<br />

附录一：常用git命令  
$ git clone		//本地如果无远程代码，先做这步，不然就忽略  
$ cd			//定位到你blog的目录下  
$ git status	//查看本地自己修改了多少文件  
$ git add .		//添加远程不存在的git文件  
$ git commit -m "what I want told to someone" //提交修改  
$ git push		//更新到远程服务器上  
$ git rm		//移除文件  
<br />

附录二：如何修改你的网页？
1.在github上的master分支中直接进行修改。（如果不添加新的文件推荐此法）  
2.在github客户端进行修改在同步。（如果添加了新的文集推荐此法）  




<sub>参考地址：
<a target="_blank" href="http://www.cnblogs.com/lijiayi/p/githubpages.html">http://www.cnblogs.com/lijiayi/p/githubpages.html</a>
</sub>
