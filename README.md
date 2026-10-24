# AqaraTwin - Web Demo / Bản xem thử trên web

## Tiếng Việt
AqaraTwin là bản sao số 3D của một ngôi nhà thông minh. Đây là **bản xem thử (Demo)** chạy trên trình duyệt:
- Dùng **dữ liệu mẫu**, không kết nối thiết bị thật, không cần tài khoản hay khóa API.
- Mã nguồn dự án không nằm trong kho này, chỉ có sản phẩm đã build.
- Phiên bản: commit `d25f89f`, build 2026-10-23 (UTC), Unity 6000.4.0f1, dung lượng nén 17.0 MB.

### Cập nhật
Thay toàn bộ tệp bằng nội dung mới của `Builds/WebGL-deploy` rồi đẩy lên kho này.

### GitHub Pages
Settings → Pages → Branch `main`, thư mục `/ (root)`. Tệp `.nojekyll` giữ GitHub không chạy Jekyll trên thư mục `Build/`.

### Vì sao bật decompression fallback
GitHub Pages không gửi tiêu đề `Content-Encoding` cho tệp nén sẵn, nên trình tải của Unity tự giải nén (Gzip) bằng JavaScript.

## English
AqaraTwin is a 3D digital twin of a smart home. This is the **Web Demo** build:
- It uses **sample data**: no connection to real devices, no account or API credentials.
- The project source is not in this repository, only the built output.
- Build: commit `d25f89f`, 2026-10-23 (UTC), Unity 6000.4.0f1, compressed size 17.0 MB.

### Updating
Replace all files with the new `Builds/WebGL-deploy` output and push to this repository.

### GitHub Pages
Settings -> Pages -> Branch `main`, folder `/ (root)`. `.nojekyll` stops GitHub from running Jekyll over `Build/`.

### Why decompression fallback is on
GitHub Pages sends no `Content-Encoding` header for pre-compressed files, so Unity's loader decompresses the Gzip files in JavaScript.

## Third-party notices
See `ATTRIBUTION.md` and `licenses/`.
