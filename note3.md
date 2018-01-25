# linux shell
- echo $变量名 显示变量内容
- env 显示系统预定义变量
- set 显示环境变量和用户自定义变量
- export 将用户自定义的变量变成环境变量（方便该变量在其他子程序中使用）
 若该变量为扩增内容时，如下：PATH="$PATH":/home
- unset 变量名 取消变量
- history -n 查看n条历史命令
## 数据流重导向
- 标准 输入（0） < 或<<
- 标准输出（1） 1>  或>>(两个大于号时累加输入，不删除以前的，文件没有时会自动生成)
- 错误输出（2） 2> 或 2>>
- find +路径+ -name +文件名可以查找文件
- 例子： find /home -name 1.txt > right 2>error 将查找正确的信息放在right文件中，错误信息放在error文件中。
find /home -name 1.txt >file1 2>&1 将正确和错误信息输出到一个文件中