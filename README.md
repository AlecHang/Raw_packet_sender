程序使用raw_socket模式进行ip包的发送，ip包的payload可以自定义。

linux环境下请以root权限运行，windows环境下请以管理员权限运行，执行send_packet.py进行发包

执行发包程序时，发包对应的网卡需配置ip地址，src_ip设置为此ip地址, 如果源地址与发包网卡IP不一致时，网卡可能会丢包， 需要网卡设置混杂模式

若dst_ip设置为不存在的ip，发包网卡并不会发送此包，而是转为发送arp包请求dst_ip所在的物理地址（毕竟不知道该往哪儿发嘛）

如果对您有用请star，谢谢~笔芯~
