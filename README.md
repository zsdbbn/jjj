镜像名为`mjjonone/mjj:amd64`，变量设置如下：容器的`SERVER_PORT`变量可设置为3000、7860等


!有些平台会检测关键词（比如render,huggingface)，可以使用打包好的Dockerfile文件解决，建议都Fork仓库再部署，防止封号。in red
!! 无法用github仓库部署的平台（比如huggingface），复制下面Dockerfile文件的内容，然后新建Dockerfile文件，要求内容一样

```
(https://github.com/mjjonone/mjj-docker)
---


在node.js环境中，`index.js`、`package.json` `start.sh`

在`start.sh`文件中填写变量信息。


- `NAME`：节点名称，默认ips。
- `CFIP`：优选IP或网址，默认icook.hk。
- `NEZHA_SERVER`：Nezha地址（如果没有可不填）。
- `NEZHA_PORT`：Nezha端口（如果没有可不填）。
- `NEZHA_KEY`：Nezha密匙（如果没有可不填）。
- `TLS`：默认为1，代表开启tls,如果不需要TLS，请将变量设置为0。
- `ARGO_DOMAIN`：隧道固定域名（如果没有可不填）。
- `ARGO_AUTH`：隧道的token或者json（如果没有可不填）。
- `WSPATH`：默认值为`argo`。
- `UUID`：默认值为`de04add9-5c68-8bab-950c-08cd5320df18`。
- `ARGO_AUTH`：隧道的值，请参考f佬的说明。
- 变量的填写方法也可以参考f佬的说明。

