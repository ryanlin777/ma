# 維謢切換sop如下：
先update git上面的網頁維謢時間內容
再用wget將所有網頁更新至前台及app
更新方式如下：


前台：
請編輯各SSH.conf檔，將$MAM 0改為1，再reload nginx服務即可

APP:
請編輯各nginx.conf檔，將incule原本vhost/*.conf Mark掉 ，並改為 include /opt/APP/openresty/nginx/conf/ma/*.conf; ，再reload nginx服務

