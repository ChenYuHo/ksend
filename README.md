ksent
=====

命令行推送个人文档到kindle。

**使用指南**

1. 安装

        npm install -g ksent

2. 设置默认发送邮箱，格式: 邮箱地址:密码

        ksent --from yourname@qq.com:yourpassword

3. 推送，如下示例，推送 a.pdf 至 zzxiaoman@kindle.cn 这个kindle接收邮箱：

        ksent -m zzxiaoman@kindle.cn a.pdf

    以上命令，参数 -m 表示接收邮箱。自此，完成推送。

如果脚得每次都要敲 -m 接收邮箱 麻烦，可以设置默认接收邮箱：

    ksent --to zzxiaoman@kindle.cn

这样，以后只需要如下命令即可推送：

    ksent a.pdf

其他

    ksent --subject '邮件主题'

    ksent --text  '邮件正文'

防止kindle 认为邮件里面没有附件..不能推送到kindle设备或者kindle阅读器
        
也可以同时推送多个文档：

    ksent a.pdf b.pdf ../img/photo.jpg /Users/hanan/book/ooxx.txt

查看帮助：

    ksent --help
    
ps: 记得把发送邮箱添加到您的kindle已认可的发件人电子邮箱列表哦
