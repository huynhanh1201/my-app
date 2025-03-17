# Hướng Dẫn Clone và Chạy Dự Án Expo

## Yêu Cầu Môi Trường

Để chạy được dự án, cần đảm bảo môi trường phát triển có các yêu cầu sau:

- **Node.js** phiên bản **v22.12.0**
- **Git** để clone repository
- **Expo CLI** và **EAS CLI**
- **Thiết bị Android hoặc trình giả lập**

## Hướng Dẫn Cài Đặt

### 1. Clone repository

```sh
git clone <repository-url>
cd <project-folder>
```

### 2. Cài đặt các dependencies

```sh
npm install
```

### 3. Cài đặt EAS CLI (nếu chưa có)

```sh
npm install -g eas-cli
```

### 4. Đăng nhập vào Expo

- Nếu chưa có tài khoản, đăng ký tại: [Expo Sign Up](https://expo.dev/signup)
- Đăng nhập bằng lệnh:

```sh
eas login
```

### 5. Cấu hình EAS cho dự án (chạy lệnh trong terminal dự án)

```sh
eas build:configure
```

### 6. Tạo bản build phát triển

```sh
eas build --platform android --profile development
```

### 7. Cài đặt bản build trên thiết bị

- Sau khi build hoàn tất, quét mã QR trong terminal hoặc mở link trên thiết bị.
- Nhấn **Install** để tải về và **Open** để cài đặt.

## Lưu Ý

- Nếu gặp lỗi liên quan đến quyền truy cập, kiểm tra xem bạn đã đăng nhập đúng tài khoản Expo chưa.
- Nếu build thất bại, thử chạy `eas build:inspect` để kiểm tra lỗi chi tiết.
- Nếu dùng thiết bị thật, bật **Developer Mode** và **USB Debugging** trong cài đặt điện thoại.

## Liên Hệ Hỗ Trợ

Nếu có bất kỳ vấn đề gì, liên hệ với nhóm phát triển hoặc kiểm tra tài liệu tại: 
[Expo Docs](https://docs.expo.dev/get-started/set-up-your-environment/?mode=development-build).# my-app
