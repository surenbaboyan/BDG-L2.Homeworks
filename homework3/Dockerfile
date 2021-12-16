FROM nginx
RUN apt update -y && apt install python3
WORKDIR /app
COPY . .
RUN python3 gen_html.py
MV index.html /usr/share/nginx/html
