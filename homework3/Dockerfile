FROM nginx
RUN apt update && apt -y install python3
WORKDIR /app
COPY . .
RUN python3 gen_html.py
RUN mv index.html /usr/share/nginx/html
