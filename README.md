# TikTok-Free
TiKTok 地区自由切换（封区解锁）和去水印。Unlock region limit & Remove the watermark when downloading.
Those configuration are specific to shadowroket app.
此配置完美适用于小火箭，可以复制粘贴到自己现有的规则中使用。surge3版本请访问 @Choler同学的 https://github.com/Choler/TikTok.

```


[Rule]
DOMAIN,api-h2.tiktokv.com,PROXY
DOMAIN,api2-16-h2.musical.ly,PROXY
DOMAIN,api2-19-h2.musical.ly,PROXY

[URL Rewrite]
(.*video_id=\w{32})(.*watermark=)(.*) $1 302
((carrier|account|sys)_region=)CN JP 302

[MITM]
hostname = ,api*.tiktokv.com,*.musical.ly,
enable = true


```
  
**For using MITM, you need A CA Certificate in shadowroket app.**<br>
**If you had never set a CA before. you need to set it first by following this:**<br> 
 
1.  Generate A CA Certificate. <br>
2. install this New CA Certificate on your iphone.<br>
3. go to Settings -> General -> About ->Certificate Trust Settings to enable Shadowrocket certificate after the installation is completed.<br>
Then add Those configuration to your config file to enjoy it. 

<br>
<br>
<br>

## tips: <br>
If you need, you can watch videos from different nations. Just modifying the second region code```JP```in```((carrier|account|sys)_region=)CN JP 302``` （default is ```JP``` means transfer to Japan).<br>
 **e.g**
 
   to US ：              ```((carrier|account|sys)_region=)CN US 302```<br>
   to UK ：              ```((carrier|account|sys)_region=)CN UK 302```<br>
   to Taiwan Province：  ```((carrier|account|sys)_region=)CN TW 302```<br>


## For greenhand: <br>



1<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/1.png) <br>
next:
2<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/2.png) <br>
next:
3<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/3.png) <br>
next:
4<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/4.png) <br>
next:
5<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/5.png) <br>
next:
6<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/6.png) <br>
next:
7<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/7.png) <br>
next:
8<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/8.png) <br>
next:
9<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/9.png) <br>
next:
10<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/10.png) <br>
next:
11<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/11.png) <br>
next:
12<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/12.png) <br>
next:
13<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/13.png) <br>
next:
14<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/14.png) <br>
next:
15<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/15.png) <br>
next:
16<br>
![TikTok-Free](https://github.com/Pinanchen/TikTok-Free/blob/master/pics/16.png) <br>


---------Over.<br>
