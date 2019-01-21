# Sidebar Enhancements

### In other languages

English - <https://github.com/SideBarEnhancements-org/SideBarEnhancements.git>

Japanese - <http://taamemo.blogspot.jp/2012/10/sublime-text-2-sidebarenhancements.html?m=1>

Russian - <https://www.youtube.com/watch?v=8I0dJTd58kI&feature=youtu.be&a>

<<<<<<< HEAD
## 介绍

此版本为Sidebar Enhancements的中文版，[原版](https://github.com/SideBarEnhancements-org/SideBarEnhancements)

### [Sublime Text 3+][] 不再支持 ST2; 请使用Sublime Text 3.

Sidebar Enhancements是增强Sublime Text的侧边栏文件和文件夹操作的一款插件 <http://www.sublimetext.com/>

- 一大亮点是提供了“删除”、“打开”和“剪贴板”操作。
- 关闭、移动、打开、恢复受重命名/移动命令的缓冲区。
- 基本功能：新建文件/文件夹、编辑、打开/运行、打开文件位置、查找所选/父文件夹/项目、剪切、复制、粘贴、粘贴到父目录、重命名、移动、删除、刷新……
- 高级功能：可选URI/URL编码复制路径、UTF-8、base64（非常适合嵌入css）编码复制内容、复制img/a/script/style等标签
- 当删除操作受影响时，使用“首选项”来控制是否关闭缓冲区
- 允许在状态栏上显示“文件修改日期”和“文件大小”。

## 安装

下载或复制到与包名同名的文件夹到ST的Packages文件夹中。


也可以到[releases](https://github.com/52fisher/SideBarEnhancements/releases)页面下载，**请注意：下载后的压缩包不能直接使用，要解压去掉内层文件夹，将所有文件放到压缩包的根目录下。**如下载后的压缩包打开后是这样的：
```
--SideBarEnhancements-5.0.23（一级文件夹）
----bin（二级文件夹）
----desktop（二级文件夹）
----edit（二级文件夹）
----Commands.sublime-commands(二级文件)
…
…
```
正确的形式是：
```
--bin（一级文件夹）
--desktop（一级文件夹）
--edit（一级文件夹）
--Commands.sublime-commands(一级文件)
…
…
```

### **安装故障排除**


如果您在安装时遇到问题，请执行以下操作：
- 首先请注意，此包只会在“文件夹”部分添加上下文菜单，而不是“打开方式”部分。
- 打开插件目录。“主菜单 ->首选项 -> 浏览插件目录”.(Main menu -\> Preferences -\> Browse Packages)
- 关闭Sublime Text
- 删除/Packages/SideBarEnhancements文件夹
- 删除User/SideBarEnhancements文件夹
- 打开上级目录，到“Installed Packages”文件夹，检查SideBarEnhancements的任何packages并将其删除
- 打开ST，使用Package Control转到：Remove Package，检查SideBarEnhancements的任何package并将其删除。
- 重启ST
- 打开ST，检查Package Control中是否含有SideBarEnhancements的任何内容（在Remove Package和Enable Package中都要检查）
- 重复直到找不到任何有个内容
- 重启ST
- 重新安装SideBarEnhancements
- 正常使用
## 快捷键 F12

（请注意，从版本2.122104开始，此软件包不再提供快捷键设置，您需要手动将其添加到您的sublime-keymap文件中（请参阅下一节））
使用F12可以在浏览器中打开当前文件

`url_testing` 允许您设置本地服务器的URL，通过F12打开
`url_production`允许您设置产品服务器的URL，通过ALT + F12打开

### 关于绝对路径

-  右键单击侧栏上的任何文件，然后选择：“项目 - \>编辑预览地址”
-  编辑此文件，并使用以下结构添加路径和URL：
=======
Chinese - <https://github.com/52fisher/SideBarEnhancements>

## Description

Provides enhancements to the operations on Sidebar of Files and Folders for Sublime Text. <http://www.sublimetext.com/>

Notably provides delete as "move to trash", open with.. and a clipboard.

Close, move, open and restore buffers affected by a rename/move command. (even on folders)

New file/folder, edit, open/run, reveal, find in selected/parent/project, cut, copy, paste, paste in parent, rename, move, delete, refresh....

Copy paths as URIs, URLs, content as UTF8, content as <data:uri> base64 ( nice for embedding into CSS! ), copy as tags img/a/script/style, duplicate

Preference to control if a buffer should be closed when affected by a deletion operation.

Allows to display "file modified date" and "file size" on statusbar (may be a bit buggy).

## Installation

Download or clone the contents of this repository to a folder named exactly as the package name into the Packages/ folder of ST.

Troubleshooting Installation:

-   First please note this package only adds a context menu to the "Folders" section and not to the "Open Files" section.
-   Open the package folder. Main menu -\> Preferences -\> Browse Packages.
-   Close Sublime Text.
-   Remove the folder "Packages/SideBarEnhancements"
-   Remove the folder "User/SideBarEnhancements"
-   Navigate one folder up, to "Installed Packages/", check for any instance of SideBarEnhancements and remove it.
-   Open ST, with Package Control go to : Remove Package, check for any instance of SideBarEnhancements and remove it.
-   Restart ST
-   Open ST, check if there is any entry about SideBarEnhancements in Package Control(in sections: "Remove Package" and just in case in "Enable Package")
-   Repeat until you find there no entry about SideBarEnhancements
-   Restart ST
-   Install it.
-   It works

## F12 key

(Please note that from version 2.122104 this package no longer provides the key, you need to manually add it to your sublime-keymap file (see next section))

F12 key allows you to open the current file in browser.

`url_testing` allows you to set the url of your local server, opened via F12

`url_production` allows you to set the url of your production server, opened via ALT+F12

### With absolute paths

-   Right click any file on sidebar and select: "Project -\> Edit Projects Preview URLs"
-   Edit this file, and add your paths and URLs with the following structure:

>>>>>>> 97d6ac4d9dca002bbcde92a9724240599176c26a
<!-- -->

    {
        "S:/www/domain.tld":{
            "url_testing":"http://testing",
            "url_production":"http://domain.tld"
        },
        "C:/Users/luna/some/domain2.tld":{
            "url_testing":"http://testing1",
            "url_production":"http://productiontld2"
        }
    }

### 关于相对路径

假如我们有一个具有以下结构的项目

    Project/ < - root project folder
    Project/libs/
    Project/public/ < - the folder we want to load as "http://localhost/"
    Project/private/
    Project/experimental/ < - other folder we may run as experimental/test in another url "http://experimental/"

接着创建配置文件：

`Project/.sublime/SideBarEnhancements.json`

内容：

    {
        "public/":{
            "url_testing":"http://localhost/",
            "url_production":"http://domain.tld/"
        },
        "experimental/":{
            "url_testing":"http://experimental/",
            "url_production":"http://domain.tld/"
        },
        "":{
            "url_testing":"http://the_url_for_the_project_root/",
            "url_production":"http://the_url_for_the_project_root/"
        }
    }

...

<<<<<<< HEAD
你可以创建配置文件 `some/folder/.sublime/SideBarEnhancements.json` 在任何地方.

#### F12 快捷键冲突

在Sublime Text 3中，`F12`键默认绑定到`“goto_definition”`命令中。 此Package该快捷键相冲突，便不会有任何反应。 您需要立即手动添加按键配置：转到“首选项 - >Package Settings - >Side Bar -> Key Bindings - User”中并添加以下任何内容：
        [
            { "keys": ["f12"],
                "command": "side_bar_open_in_browser" ,
                "args":{"paths":[], "type":"testing", "browser":""}
            },
            { "keys": ["alt+f12"],
                "command": "side_bar_open_in_browser",
                "args":{"paths":[], "type":"production", "browser":""}
            },
            {
                "keys": ["ctrl+t"],
                "command": "side_bar_new_file2"
            },
            {
                "keys": ["f2"],
                "command": "side_bar_rename"
            },
        ]

## 配置“打开方式”（用……打开）菜单的注意事项：

文件地址: `User/SideBarEnhancements/Open With/Side Bar.sublime-menu` . 右键单击打开项目中的任何文件，然后选择“用……打开>Edit Applications...”
=======
You can create config files `some/folder/.sublime/SideBarEnhancements.json` anywhere.

#### F12 key conflict

On Sublime Text 3 `F12` key is bound to `"goto_definition"` command by default. This package was conflicting with that key, this no longers happens. You need to manually add the keys now: Go to `Preferences -> Package Settings -> Side Bar -> Key Bindings - User` and add any of the following:

		[
			{ "keys": ["f12"],
				"command": "side_bar_open_in_browser" ,
				"args":{"paths":[], "type":"testing", "browser":""}
			},
			{ "keys": ["alt+f12"],
				"command": "side_bar_open_in_browser",
				"args":{"paths":[], "type":"production", "browser":""}
			},
			{
				"keys": ["ctrl+t"],
				"command": "side_bar_new_file2"
			},
			{
				"keys": ["f2"],
				"command": "side_bar_rename"
			},
		]

## Keybinding for Find in paths:

You may wish to add a key for opening "find in paths.."

	[
		{
			"keys": ["f10"],
			"id": "side-bar-find-files",
			"command": "side_bar_find_files_path_containing",
			"args": {
				"paths": []
			}
		}
	]


## Notes on configuring the `Open With` menu:

Definitions file: `User/SideBarEnhancements/Open With/Side Bar.sublime-menu` (note the extra subfolder levels). To open it, right-click on any file in an open project and select `Open With > Edit Applications...`
>>>>>>> 97d6ac4d9dca002bbcde92a9724240599176c26a

-   On OSX, the 'application' property simply takes the *name* of an application, to which the file at hand's full path will be passed as if with `open ...`, e.g.: "application": "Google Chrome"
-   On OSX, invoking *shell* commands is NOT supported.
-	You should change Caption and id of the menu item to be unique.

<!-- -->

<<<<<<< HEAD
    //application 1
    {
        "caption": "Photoshop",
        "id": "side-bar-files-open-with-photoshop",
        "command": "side_bar_files_open_with",
        "args": {
            "paths": [],
            "application": "Adobe Photoshop CS5.app", // OSX
            "extensions":"psd|png|jpg|jpeg",  //any file with these extensions
            "args":[]
        }
        "open_automatically" : true // will close the view/tab and launch the application
    },

### 参数变量说明

- $PATH - 当前文件的全部路径，如C:\Files\Chapter1.txt.
- $PROJECT - 当前项目的根目录
- $DIRNAME - 当前文件的目录, 如C:\Files.
- $NAME - 当前文件的名称部分,如Chapter1.txt.
- $EXTENSION - 当前文件的扩展名,如 txt.

## FAQ

Q: 为什么菜单没有显示“打开文件”？

- 需要注意：SideBarEnhancements的上下文菜单仅适用于项目中的文件和文件夹（**侧边栏中的文件夹部分**），同时由于ST的限制，不能打开侧边栏中列出的文件。

Q：是否可以关闭“在 **右侧显示预览** 点击文件”。

-  老夫无能为力.
=======
	//application 1
	{
		"caption": "Photoshop",
		"id": "side-bar-files-open-with-photoshop",
		"command": "side_bar_files_open_with",
		"args": {
			"paths": [],
			"application": "Adobe Photoshop CS5.app", // OSX
			"extensions":"psd|png|jpg|jpeg",  //any file with these extensions
			"args":[]
		}
		"open_automatically" : true // will close the view/tab and launch the application
	},

### Vars on "args" param

- $PATH - The full path to the current file, "C:\Files\Chapter1.txt"
- $PROJECT - The root directory of the current project.
- $DIRNAME - The directory of the current file, "C:\Files"
- $NAME - The name portion of the current file, "Chapter1.txt"
- $NAME_NO_EXTENSION - The name portion of the current file without the extension, "Chapter1"
- $EXTENSION - The extension portion of the current file, "txt"
>>>>>>> 97d6ac4d9dca002bbcde92a9724240599176c26a

## 使用其他库文件

(check each license in project pages)

-   "getImageInfo" to get width and height for images from "bfg-pages". See: <http://code.google.com/p/bfg-pages/>
-   "desktop" to be able to open files with system handlers. See: <http://pypi.python.org/pypi/desktop>
-   "send2trash" to be able to send to the trash instead of deleting for ever!. See: <http://pypi.python.org/pypi/Send2Trash>
-   "hurry.filesize" to be able to format file sizes. See: <http://pypi.python.org/pypi/hurry.filesize/>
-   "Edit.py" ST2/3 Edit Abstraction. See: <http://www.sublimetext.com/forum/viewtopic.php?f=6&t=12551>

## 源代码

<https://github.com/SideBarEnhancements-org/SideBarEnhancements>

## 论坛

<http://www.sublimetext.com/forum/viewtopic.php?f=5&t=3331>

<<<<<<< HEAD
# 贡献者:
(非常感谢)
-   Aleksandar Urosevic
-   bofm
-   Dalibor Simacek
-   Devin Rhode
-   Eric Eldredge
-   Hewei Liu
-   Jeremy Gailor
-   Joao Antunes
-   Leif Ringstad
-   MauriceZ
-   Nick Zaccardi
-   Patrik Göthe
-   Peder Langdal
-   Randy Lai
-   Raphael DDL Oliveira
-   robwala
-   Stephen Horne
-   Sven Axelsson
-   Till Theis
-   Todd Wolfson
-   Tyler Thrailkill
-   Yaroslav Admin
=======
# Contributors:

(Thank you so much!)
Aleksandar Urosevic, bofm, Dalibor Simacek, Devin Rhode, Eric Eldredge, Hewei Liu, Jeremy Gailor, Joao Antunes, Leif Ringstad, MauriceZ, Nick Zaccardi, Patrik Göthe, Peder Langdal, Randy Lai, Raphael DDL Oliveira, robwala, Stephen Horne, Sven Axelsson, Till Theis, Todd Wolfson, Tyler Thrailkill, Yaroslav Admin
>>>>>>> 97d6ac4d9dca002bbcde92a9724240599176c26a

## TODO

<https://github.com/SideBarEnhancements-org/SideBarEnhancements/issues/223>

## License

"None are so hopelessly enslaved as those who falsely believe they are free." Johann Wolfgang von Goethe

Copyright (C) 2014 Tito Bouzout [tito.bouzout@gmail.com][]

This license apply to all the files inside this program unless noted different for some files or portions of code inside these files.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. <http://www.gnu.org/licenses/gpl.html>

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/gpl.html>

## 觉得有用?欢迎支持（原作者） ^_^


[捐赠该项目.][]

  [Sublime Text 3+]: http://www.sublimetext.com/
  []: https://www.dropbox.com/s/ckz5n2ncn2pxkii/sidebar.png?dl=1
  [desktop]: http://pypi.python.org/pypi/desktop
  [Send2Trash]: http://pypi.python.org/pypi/Send2Trash
  [bfg-pages]: http://code.google.com/p/bfg-pages/
  [tito.bouzout@gmail.com]: tito.bouzout@gmail.com
  [Donate to support this project.]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=DD4SL2AHYJGBW
