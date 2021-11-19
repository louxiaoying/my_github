# my_github
test for linux
$git config --global user.name "your name"
$git config --global user.email  "your email"
git config --list
cd  ~/.ssh
ssh-keygen -t rsa -C "邮箱地址"
#打开/home/tangxingwang/.ssh/id_rsa文件夹下id_rsa.pub文件，复制里面的内容，打开之后不要惊讶，这就是你需要的密钥。你需要登录你的github来添加这个密钥，登录github后找到SSH and GPG keys
git clone git@github.com:tangxingwang/my_github.git
#从linux中添加文件到github中
cd my_github  
touch test.py
git add test.py
git status
git commit -m"first commit"
git push origin master
