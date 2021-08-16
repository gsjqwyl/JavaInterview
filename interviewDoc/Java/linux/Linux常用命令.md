**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


### 启动网络命令

ip addr 查看网卡信息

```
service network start 启动网卡
service network stop 关闭网卡
service network restart 重启网络
```

### pwd命令

pwd命令，查看当前目录的路径

linux下所有的绝对路径都是从根目录"/"开始

root:是linux下root用户的根目录

home:是linux下其他用户的默认根目录 （例如：在linux上创建了一个bow用户，那么就会在/home下面生成一个bow目录作为bow用户的根目录）

etc:是linux下系统配置文件目录

tmp:临时文件目录，所有用户都可以用



### ls命令

ls [参数] 目录路径
ls 表示查看目录下的文件

```
ls #表示查看当前目录下的文件
ls -l #表示查看当前目录下的详细信息
ls -a #表示查看当前目录下的所有文件(包含隐藏文件)
ls -la #表示查看当前目录下的所有文件（包含隐藏文件）的详细信息
ls -lh #h是以适当的单位来显示文件的大小 ls -lh表示查看当前目录下的文件的详细信息，并以合适单位显示文件大小 
 
ls -l / #表示查看根目录"/"下文件的详细信息
 
ls /etc #表示查看目录/etc下的文件
 
ls --help #查看命令的帮助文档
--help参数：所有linux上的命令都有，但写法上有如下几种：
 (1)--help
  (2)--h
  (3)-help
  (4)-h
ll命令:它和ls -l命令功能相同，但是不是所有的linux上都默认安装
```



### cd命令

cd 目录路径 #进入一个目录，目录路径可以是绝对路径(以/开始的路径都是绝对路径)，也可以是相对路径
相对路径：以非/开始的路径，
注意: "."表示当前目录
"…"表示当前目录的上一级目录，它可以多个一起使用
"~"表示当前用户的根目录 例如：root用户时，~表示/root目录 bow用户时，~表示/home/bow目录

```
cd / #表示进入系统根目录
cd usr/ #表示进入当前目录下的usr目录
cd local/ #表示进入当前目录下的local目录
cd ./bin #表示进入当前目录下的bin目录
cd .. #表示进入当前目录的上一级目录
cd ../.. #表示进入当前目录的上级目录的上一级目录
cd /usr/local/bin #进入/usr/local/bin目录
cd ../etc #表示进入和当前目录同级的etc目录 #..表示当前目录的上一级目录 ../etc表示当前目录上级目录下的etc目录（和当前目录同级）
cd ~ #表示进入当前用户的根目录（cd ~ 和直接执行cd后不加目录的效果相同）
 #例如：root用户进入/root目录，bow用户进入/home/bow目录
 
cd ~/data #表示进入当前用户根目录下的data目录 例如：root用户则进入了/root/data目录
```



### mkdir命令

mkdir 目录路径 #创建一个目录，目录路径可以是绝对路径也可以是相对路径

```
mkdir data #在当前目录下创建一个data目录
mkdir ./dir #在当前目录下创建一个dir目录
mkdir /root/tmp #在/root目录下创建一个tmp目录
```

mkdir创建目录时，只有在目录的上级目录存在时，才会创建

mkdir -p 目录#创建目录时，如果没有父目录，会创建父目录，递归地创建目录
mkdir -p a/b/c #在当前目录下创建3级目录



### rmdir命令

```
rmdir [参数] 目录路径 #删除目录命令，rmdir默认只能删除空目录
 
rmdir ./dir #删除当前目录下的dir目录
 
rmdir -p 目录路径 #表示删除目录和它的父目录（目录要是一个空目录）
rmdir -p a/b/c #删除当前目录下的a/b/c目录
```



### touch命令

touch 命令 #创建文件命令

touch 文件路径

```
touch 1.txt #在当前目录下创建一个1.txt文件
touch /root/2.txt #在/root目录下创建一个2.txt文件
```



### rm命令

rm [参数] 路径 #删除命令

rm 1.txt #删除当前目录下的1.txt文件，删除时会提示，是否删除如果输入y表示删除，输入n表示不删除

rm -f /root/2.txt #-f表示强制删除，不会提示,强制删除/root目录下的2.txt

