# Sublime&Markdown
==============================
## Sublime
 * 安装package control
 * 安装实用插件
 * 实用插件的介绍和选择
 * emmet语法  
 
## Markdown
 * Markdown基本语法
 * Markdown工具选择
 * Markdown实用模板

==================================

####安装package control

_方法一：_用代码实现安装:   
从菜单 View - Show Console 或者 ctrl + ~ 快捷键，调出 console，对于不同版本的sublime分别在console输入以下代码，重启sublime即可生效  

*sublime text 3*

```import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())```  

*sublime text 2*

```import urllib2,os; pf='Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler( ))); open( os.path.join( ipp, pf), 'wb' ).write( urllib2.urlopen( 'http://sublime.wbond.net/' +pf.replace( ' ','%20' )).read()); print( 'Please restart Sublime Text to finish installation')```

** 方法二：用package control安装包实现安装
  * 点击Preferences > Browse Packages菜单
  * 进入打开的目录的上层目录，然后再进入Installed Packages/目录
  * 下载 Package Control（sublime-package ）并复制到Installed Packages/目录
  * 重启Sublime Text（看到preferences下出现package control即是安装成功）
  
  
-------------------------------------------------------------------------------
#### 安装插件
* 选择：Preferences > Package control，打开一个窗口，然后选择：Package Control: Install Package，选择所需插件即可。

