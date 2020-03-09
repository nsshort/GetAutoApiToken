# GetAutoApiToken
### 工具说明 ###
* 配合AutoApi/原教程使用的获取refresh_token工具，建议按原教程使用rclone获取，因为此工具使用起来实在有点麻烦！
  仅是为了rclone报错或者无PC端的朋友而适配的工具。
  
### 步骤 ###
* fork本仓库

![image](https://github.com/wangziyingwen/ImageHosting/blob/master/GetAutoApiToken/fork.png)

* 点击仓库Settings，往下拉找到 GitHub Pages，Source 栏选择 master branch，然后上面会出现一个网址（俗称项目主页），

![image](https://github.com/wangziyingwen/ImageHosting/blob/master/GetAutoApiToken/Settings.png)
![image](https://github.com/wangziyingwen/ImageHosting/blob/master/GetAutoApiToken/Gpage.png)

  点击网址看看能不能进去网页（显示未更新啥的）如图，进不去再等等，反应有点慢。然后复制项目主页网址
  
![image](https://github.com/wangziyingwen/ImageHosting/blob/master/GetAutoApiToken/未更新.png)

* 按原教程注册应用，重定向url选web，到这里的时候！！！内容填入 你的项目主页网址 ，不要填  http://localhost:53682/
 （跟原教程区别！！！！），最后点注册即可。
  
  接下来的按原教程操作，获取id、机密、赋予权限，直到需要用rclone。
  
* 接下来，修改你的GetAutoApiToken项目里的index.html文件
  修改内容如下：（只要修改文字，外面的单引号/双引号千万不要覆盖掉）
  
  * 修改地方1：（第5行）
  > 未更新   
  
  改为   
  
  > 已更新
  
  * 修改2（第10行最后面有2个）、修改3（第17行1个）、修改4（第20行1个）、修改5（第25行1个）
  > 把其中的文字改为相应内容（你的应用id、你的应用机密、你的项目主页）
  
  保存，紧接着
  
  * 修改6: 
  在AutoApi项目里的或者原教程项目里的1.py，中间部位有一个
  
  >'redirect_uri':'http://localhost:53682/'
  
  改为
  
  >redirect_uri':'你的项目主页'
  
* 保存刷新，打开你的项目主页网址，看看内容有没有更新。如果显示"已更新" ，点击get refresh_token

  会跳转到微软登陆页面，登陆完会跳出来一大段abcdefg啥的，在里面找refresh_token。
  
* 至此，refresh_token获取完毕

### 最后 ###
* 真的很烦，超级多步骤
