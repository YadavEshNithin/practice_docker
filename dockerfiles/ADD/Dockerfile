FROM almalinux
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/daws-84s/notes/refs/heads/main/session-01.txt /usr/share/nginx/html/
RUN chmod +r  /usr/share/nginx/html/
ADD sample.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]