### 背景
学习flask,进一步熟悉py3.7, <br>
博客可以用来整理记录一些日常技术笔记 <br>
### 个人博客系统

环境:Ubuntu18.04 <br>
框架语言: flask1.1.2+bootstrap4+python3.7+nginx1.14+gunicorn <br>
功能:
1 游客用户只能查看文章后评论以及点赞/踩 <br>
2 admin用户 评论回复,删除,修改,点赞/踩;文章发布,修改,删除 <br>
3 文章,评论分页<br>
4 admin用户登录认证<br>
### 环境变量
vi ~/.bashrc <br> 
export PYTHONPATH="your project root path" <br>
export PATH=$PYTHONPATH:$PATH <br>

### nginx 安装
sudo apt-get install nginx

### 依赖安装(虚拟环境pip)

pip install -r requirements.txt

### nginx 配置文件
touch /etc/nginx/site_enabled/aweblog.conf

### 生成虚拟数据(虚拟环境下执行)
flask gen-fake-data --cn 10
###  启停脚本
cd Flask_bird/bin <br>
停: stop.sh <br>
启: start.sh <br>

### admin 账号
username:admin   <br>
password:admin123 <br>

### 项目展示
评论列表<br>
![comments.png](https://github.com/Astrivemanlw/Blog/blob/master/comments.png)  <br>
文章编辑<br>
![edit_post.png](https://github.com/Astrivemanlw/Blog/blob/master/edit_post.png) <br>
主页<br>
![home.png](https://github.com/Astrivemanlw/Blog/blob/master/home.png) <br>
登陆界面<br>
![login.png](https://github.com/Astrivemanlw/Blog/blob/master/login.png) <br>
文章管理<br>
![post_manage.png](https://github.com/Astrivemanlw/Blog/blob/master/post_manage.png) <br>
