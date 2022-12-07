# PicGo + GitHub to build a personal picture bed tool

## 1. GitHub repository settings

> 流程：新建 public 仓库 -> 创建 token -> 复制 token 备用

### 1.1 New repository

点击 git 主页右上角的 `+` 创建 `New repository`；

填写仓库信息，例如我就创建了一个 `MyNotesImg` 的仓库。这里注意，仓库得设置为 `Public` 因为后面通过客户端访问算是外部访问，因此无法访问 `Private` ，这样的话图片传上来之后只能存储不能显示。所以要设置为 `Public`。

![Create_repository](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/Create_repository(2022-12-07-20-35-27).png)

### 1.2  Create token and copy and save

此时仓库已经建立，点击右上角头像，然后进入设置；

![Settings](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/Settings(2022-12-07-20-36-59).png)

在页面最下找到 `Developer settings`，点击进入；

![Developer_settrings](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/Developer_settrings(2022-12-07-20-37-46).png)

创建 token；

![create_new_token](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/create_new_token(2022-12-07-20-39-39).png)

填写 Note，设置 Expiration，勾选复选框 repo ，接着到页面底部 `Generate token` 就完成了；

![token_settings](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/token_settings(2022-12-07-20-40-12).png)

然后复制生成一串字符 token，这个 token 只出现一次，所以要保存一下

![token](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/token(2022-12-07-20-42-01).png)

## 2. PicGo client configuration

### 2.1 Download & install

PicGo git地址：[PicGo](https://github.com/Molunerfinn/PicGo)

### 2.2 configuration

![PicGo_Github_setting](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/PicGo_Github_setting(2022-12-07-20-44-56).png)

- 仓库名 即你的仓库名
- 分支名 默认 master
- Token 就是刚刚复制的那一串字符
- 存储路径 这个可以填也可以不填，填了的话图片就上传到 git 中 data 这个文件夹
- 域名 

 然后点确定就可以了。

然后关于上传的快捷键设置。默认的是 Mac 按键，推荐改成 `Ctrl + alt +c`（当然也可以不改）。

![PicGo_hot_key](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/PicGo_hot_key(2022-12-07-20-49-26).png)

### 2.3 PicGo rename plugin

![rename_plugin](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/rename_plugin(2022-12-07-20-52-35).png)

我的插件重命名格式

![my_plugin_config](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/my_plugin_config(2022-12-07-20-53-25).png)

具体设置课参考 [picgo-plugin-rename-file](https://github.com/liuwave/picgo-plugin-rename-file#readme)

## 3. My picgo settings

Details can be found at [data.json](https://github.com/MrZhuA00/build-picture-bed-tool/blob/main/data.json) 

## 4. Typora uses PicGo to upload pictures

> 偏好设置 -> 图像 ->  上传服务设定   上传服务选择 "PicGo(app)"，选择 PicGo 安装路径

![typora_setting](https://raw.githubusercontent.com/MrZhuA00/NotesImg/main/Images/typora_setting(2022-12-07-21-15-49).png)