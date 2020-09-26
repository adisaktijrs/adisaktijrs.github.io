---
title: post-b
date: 2020-09-25 17:41:29
tags:
---

##### Code yang digunakan
Ini merupakan code yang harus disisipkan ke dalam

{% codeblock lang:js %}
var _self = (typeof window !== 'undefined')
	? window   // if in browser
	: (
		(typeof WorkerGlobalScope !== 'undefined' && self instanceof WorkerGlobalScope)
		? self // if in worker
		: {}   // if in node js
	);
  
server{
    listen 443;
    server_name xxoo.lol;
    ssl on;
    ssl_certificate /usr/local/nginx/conf/vhost/ca/xxoo.lol.crt;
    ssl_certificate_key /usr/local/nginx/conf/vhost/ca/xxoo.lol.key;
    ssl_protocols SSLv3 TLSv1;
    ssl_ciphers ALL:-ADH:+HIGH:+MEDIUM:-LOW:-SSLv2:-EXP;

    location / {
        proxy_redirect off;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto https;
        proxy_pass https://www.google.com.hk;
    }
}
{% endcodeblock %}