```
rm -r a/ #递归的删除当前目录下a目录下的所有内容
[root@bow ~]# rm -r a/
rm：是否进入目录"a/"? y
rm：是否进入目录"a/b"? y
rm：是否进入目录"a/b/c"? y
rm：是否删除普通空文件 "a/b/c/3.txt"？y
rm：是否删除目录 "a/b/c"？y
rm：是否删除普通空文件 "a/b/2.txt"？y
rm：是否删除目录 "a/b"？y
rm：是否删除普通空文件 "a/1.txt"？y
rm：是否删除目录 "a/"？y
rm -rf a/ #强制删除当前目录下a目录及a目录下的所有内容
 
rm -rf * #删除当前目录下的所有内容
rm -rf a/* #删除当前目录下a目录下的所有内容
rm -rf *.txt #删除当前目录下的所有txt文件
rm -rf *s* #删除当前目录下所有名字中包含s的文件或文件夹
```



### echo命令

echo #输出命令，可以输入变量，字符串的值

```
echo Hello World #打印Hello World
echo $PATH #打印环境变量PATH的值,其中$是取变量值的符号，用法：$变量名 或者 ${变量名}
 
echo -n #打印内容但不换行
echo -n Hello World
```



### >和>>命令

和>>:输出符号，将内容输出到文件中，>表示覆盖(会删除原文件内容) >>表示追加

```
echo Hello World > 1.txt #将Hello World输出到当前目录下的1.txt文件
 #如果当前目录下没有1.txt文件会创建一个新文件，
  #如果当前目录下有1.txt，则会删除原文件内容，写入Hello World
echo 1234 >> 1.txt #将1234追加到当前目录下的1.txt中，如果文件不存在会创建新文件
```

通过>和>>都可以创建文件



### 文件查看命令

cat 文件路径 #查看文件的所有内容

```
cat 1.txt #查看当前目录下1.txt的内容
cat /root/1.txt #查看/root目录下的1.txt文件内容
```

more 文件路径 #分页查看文件内容

more linux常用命令.txt #分页查看当前目录下linux常用命令.txt文件的内容
\#按空格或回车，会继续加载文件内容，按q退出查看
\#当加载到文件末尾时，会自动退出查看

less 文件路径 #分页查看文件内容
less linux常用命令.txt #分页查看文件内容，按空格继续加载文件，按q退出查看，不会自动退出查看

head [参数] 文件路径 #从文件开始查看文件

```
head linux常用命令.txt #查看文件的前10行内容
 
head -n 文件路径 # n是一个正整数，表示查看文件的前n行数据
head -20 linux常用命令.txt #查看文件的前20行内容
```

tail [参数] 文件路径 #从文件的末尾查看文件内容
tail linux常用命令.txt #查看文件的后10行内容

```
tail -n 文件路径 # n是一个正整数，表示查看文件的后n行数据
tail -15 linux常用命令.txt #查看文件后15行内容
 
tail -f 文件路径 #动态的查看文件的最后几行内容(查看文件时，等待文件更新，如果文件更新了，会显示出新的内容)
```

tail -f 1.txt #查看文件1.txt的最新内容，tail -f 一般用来查看日志文件 按CTRL+C或才CTRL+Z退出查看

```
CTRL+C：表示暂停进程
CTRL+Z: 表示停止进程
```



### 文件编辑命令

vi/vim命令：这两个命令在使用上几乎完全一样（个人喜欢vim命令）

安装vim命令：（安装是需要网络的）

```
 yum -y install vim
```

yum命令是centos和red hat系统上使用官方资源包去安装软件的命令

```
yum -y install 软件名
yum -y remove 软件名
```

查看虚拟机能不能上外网：

```
ping www.baidu.com
CTRL+C或者CTRL+Z退出
```

vim命令总体分为两类

vim 文件路径 --进入非编辑模式

非编辑模式命令：

```
yy：复制光标当前行
p：粘贴
dd:删除光标当前行
$:光标跳到当前行的行尾
^:光标跳到当前行的行首
 
:s/原字符串/新字符串/:替换光标当前行内容
:%s/原字符串/新字符串/g:全文替换 #g表示global i表示ignore忽略大小写
 
/要查找的内容:从光标当前行向后查找内容
/d #在文件中查找d字母
?要查找的内容：从光标当前位置向前查找内容
?d #查找文件中的d字母
CTRL+F:向下翻1页
CTRL+B:向上翻1页
 
:set nu：显示文件的行号
:set nonu: 去掉行号显示
u:撤消
 
**:set ff :显示文件的格式 #unix表示在unix上的文件 dos表示文件是windows上的文件**
:w ：表示保存文件
:q :表示退出vim命令
:wq:保存并退出
:w!:强制保存
:q!:强制退出但不保存
:wq!:强制保存并退出
i:表示进入编辑模式，并且光标在当前行
o：表示进入编辑模式，并且光标出现的当前行的下一行(新行)
```

