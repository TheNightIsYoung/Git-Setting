# YaHei Consolas Hybrid 1.12

a font for developers that correctly displays Asian characters when mixed with Latin.

**[ Note that ]:** 

I am not the author of 'YaHei consoles Hybrid', but a simple user. Personal favorite programming font, put it on GitHub for easy download and use in the future.

## 1. Set Up In Windows ##

**Step 1 >>> TTF Download**

TTF 字体关联文件下载

```
	$ git clone 
```

**Step 2 >>> TTF Setup**

如果 TTF 文件关联程序没有出错，可直接双击 TTF（YaHei Consolas Hybrid 1.12.ttf）文件，在弹出的字体预览安装界面中，点击 **“安装”** 按钮进行字体安装。

字体安装成功后，直接关闭安装窗口即可。

**Step 3 >>> Check Setup**

系统盘符下在字体目录（C:\Windows\Fonts）中查找 `YaHei Consolas Hybrid`，可以发现字体已经成功安装到字体目录中。

这时，你会发现：你已经可以在 Office 或者 IDE 中使用它了。

## 2. Set Up In Ubuntu/Debian ##

**Step 1 >>> Download 'YaHei Consolas Hybrid' TTF**

```
	$ git clone https://github.com/yakumioto/YaHei-Consolas-Hybrid-1.12
```

**Step 2 >>> 创建字体存放目录**

在系统 `/usr/share/fonts/truetype/` 目录下，创建字体库的存放目录 'YaHei Consolas Hybrid' :

```
	$ sudo mkdir -p /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
```

**Step 3 >>> 复制 TTF 文件到系统字体存放目录**

将 'YaHei Consolas Hybrid 1.12.ttf' 复制到上面建立的字体存放文件夹中.

```
	$ sudo cp YaHei\ Consolas\ Hybrid\ 1.12.ttf /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
```

**Step 4 >>> 修改字体相关文件权限**

修改字体目录，字体文件的权限：

```
	$ sudo chmod 644 /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
	$ cd /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
	$ sudo chmod 644 YaHei\ Consolas\ Hybrid\ 1.12.ttf
```

**Step 5 >>> 开始字体安装**

开始安装字体：

```
	### 1. 创建字体的 fonts.scale 文件，用来控制字体旋转缩放
	$ sudo mkfontscale
	
	### 2. 创建字体的 fonts.dir 文件，用来控制字体粗斜体产生	
	$ sudo mkfontdir
	
	### 3. 建立字体缓存信息，也就是让系统认识该字体
	$ sudo fc-cache -fv
```

至此，就可以在 IDE 中使用该字体了...
