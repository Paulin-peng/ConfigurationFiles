ConfigurationFiles
==================

configuration files, such as repo (download android source file)、.git-completion.bash(git autocomplete bash)

##使用方法
1. 直接使用的作者提供的~/.vimrc和~/.vimrc.bundles， 直接将两个文件下载下来放到自己Linux系统用户home目录下，然后创建了~/.vim文件夹，执行git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle 命令，解决下边两个问题就配置成功了。

	复制结束后，键入命令vim .vimrc时可能遇到好几条这种样子错误提示：……^M

	原因：Windows与Linux环境下换行符不同造成，文件换行符是Windows下的，要处理成Linux环境下。

	解决方法：键入命令vim .vimrc，然后再vim里输入:set ff=unix，然后键入:wq。对于.vimrc.bundles文件同样操作。 
	其他处理方法见：http://blog.csdn.net/cjf_iceking/article/details/47836201

2. 继续输入vim .vimrc可能会报出关于fugitive#statusline()的错误 
解决方法：运行命令BundleInstall执行结束将插件下载完毕后问题自然解决。
3. 还有错误可能是找不到”molokai”颜色配置方案
解决方法：到网址：https://github.com/tomasr/molokai 下载颜色方案，把你下载的molokai.vim复制到的/usr/share/vim/vimXX/colors文件夹下，…/vimXX/…根据你的vim版本确定文件夹的名字，我的是vim74因此完整路径就是：/usr/share/vim/vim74/colors