编辑模式命令：

编辑模式下可以能过方向键控制光标的位置，并且可以输入文件到光标当前位置

```
 ESC:退出编辑模式
```



### cp命令

cp 拷贝命令

cp [参数] 原文件路径 目标文件路径

```
cp 1.txt a/ #将1.txt文件拷贝到a目录下
cp 1.txt 2.txt #将1.txt拷贝到2.txt
cp -r a data #-r参数表示将目录和目录下的文件一起拷贝，将a目录拷贝到data目录
```



### scp命令

scp 远程拷贝命令，它可以将本地文件拷贝到远程服务器，也可以将远程服务器的文件拷贝到本地，也可以将一台服务器文件拷贝到另一台

```
scp -r 本地文件路径 用户名@ip[:port]:远程路径 #将本地文件拷贝到远程服务器
scp -r 2.txt root@192.168.5.105:/root/data/ #将本地的2.txt拷贝到192.168.5.105的/root/data目录下
 
scp -r 用户名@ip[:port]:远程文件路径 本地路径 #将远程文件拷贝到本地
scp -r root@192.168.5.105:/root/3.bak /root/data #将远程的/root/3.bak文件拷贝到本地的/root/data目录
```

scp -r 用户名@ip[:port]:远程文件路径 用户名@ip[:port]:远程文件路径 #将文件从一台服务器拷贝到另一台服务器

```
scp -r root@192.168.5.105:/root/tmp root@192.168.5.105:/root/data/ #将/root/tmp拷贝到远程的/root/data目录下
```



### mv命令

mv 移动命令,它可以移动文件,也可以给文件改名

mv 原文件路径 目标文件路径 #将文件从一个地方拷贝到另一个地方

```
mv 1.txt 12.txt #将文件1.txt改名为12.txt
mv tmp tmp #将tmp目录改名为tm
mv 12.txt tm #将文件12.txt移动到tm目录下
```



### man命令

man 命令,查看命令的命令,查看命令帮助文档(显示的信息最详细)

```
man mv #查看mv命令的文件
 
man命令和命令的 --help参数结果相似(man命令只适用于linux本身的命令)
```



### free命令

free命令,它是用来查看系统内存的命令

```
free #查看系统内存使用情况
free -h #查看内存使用情况,并且以合适的单位显示大小
```



### df命令

df命令,它是查看系统硬盘的命令

```
df #查看系统硬盘使用情况
df -h #查看硬盘使用,并以合适单位显示大小
```



### wc命令

wc 命令,word count的缩写,它是查看文件的单词个数

wc [参数] 文件

```
wc -l linux常用命令.txt #-l表示line行数 计算文件的行数
wc -w linux常用命令.txt #-w表示word单词个数 计算文件的单词个数
```



### ps命令

ps命令,它是查看系统进程的命令

ps -aux

ps -ef

jps 查看java进程



### kill命令

kill 进程id #结束进程

```
root 21752 1.6 0.5 158800 5532 ? Ss 08:34 0:00 sshd: root@pts/0
```

kill 21752 #结束ssh登陆的进程

kill -9 进程id #强制结束进程



### 用户和权限命令

创建用户组:

groupadd 用户组名称 #创建一个用户组

```
groupadd bows #创建一个叫bows的用户组
删除用户组:
groupdel 用户组名称 #删除一个用户组(删除时必须是用户组下没有用户时)
groupdel bows #删除用户组
```

创建用户:

useradd 用户名 [-g 用户组名 -G 用户组名] #创建一个用户,-g指定用户的主用户组,-G指定用户的其他用户组

```
useradd bow -g bows #创建bow用户,并指定它的主用户组是bows
id 用户名 #查看用户的id
id bow #查看用户bow的id
```

删除用户:

```
userdel 用户名 #删除用户
userdel bow #删除用户bow
```

切换用户:

```
su 用户名 #切换用户,但不加载用户的环境变量
su - 用户名 #切换用户,并加载用户的环境变量(建议使用这种方式切换用户)
su bow #切换到bow用户(root用户切换到其他用户是不需要输入密码的,其他用户切换到root用户是要输入root用户密码的,其他用户之间的切换也是需要密码)
exit #退出当前用户的登陆
```

