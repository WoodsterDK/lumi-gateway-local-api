# 设备上报和控制报文格式
device report and control command format

JSON报文格式如下： JSON format as following:

```
{
	"cmd" : "write",           //命令类型 command type
	"model" : "ctrl_neutral1",   //设备类型 device model
	"sid" : "112316",          //设备的id device ID
	"short_id" : 4343,         //zigbee设备的短id zigbee device short id
	"token" : "8",             //用来区分是报文是第几条，可以先忽略这个属性 token
	"data" : "{\" channel_0\":\"on\"}"    //设备状态等信息，再次解开字符串获取其中属性 Data
}```

>其中data的内容是个字符串， 我们对这个字符串再次转成json，从中提取属性。
