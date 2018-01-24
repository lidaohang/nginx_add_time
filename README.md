# nginx_add_time

### nginx核心时间点注入
$request_time           #nginx处理请求所用总时间
 
$request_header_time    #client从建立连接nginx成功后header头接收完毕的时间

$request_body_time      #client从建立连接nginx成功后body接收完毕的时间

$request_module_time    #client从建立连接nginx接收完数据后到upstream连接之前所用的时间
 
$upstream_connect_time  #nginx与upstream_server建立连接所用时间

$upstream_process_time  #nginx从建立连接发送数据后nginx成功到接收upstream_server第一个字节之间的时间(这里包含后端处理时间以及后端响应回来的网络时间)

$upstream_send_time     #nginx从建立连接upstream_server后开始发送数据到发送完最后一个字节之间的时间(这里指发送到缓冲区的时间，不管对方接受与否)

$upstream_response_time #nginx从连接upstream成功到接收upstream返回最后一个字节所用总时间
