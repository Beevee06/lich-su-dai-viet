# Lịch sử Đại Việt

Website tĩnh đa trang với giao diện hiện đại (glassmorphism, nền tối), gồm:
- index.html (trang chủ, timeline, triều đại, anh hùng, văn hóa)
- events.html (carousel sự kiện)
- modern-history.html (Việt Nam hiện đại)
- kien-truc.html, van-hoc.html, nghe-thuat.html, my-thuat.html
- styles.css, script.js

## Triển khai bằng GitHub Pages
1. Tạo repo public trên GitHub.
2. Đẩy mã nguồn lên branch `main`.
3. Vào Settings → Pages → Source: chọn `main` và Folder: `/root`.
4. Site sẽ chạy tại: `https://<username>.github.io/<repo>/`.

## Lệnh Git (PowerShell)
```powershell
cd D:\histoy
git init
git add .
git commit -m "Publish site"
git branch -M main
# Cập nhật USER/REPO bên dưới trước khi chạy
git remote add origin https://github.com/USER/REPO.git
git push -u origin main
```

## Chạy thử cục bộ
```powershell
npx http-server -p 8000
# Mở http://localhost:8000
```

## Ghi chú
- `.nojekyll` đảm bảo Pages không dùng Jekyll.
- Các liên kết tương đối giữa các trang đã tương thích với đường dẫn `/repo/`.
- Có thể thêm domain riêng qua GitHub Pages nếu cần.