修改用户密码:

```
passwd 用户名 #修改用户密码
passwd bow #修改bow用户的密码
```

权限:

```
文件类型        用户权限       用户组权限       其他用户权限
-                 rw-              r--             r--                . 1 root 
root 5890 3月 23 14:11 linux常用命令.txt
d                 rwx              r-x             r-x                . 4 root 
root  81 3月 24 08:06 data
d表示文件夹    u表示用户权限   g表示用户组权限   o表示其他用户权限
 
r:表示读权限 数字表示为4
w:表示写权限 数字表示为2
x:表示执行权限 数字表示为1
-:表示没有权限
```



### chmod 赋权限命令

```
chmod 权限 文件路径
-rw-r--r--. 1 root root   31 3月  24 07:46 2.txt
chmod u+x 2.txt #给用户加上执行权限
-rwxr--r--. 1 root root   31 3月  24 07:46 2.txt
chmod g+w 2.txt #给用户组加写权限
-rwxrw-r--. 1 root root   31 3月  24 07:46 2.txt
chmod o+x 2.txt #给其他用户加执行权限
-rwxrw-r-x. 1 root root   31 3月  24 07:46 2.txt
chmod g-w 2.txt #去掉用户的写权限 
-rwxr--r-x. 1 root root   31 3月  24 07:46 2.txt
```

用3个数字来设置文件或目录的权限,第1个数字表示用户权限,第2数字表示用户组权限,第3个数字表示其他用户权限

```
chmod 755 2.txt #设置用户的权限为rwx,用户组的权限r-x,其他用户的权限r-x
-rwxr-xr-x. 1 root root 31 3月 24 07:46 2.txt
chmod 766 2.txt #设置用户权限为rwx,用户组权限rw-,其他用户的权限rw-
-rwxrw-rw-. 1 root root 31 3月 24 07:46 2.txt
```

设置目录权限时,要使用-R参数,保证目录下的所有文件和目录的权限相同

```
drwxr-xr-x. 4 root root 81 3月 24 08:06 data
chmod -R 777 data #将data目录以及它下面的所有文件的权限设置为rwxrwxrwx
drwxrwxrwx. 4 root root 81 3月 24 08:06 data
```

chown 命令,它是更改文件所属用户

```
chown -R 用户[:用户组] 目录或文件
-rwxrw-rw-. 1 root root 31 3月 24 07:46 2.txt
chown bow 2.txt #将2.txt的所属用户改为bow
-rwxrw-rw-. 1 bow root 31 3月 24 07:46 2.txt
chown bow:bows 2.txt #将2.txt所属的用户改为bow,用户组改为bows
-rwxrw-rw-. 1 bow bows 31 3月 24 07:46 2.txt
drwxr--r--. 4 root root 81 3月 24 08:06 data
chown -R bow:bows data #将data目录及它子目录文件的所属用户改为bow,用户组改为bows
drwxr--r--. 4 bow bows 81 3月 24 08:06 data
```



### 查找命令

find命令,可以根据文件的时间,名称等查找文件

```
find *.txt #查找txt文件
```

grep 命令,查找内容

```
grep cat linux常用命令.txt #在linux常用命令.txt文件中查询包含cat的行,查找文件内容
```

| 通道符号,连接两个命令的,将前一个命令的查询结果传给后一个命令

```
ps -ef | grep sshd #查看系统中sshd的进程 
ps -ef | grep java #查看所有java进程
grep -v #-v参数表示查询不包含查找条件的行
grep -v cat linux常用命令.txt #查找linux常用命令.txt中不包含cat的行
 
ps -ef | grep sshd | grep -v grep #查询sshd的进程,不包括grep的行
```

–了解性查询命令

```
who命令 #查询系统中的用户(登陆的用户)
whoami命令 #查看系统当前用户名
whereis命令 #查看系统安装的某个软件的路径
whereis python #查看python的安装路径
which 命令 #查找软件的可执行文件路径 
which python #查看python可执行文件路径
```



### 压缩命令

安装zip和unzip命令:

```
yum -y install zip unzip
```

zip压缩命令

zip 压缩文件名 要压缩的文件路径

