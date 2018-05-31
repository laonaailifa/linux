#上网
[超赞的 Linux 软件](https://alim0x.gitbooks.io/awesome-linux-software-zh_cn/content/)
[16 Things To Do After Installing Ubuntu 16.04 LTS](https://www.omgubuntu.co.uk/2016/04/10-things-to-do-after-installing-ubuntu-16-04-lts)

## mentohust
下载mentohust.deb
安装


##ssr
	#安装ssr
	git clone https://github.com/SAMZONG/gfwlist2privoxy.git
	cd gfwlist2privoxy/
	mv ssr /usr/local/bin
	chmod +x /usr/local/bin/ssr
	ssr install
	#配置
	ssr config
	#安装privoxy
	apt install -y privoxy
	#全局
	echo 'forward-socks5 / 127.0.0.1:1080 .' >> /etc/privoxy/config
	#PAC
	cd gfwlist2privoxy/
	bash gfwlist2privoxy #输入 127.0.0.1:1080
	cp -af gfw.action /etc/privoxy/
	echo 'actionsfile gfw.action' >> /etc/privoxy/config
	#管理脚本
	mv gfwlist2privoxy/ssr_manager /usr/local/bin
	chmod +x /usr/local/binssr_manager
	
	
	# 启动服务
	ssr_manager start
	# 关闭服务
	ssr_manager stop 
	# 添加开机自启动
	ssr_manager autostart
	
#卸载本地软件

## libreoffice
		
		sudo apt-get update
		sudo apt-get upgrade
		sudo apt-get remove libreoffice-common
		
## 卸载Amazon链接

		sudo apt-get remove unity-webapps-common
		
## 游戏
		
		sudo apt-get purge aisleriot #纸牌王 
		sudo apt-get purge gnome-sudoku #数独 
		sudo apt-get purge gnomine #扫雷 
		sudo apt-get purge gnome-mahjongg  #对对碰 

		
#美化
* unity-tweak-tool

		sudo apt-get install unity-tweak-tool
或者

		wget -q -O - http://archive.getdeb.net/getdeb-archive.key | sudo apt-key add -
		sudo sh -c 'echo "deb http://archive.getdeb.net/ubuntu xenial-getdeb apps" >> /etc/apt/sources.list.d/getdeb.list'
		sudo apt-get update
		sudo apt-get install ubuntu-tweak
* 	gnome-tweak-tool

			sudo apt-get install gnome-tweak-tool
		
##主题
*   Flatabulous 扁平化主题

		sudo add-apt-repository ppa:noobslab/themes
		sudo apt-get update
		sudo apt-get install flatabulous-theme

* numix-gtk-theme  主题

		sudo add-apt-repository ppa:numix/ppa
		sudo apt-get update
		sudo apt-get install numix-gtk-theme numix-icon-theme-circle

##字体图标
* Flat Icons  

		sudo add-apt-repository ppa:noobslab/icons
		sudo apt-get update
		sudo apt-get install ultra-flat-icons
		
* 文泉译微米黑字体
		
		sudo apt-get install fonts-wqy-microhei

##终端
* 安装zsh

		sudo apt-get install zsh
		
* 下载 oh-my-zsh 项目来帮我们配置 zsh

		sudo wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh

* 切换到 zsh 模式

		chsh -s /bin/zsh 

# 软件
* [ chrome](https://www.google.com/chrome/)
* [remarkable](https://remarkableapp.github.io/linux/download.html)
* [wps](http://linux.wps.cn/)

	* 	下载缺失的字体文件，然后复制到Linux系统中的/usr/share/fonts文件夹中。
		[国外下载地址](https://www.dropbox.com/s/lfy4hvq95ilwyw5/wps_symbol_fonts.zip)
		[国内下载地址](http://pan.baidu.com/s/1mh0lcbY)
		下载完成后
		sudo cp * /usr/share/fonts
	* 	执行以下命令,生成字体的索引信息：
		sudo mkfontscale
		sudo mkfontdir
	*	3. 运行fc-cache命令更新字体缓存。
		sudo fc-cache
	


	
*[ VScode](https://code.visualstudio.com/docs/?dv=linux64_deb
* [搜狗输入法](https://pinyin.sogou.com/linux/?r=pinyin)
* [wyy](https://music.163.com/#/download)
	