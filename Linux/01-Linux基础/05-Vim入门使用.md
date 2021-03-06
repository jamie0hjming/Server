## 一 vi与vim

#### 1.1 vi
vi是Linux上的一款编辑器，但是没有排版等类似word那样的功能，它只是一个文本编辑程序，支持输出、删除、查找、替换、块操作。vi没有菜单，只有命令。  

#### 1.2 vi工作模式

vi有三种基本工作模式：命令模式，文本输入模式，末行模式：
![](/images/linux/00-vi模式.png)

命令行模式:
```
使用 vi 1.txt时，默认就会进入命令模式，这时候输入任何信息都不会显示，而是以命令形式执行。若输入的字符不是Vi的合法命令，Vi会响铃报警。
任何时候，不管用户处于何种模式，只要按一下ESC键，即可使Vi进入命令模式。
```

编辑模式:
```
在命令模式下输入 i 即可进入编辑模式；在命令模式下输入附加命令a 、打开命令o、修改命令c、取代命令r或替换命令s都可以进入文本输入模式。	在该模式下，用户输入的任何字符都被Vi当做文件内容保存起来，并将其显示在屏幕上。在文本输入过程中，若想回到命令模式下，按键ESC即可。
```

末行模式:
```
末行模式也称ex转义模式。在命令模式下，用户按“:”键即可进入末行模式下，此时Vi会在显示窗口的最后一行(通常也是屏幕的最后一行)显示一个“:”作为末行模式的提示符，等待用户输入命令。多数文件管理命令都是在此模式下执行的(如把编辑缓冲区的内容写到文件中等)。末行命令执行完后，Vi自动回到命令模式。如果要直接从命令模式转换到编辑模式，可以键入命令a或者i。
```

退出vi命令：
```
shift zz
或者从末行模式退出，输入 w（保存） q（退出）
```

#### 1.3 vim

vim是从 vi 发展出来的一个文本编辑器 。代码补完、编译及错误跳转等方便编程的功能特别丰富。


## 二 