```
zip 2.zip 2.txt #将2.txt压缩到2.zip中
 
zip data.zip data #只会压缩文件夹,不会压缩文件夹下的内容
 
zip da.zip da/* #压缩文件夹和文件夹内的文件(压缩文件夹和它的下一级文件) 
 
zip -r data.zip date #-r表示递归地将文件夹及它的子目录文件全部压缩
```

unzip解压命令

unzip 压缩文件路径

```
unzip 2.zip #将2.zip压缩包解压到当前目录下
unzip -l 压缩文件名 #不解压文件,查看压缩包内的文件
unzip -l da.zip #查看da.zip压缩文件中包含的文件
unzip da.zip -d 目标目录 #将压缩文件解压到指定目录 
unzip da.zip -d tm/ #将压缩文件da.zip解压到tm目录下
```

tar命令,用来压缩和解压缩.tar和.tar.gz包

压缩.tar包:

```
tar cvf 压缩文件名 要压缩的文件或目录
tar cvf 2.tar 2.txt #将2.txt压缩为2.tar包
tar cvf data.tar data #将data目录夸张到data.tar包中
```

解压.tar包:

tar xvf 压缩文件名 [-C 指定解压目录]

```
tar xvf 2.tar #将2.tar解压到当前目录
tar xvf 2.tar -C a/ #将2.tar解压到a目录
tar xvf data.tar #解压data.tar到当前目录
```

压缩.tar.gz包:

```
tar zcvf 压缩文件名 要压缩的文件
tar zcvf tm.tar.gz tm #将当前目录下的tm目录压缩为tm.tar.gz
```

解压.tar.gz包:

```
tar zxvf 压缩文件名
tar zxvf tm.tar.gz #将tm.tar.gz解压到当前目录
gzip命令,将文件压缩为.gz包(可以用来压缩.tar文件)
gzip 要压缩的文件 
gzip 2.txt #将2.txt压缩为2.txt.gz
gzip data.tar #将data.tar压缩为data.tar.gz
```



### source命令

source 文件路径 #让配置文件修改结果立即生效,(还可以在shell脚本中引用其他的shell脚本)

```
/etc/profile #linux上的系统环境变量配置文件
source /etc/profile #将系统环境变量生效
```



### export命令

```
export 导入全局变量(环境变量)
 
export 变量名=变量值
export 变量名
 
变量的赋值:
变量名=变量值
```

<<EOF

<<EOF … EOF:将<<EOF和EOF之间的多行内容传给前面的命令,
其中EOF可以是任意字符串,但约定都使用EOF

```
[root@bow ~]# cat <<EOF
> HELLO
> WORD
> JOB
> SMITH
> EOF
HELLO
WORD
JOB
SMITH
```

<<EOF是shell脚本中使用sqlplus的基础

```
[root@bow ~]# cat <<A
> 11234
> 1234
> 1234
> 1253
> 1253
> A
11234
1234
1234
1253
1253
```

注意:EOF必须顶行写

```
[root@bow ~]# cat <<EOF
> ASDF
> EOF
> ASDFASDF
> EOF
ASDF
 EOF
ASDFASDF
```



### cut命令

cut 截取命令

```
-f 参数,指定列
-d 参数指定列和列之间的分隔符,默认的分隔符是\t(行向制表符)
cut -f 1 1.txt #取1.txt文件中的第1列内容(列分隔符默认为\t)
cut -f 2 1.txt #取1.txt文件中的第2列内容
cut -f 1 -d ',' 3.txt #取3.txt文件中的第1列(列分隔符为,)
cut -f 2 -d ',' 3.txt #取3.txt第2列
```

wc -l linux常用命令.txt | cut -f 1 -d ’ ’ #取文件linux常用命令.txt的行数(分隔符是空格)

```
[root@bow ~]# cut -f 1 -d ',' <<EOF
> A,B,C
> D,E,F
> EOF
A
D
```



### printf命令

```
%ns　　输出字符串，n是数字，指代输出几个字符
%ni　　输出整数。n是数字，指代输出几个数字
%m.nf　　位数和小数位数。例如：%8.2f 代表输出8位数，其中2位是小数，6位是整数
```

printf 格式字符串 内容

