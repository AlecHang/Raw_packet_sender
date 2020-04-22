程序使用raw_socket模式在链路层进行ip包的发送，ip包的payload可以自定义。

linux环境下请以root权限运行，windows环境下请以管理员权限运行，执行send_packet.py进行发包

发包的mac源地址、目的地址需要自己填充，但不管填充什么都一定能发出去。

执行发包程序时，发包对应的网卡填写需正确。
s.bind(("p1p3", socket.htons(0x0800)))，"p1p3"改为需要发包的网卡

如果对您有用请star，谢谢~笔芯~

