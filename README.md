# [Makefile](https://github.com/qitas/makefile) 
#### qitas@qitas.cn

对C、C++语言程序、需要先把源文件编译成中间代码文件，在Linux下中间代码是 .o 文件，在Windows下是 .obj 文件，这个动作叫做编译（compile）。把大量的.o文件合成执行文件叫作链接（link），对于编译和链接过程需要有相应文件的路径。

 make命令执行时，需要一个 Makefile 文件，以告诉make命令需要怎么样的去编译和链接程序。
```
make，又指GNU Make，指一条可执行指令，该指令是读入一个名为makefile的文件然后执行这个文件中指定的指令。
Make从makefile文件中获得构建程序的依赖关系，Makefile列出了每个目标文件以及如何由其他文件来生成它。 
编写一个程序时，为它编写一个makefile文件，就可以使用Make来编译和安装这个程序。
```
 Makefile文件就是告诉make命令怎么样地去编译和链接程序。Makefile就像一个Shell脚本一样，其中也可以执行操作系统的命令。

### [收录资源](qitas/) 

- [文档](docs/) 
- [示例](demo/) 

#### 关联上层项目：[mAIn智慧构建平台](https://github.com/Qitas/mAIn) 

[![sites](qitas/qitas.png)](http://www.qitas.cn)
## 锻造最美之器