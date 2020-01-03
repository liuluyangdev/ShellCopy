# ShellCopy
批量将已知路径的文件复制到指定路径下

这是Linux下的一个shell脚本

使用方式：./ShellCopy midi_file aosp

参数说明：

midi_file ：一个文件，里面可以是一些你修改过的 文件的绝对路径。只是一个记录

aosp ： 必须是midi_file中记录的所有路径 共同拥有的一个文件夹的名字

拿Android源码来举例：

我在/home下新建一个名为 Android_Q 的文件夹，然后将Android的AOSP代码pull到这个文件夹下，
此时可以在Android_Q这个文件夹的同级路径下建个midi_file文件，来记录修改过的文件，
此时的aosp参数可以是：Android_Q

这个脚本的目的就是，将你记录的修改过的文件，提取出来，并保持原目录结构！

运行的结果会生成一个patch的文件夹，里面会包含midi_file里所有记录的文件！
