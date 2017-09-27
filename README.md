# 維謢切換sop如下：
前台：
請編輯各SSH.conf檔，將$MAM 0改為1，再reload nginx服務即可

APP:
請編輯各nginx.conf檔，將incule原本vhost/*.conf Mark掉 ，並改為 include /opt/APP/openresty/nginx/conf/ma/*.conf;

