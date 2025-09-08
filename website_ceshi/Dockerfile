FROM nginx:alpine

# 复制网站文件到nginx默认目录
COPY index.html /usr/share/nginx/html/
COPY style.css /usr/share/nginx/html/
COPY script.js /usr/share/nginx/html/
COPY photo /usr/share/nginx/html/photo

# 复制自定义nginx配置
COPY nginx.conf /etc/nginx/conf.d/default.conf

# 暴露端口80
EXPOSE 80

# 启动nginx
CMD ["nginx", "-g", "daemon off;"]