FROM almalinux
RUN dnf install nginx -y 
RUN rm -rf /usr/share/nginx/html/index.html 
# COPY index.html /usr/share/nginx/html/
# COPY templatemo_591_villa_agency/ /usr/share/nginx/html/
ONBUILD COPY index.html /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]