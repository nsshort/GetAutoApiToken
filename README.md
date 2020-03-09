# GetAutoApiToken
### 工具说明 ###
* 配合AutoApi/原教程使用的获取refresh_token工具，建议按原教程使用rclone获取，因为此工具使用起来实在有点麻烦！
  仅是为了rclone报错或者无PC端的朋友而适配的工具。
  
### 步骤 ###
* fork本仓库
* 点击仓库Settings，往下拉找到 GitHub Pages，Source 栏选择 master branch，然后上面会出现一个网址（俗称项目主页），

  点击网址看看能不能进去网页（未更新）如图，进不去再等等，反应有点慢。然后复制项目主页网址

* 首先去https://portal.azure.com/#home 注册一个应用,这一步网上的教程实在是太多了,我就不详细写了,大致写一下流程

  先用e5管理员账号登录网站,然后在主页找到Azure Active Directory点进去，
  
  再在左侧目录找到点击应用注册，再点上方的新注册就会跳出一个新建应用的界面，
  
  应用名字随意填写,然后选择任何组织目录(任何 Azure AD 目录 - 多租户)中的帐户，
  
  重定向url选web，填入 ## 第二步项目主页网址 ##，最后点注册即可。

* 
