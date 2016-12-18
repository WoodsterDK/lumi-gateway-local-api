# 人体传感器 PIR sensor


##属性上报 status report

人体传感器探测到人会立即上报一次report信息。在一直有人的情况下为了省电人体传感器最快一分钟发送一次report。 

PIR sensor will report once it detects human body.

| 属性 | 说明 |
| -- | -- |
| battery | 0-100电池电量 |
| status | motion探测到有人 |

```{"cmd":"report","model":"motion","sid":"112316","short_id":4343,"token":"4","data":"{\"status\":\"motion\"}" }```

##心跳上报(~60分钟每次): heatbeat every 60 minites

```{"cmd":"report","model":"motion","sid":"112316","short_id":4343,"token":"4","data":"{\"battery\":\"71\"}" }```





