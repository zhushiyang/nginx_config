# nginx_config
Nginx配置文件
# 添加了upsync支持

```
├── certs # 存放证书文件，目录名称也可以更换为ssl，修改主机配置文件即可
│   ├── zhushiyang.net.key
│   └── zhushiyang.net.pem
├── dump_upstreams # 存放upsync的dump upstream文件
├── fastcgi.conf
├── fastcgi.conf.default
├── fastcgi_params
├── fastcgi_params.default
├── koi-utf
├── koi-win
├── mime.types
├── mime.types.default
├── nginx.conf # nginx主配置文件
├── nginx.conf.default
├── proxy.conf
├── scgi_params
├── scgi_params.default
├── streams  # 四层转发配置目录，主机文件里面默认没有
│   └── vpn.zhushiyang.net.conf
├── upstreams  # 存放upstream的配置文件
│   └── web_cluster.conf # 不支持upsync的upstream配置
|   └── web_cluster_upsync.conf # 支持upsync，使用etcd存储数据的upstream示例配置
├── uwsgi_params
├── uwsgi_params.default
├── vhosts  # 七层转发配置目录
│   └── www.zhushiyang.net.conf
└── win-utf
```
