# Sử dụng Node.js 18 làm base image
FROM node:18

# Thiết lập thư mục làm việc trong container
WORKDIR /app

# Sao chép file package.json và package-lock.json (nếu có)
COPY package*.json ./

# Cài đặt dependencies
RUN npm install

# Sao chép toàn bộ source code vào container
COPY . .

# Mở cổng 3000
EXPOSE 3000

# Chạy ứng dụng khi container khởi động
CMD ["node", "server.js"]
 