```
[root@bow ~]# printf '%s,%s,%s\n' abc def ghj klj klo qer #一行单词第三个打印成一行,单词和单词之间用逗号隔开
abc,def,ghj
klj,klo,qer
[root@bow ~]# printf '%s %s\n' $(cat 4.txt) #将文件4.txt中的一行内容中的单词划分为两个一组打印 cat 合作查看文件内容 $(cat 4.txt)表示取cat命令的执行结果
empno ename
job sal
comm depno
5.txt内容
A B C D E
F G H
[root@bow ~]# printf '%s,%s\n' $(cat 5.txt)
A,B
C,D
E,F
G,H
[root@bow ~]# printf '%5.2f\n' 12.1 #%5.2f表示输出一个小数,数的长度是5,其中有两个小数
12.10
[root@bow ~]# printf '%5.2f\n' 121234.116134 #如果输出的值最大长度超出5,那么整数部分不变量,小数部分会按照四舍五入的方法保存两位
121234.12
[root@bow ~]# printf '%i\n' 1234.5678  #%i只取数字的整数部分
-bash: printf: 1234.5678: 无效数字
1234
```



### awk命令

awk 命令字符串 要处理的内容

```
[root@bow ~]# awk '{printf $1 "\n"}' 1.txt #printf 打印 $n 表示取第几列 $1表示取第1列 
Hello
smith
tomcat
```

awk ‘{print $2}’ 1.txt #取1.txt的第2列,print和printf功能相同是打印,比printf多一个换行功能

```
[root@bow ~]# awk '{printf $1 ","}' 1.txt
Hello,smith,tomcat,[root@bow ~]#
[root@bow ~]# awk '{printf $1}' 1.txt
Hellosmithtomcat
[root@bow ~]# awk '{printf $1 "\v"}' 1.txt
Hello
     smith
          tomcat
[root@bow ~]# awk '{printf $1 ","}' 1.txt
Hello,smith,tomcat,
```



### sed命令

sed 参数 命令 要处理的内容

```
-n　　一般sed命令会把所有数据都输出到屏幕。如果加入此选择，则只会把经过sed命令处理的行输出到屏幕。
-e　　允许对输入数据应用多条sed命令编辑
-i　　用sed的修改结果直接修改读取的数据的文件，而不是修改屏幕输出
[root@bow ~]# sed '2p' 1.txt #查询第2行
Hello world
smith 18
smith 18
tomcat etl
[root@bow ~]# sed -n '2p' 1.txt
smith 18
[root@bow ~]# sed -i 's/18/20/g' 1.txt 使用sed命令修改1.txt内容,将1.txt中18替换为20
[root@bow ~]# cat 1.txt
Hello world
smith 20
tomcat etl
a\　　追加，在当前行后添加一行或多行。添加多行时除最后一行外，每行末尾需要用"\"代表数据未完结。
d　　删除，删除指定的
p　　打印，输出指定的行
[root@bow ~]# sed -i '2a !' 1.txt #在第2行后面追加一行 !
[root@bow ~]# cat 1.txt
Hello world
smith 20
!
tomcat etl
[root@bow ~]# sed -i '3d' 1.txt #删除文件的第3行内容
[root@bow ~]# cat 1.txt
Hello world
smith 20
tomcat etl
[root@bow ~]# vim 6.txt
[root@bow ~]# cat 6.txt
abcd/home/bow
if ad
 -e /home/bow
abcd/home/bow
if ad
 -e /home/bow
abcd/home/bow
if ad
 -e /home/bow
#将6.txt文件中的/home/bow修改为/user/bw
#注意:替换时,的符号是根据/来判断 s/原字符串/目标字符串/g 如果原字符串或新的字符串中有/时,需要使用\来转义
# 错误写法:s//home/bow//user/bw/g 正确写法 s/\/home\/bow/\/user\/bw/g
[root@bow ~]# sed -i 's/\/home\/bow/\/user\/bw/g' 6.txt
[root@bow ~]# cat 6.txt
abcd/user/bw
if ad
 -e /user/bw
abcd/user/bw
if ad
 -e /user/bw
abcd/user/bw
if ad
 -e /user/bw
```

注意:linux中字符串的下标是从0开始的



### service命令

service服务命令

```
ervice 服务名 [命令]
命令:enable|disable|start|stop|restart|status
start:启动服务
stop:关闭服务
restart:重启服务
status:查看服务状态
service network start #遍历网络
service network stop #关闭网络
service network restart #重启网络
service network status #查看网络状态
service iptables start #centos6及6以下版本,启动防火墙的命令
service iptables stop #centos6及6以下版本,关闭防火墙(注意,关闭防火墙,只是临时关闭,下次重启之后防火墙依然会启动)
service iptables restart #重启防火墙
service mysqld start #启动mysql数据库
service mysqld restart #启动mysql数据库
service mysqld stop #关闭mysql数据库
```



