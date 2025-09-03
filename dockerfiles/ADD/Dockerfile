FROM almalinux
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/YadavEshNithin/practice_docker/refs/heads/main/dockerfiles/FROM/Dockerfile /usr/share/nginx/html/
RUN chmod -r +r  https://raw.githubusercontent.com/YadavEshNithin/practice_docker/refs/heads/main/dockerfiles/FROM/Dockerfile
ADD sample.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]