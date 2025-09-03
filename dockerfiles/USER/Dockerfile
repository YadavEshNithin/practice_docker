FROM almalinux:9
RUN dnf install nginx -y 
RUN useradd sivasir
USER sivasir
CMD ["nginx", "-g", "daemon off;"]