### chkconfig命令

chkconfig命令检查，设置系统的各种服务

```
chkconfig 服务名 on|off #on表示打开服务 off表示关闭服务 通过chkconfig设置的服务是永久生效
centos6及以下版本永久关闭或打开防火墙
chkconfig iptables on #打开防火墙
chkconfig iptables off #永久地关闭防火墙
```

防火墙:

centos7以上:

```
systemctl start firewalld #启动防火墙
systemctl stop firewalld #关闭防火墙(临时关闭)
systemctl status firewalld #查看防火墙状态
systemctl disable firewalld #永久关闭防火墙
systemctl enable firewalld #打开防火墙(不是启动防火墙)
通过firewall-cmd来配置防火墙
```

centos6及以下:

防火墙配置文件:/etc/iptables,这个文件可以详细的配置防火墙,如果没有/etc/iptables文件可以使用iptables save可以生成该文件

iptables 命令配置防火墙

```
service iptables start #centos6及6以下版本,启动防火墙的命令
     service iptables stop #centos6及6以下版本,关闭防火墙(注意,关闭防火墙,只是临时关闭,下次重启之后防火墙依然会启动)
     service iptables restart #重启防火墙
```

环境变量配置文件

/etc/profile是linux系统上配置系统环境变量的一个文件(针对所有用户的配置)
用户根目录下的.bash_profile:是用户环境变量的配置(针对当前用户有效)

```
su - 用户名 #切换用户时,会加载用户根目录下的.bash_profile环境变量配置文件
su 用户名 #不会加载.bash_profile
```

网络配置文件

网卡配置文件目录:/etc/sysconfig/network-scripts

网卡配置文件名都是以ifcfg-开头,其中ifcfg-lo是本地网卡,是不需要配置的

```
vim /etc/sysconfig/network-scripts/ifcfg-enp0s3
#网卡类型
TYPE="Ethernet"
#协议 dhcp表示:ip地址是自动分配的,static表示静态ip(手动配置ip地址),none表示没有协议(也是需要手动配置ip地址)
BOOTPROTO="dhcp"
DEFROUTE="yes"
#网卡名称
NAME="enp0s3"
UUID="deed3fd2-bd67-459b-8a49-ef0dd6e575a2"
DEVICE="enp0s3"
#配置网卡是否随机启动,yes:表示随机启动,no:表示需要手动启动
ONBOOT="yes"
#配置静态ip,BOOTPROTO必须是static或none
#ip地址配置
IPADDR=192.168.1.106
#配置子网掩码
NETMASTER=255.255.255.0
#配置网关
GATEWAY=192.168.1.1
#配置dns:域名解析服务器可以配置多个
DNS1=192.168.1.1
DNS2=192.168.5.1
```

修改完网卡文件之后,*重启网络*即可



### sudo命令

sudo命令,它在非root用户下,去调用一些root用户的命令,或者修改一些文件
sudo命令是需要配置的,sudo的配置文件是/etc/sudoers

```
#给bow用户配置sudo权限
[root@bow ~]# vim /etc/sudoers
##
## Allow root to run any commands anywhere 
root ALL=(ALL) ALL
#给bow用户设置sudo命令权限
bow ALL=(ALL) ALL
```

sudo命令的使用:

sudo 命令

```
[root@bow ~]# su - bow
上一次登录：四 3月 26 07:30:53 CST 2020pts/0 上
[bow@bow ~]$ sudo vim /etc/profile
```



### ping命令

ping命令查看网络连通性的命令和windows上的功能一样

```
ping ip（0.0.0.100）
```



### ifconfig命令

ifconfig命令属于net-tools软件包,使用前需要安装net-tools

net-tools的安装:

```
yum -y install net-tools
ifconfig查看ip地址
```



### netstat命令

netstat命令也属于net-tools软件包

```
netstat -tulp | grep 1521 #查看oracle监听器程序是否正常启动
```



### rpm命令

rpm是linux上的安装命令，用来安装.rpm格式的安装包

```
rpm -ivh .rpm文件的路径 #表示安装软件包
 
rpm -qa #查看已安装的软件 
rpm -qa | grep mysql #查看已经安装的mysql软件包
 
rpm -e --nodeps 安装包名 #卸载软件包 -e表示卸载 --nodeps表示不理会的依赖关系
OK，本文就这样。
```