# TikTok-Free
TiKTok 地区自由切换（封区解锁）和去水印。Unlock region limit & Remove the watermark when downloading.
Those configuration are specific to shadowroket app.
此配置完美适用于小火箭，surge3版本请访问 @Choler同学的 https://github.com/Choler/TikTok.


----------------


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



--------------------------
tips:
For using MITM, you need A CA Certificate in shadowroket app.
If you had never set a CA before. you need to set it first by following this:

1.Generate A CA Certificate.
2.install this New CA Certificate on your iphone.
3.go to Settings -> General -> About ->Certificate Trust Settings to enable Shadowrocket certificate after the installation is completed.

Then add Those configuration to your config file to enjoy it.


















