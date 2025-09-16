1.直接本地运行token.html根据提示获取即可
然后访问页面根据提示获取token
2.将sjapi中的// 发送POST请求
                const response = await fetch('/api/public/emailList', 
将/api/public/emailList连接补充完整(注意仅管理员账户可用)
3api收件使用访问你的域名/sjapi.html?token=你获取的token  注意:需要网页的需要吧token.html改为index.php上传到服务器或者虚拟主机即可访问你的域名?token=你获取的token 
4.批量生成同1的方式
5.#cloudflare  work的方式（worker-2025-09-15.js为api收件）
 api收件编辑work中的内容将// 发送POST请求
                const response = await fetch('/api/public/emailList', 
将/api/public/emailList连接补充完整 让后部署绑定自定义域然后访问你的域名?token=你获取的token 
