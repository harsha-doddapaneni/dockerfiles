FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/harsha-doddapaneni/notes/refs/heads/main/session-01.txt?token=GHSAT0AAAAAADC6GNLCXKTS7NTAPELF6ATY2CJI7ZQ /usr/share/nginx/html/index.html
RUN chmod +x /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]