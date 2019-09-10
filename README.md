## 功能：
一键调用idat静态分析so、exe、dll，   
导出结果为json文本.

## 运行环境：
win10 x64 1903  
ida 7.0

## 使用步骤：
###### (0)将ida完整程序拷贝到"IDA_Pro_v7.0_Portable"下(程序依赖于idat.exe)  
###### (1)将目标文件放入input中(EXE/DLL/SO)  
###### (2)编写IDAPY脚本,放在script中  
###### (3)运行run.exe  
###### (5)IDAPY脚本运行结果,将输出到output中  
###### (6)IDAPY脚本中的print(),将输出到log中  

## 注意：
IDAPY脚本中的输出文件路径，可使用变量idc.ARGV[1],  
值固定为"\\output\\***.json"

## 目录说明：
IDA_Pro_v7.0_Portable： 存放idat.exe  
input：                 存放待分析的可执行文件  
log：                   存放IDAPY脚本的运行日志  
output：                存放IDAPY脚本的输出  
script：                存放IDAPY脚本  
src(run)：              工具源代码  
