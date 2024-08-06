# Chỉ định hình ảnh cơ sở
FROM node:16

# Tạo thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép package.json và package-lock.json vào thư mục làm việc
COPY package*.json ./

# Cài đặt các phụ thuộc
RUN npm install

# Sao chép mã nguồn vào thư mục làm việc
COPY . .

RUN npm run build

RUN npm install -g serve

# Mở cổng cho ứng dụng
EXPOSE 5000

# Chạy ứng dụng khi container khởi động
CMD [ "serve", "-s", "-l", "5000", "build" ]