##我的DOLl开发环境配置流程
This is ChenWenchen's first Git respository, ES2016_14353033.
2016/10/7 

* 1、首先我使用的是上学期上操作系统的课程安装的虚拟机（VMware上的Ubuntu），已经配置好了Ubuntu的基础上直接进行dol配置。 
* 2、首先安装一些需要用到的环境，用sudo apt-get命令进行：`sudo apt-get update` , `sudo apt-get install ant` , `sudo apt-get install openjdk-7-jdk` , `sudo apt-get install unzip`. 
* 3、下载ststemc和dol的压缩包，新建目录并解压： `unzip dol_ethz.zip -d dol` , `tar -zxcf systemc-2.3.1.tgz`
* 4、编译systemc： `../configre CXX=g++ --disable-async-updates` , `sudo make install` 
* 5、修改build_zip.xml中编译systemc的位置property name="systemc.lib" value="工作目录/lib-linux/libsystemc.a"
