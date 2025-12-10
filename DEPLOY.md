# Hướng dẫn Deploy lên Vercel

## Cách 1: Deploy qua Vercel Dashboard (Khuyên dùng)

1. **Đăng nhập Vercel:**
   - Truy cập https://vercel.com
   - Đăng nhập bằng GitHub/Google/GitLab

2. **Push code lên GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <your-github-repo-url>
   git push -u origin main
   ```

3. **Import project trên Vercel:**
   - Click "Add New Project"
   - Chọn repository vừa push
   - Vercel sẽ tự động detect và deploy
   - Click "Deploy"

4. **Xong!** Website sẽ có URL dạng: `https://your-project.vercel.app`

## Cách 2: Deploy qua Vercel CLI

1. **Cài đặt Vercel CLI:**
   ```bash
   npm install -g vercel
   ```

2. **Deploy:**
   ```bash
   vercel
   ```
   
   - Lần đầu sẽ yêu cầu đăng nhập
   - Chọn các tùy chọn theo hướng dẫn
   - Production: `vercel --prod`

3. **Xem kết quả:**
   - URL sẽ hiển thị sau khi deploy xong

## Lưu ý:

- Tất cả file HTML, CSS, JS và hình ảnh sẽ được deploy tự động
- Vercel hỗ trợ HTTPS miễn phí
- Mỗi lần push code lên GitHub, Vercel sẽ tự động deploy lại (nếu đã kết nối)

