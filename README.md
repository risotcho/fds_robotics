## Quy tắc chung cho repo này!

📘 I. Quy tắc về việc viết code (Coding Guidelines)

1. Đặt tên rõ ràng và nhất quán
	•	Tên biến, hàm, class phải có ý nghĩa rõ ràng, dễ hiểu.
	•	Sử dụng camelCase cho biến/hàm, PascalCase cho class, UPPER_SNAKE_CASE cho hằng số.
	•	Không dùng viết tắt trừ khi thực sự phổ biến (VD: id, url, html).

2. Tuân thủ chuẩn code (Coding Style)
	•	Sử dụng chuẩn style phù hợp với ngôn ngữ (VD: PEP8 cho Python, PSR cho PHP, Airbnb cho JavaScript).
	•	Format code rõ ràng: indent, dấu cách, xuống dòng hợp lý.
	•	Dùng công cụ tự động format như Prettier, Black, ESLint, …

3. Không hard-code
	•	Tránh ghi giá trị cố định vào code, hãy sử dụng biến, config, hoặc hằng số.

4. Viết comment hợp lý
	•	Chỉ comment khi cần thiết (giải thích logic phức tạp hoặc lý do đặc biệt).
	•	Không lạm dụng comment.

5. Viết code dễ đọc hơn code ngắn
	•	Ưu tiên code dễ đọc, dễ hiểu hơn code tối ưu về ký tự.

6. Tách biệt chức năng
	•	Một hàm chỉ nên làm một việc duy nhất.
	•	Tách module hợp lý theo chức năng (VD: controller, service, model…).

7. Xử lý lỗi đầy đủ
	•	Bắt và xử lý ngoại lệ, không để app crash đột ngột.
	•	Ghi log rõ ràng, tránh ghi quá nhiều hoặc thiếu thông tin.

⸻

📦 II. Quy tắc cập nhật phiên bản code (Versioning Guidelines)

1. Tuân thủ Semantic Versioning (SemVer): MAJOR.MINOR.PATCH
	•	MAJOR: thay đổi lớn, có thể phá vỡ tương thích cũ.
	•	MINOR: thêm tính năng mới, vẫn tương thích.
	•	PATCH: sửa lỗi, không thay đổi API.

Ví dụ:
	•	1.4.0 → thêm tính năng mới.
	•	1.4.2 → sửa lỗi nhỏ.
	•	2.0.0 → thay đổi lớn không tương thích với bản 1.x.

2. Mỗi commit phải có message rõ ràng
	•	Dùng định dạng thống nhất (VD: Conventional Commits):
	•	feat: thêm tính năng login
	•	fix: sửa lỗi khi đăng ký
	•	refactor: cải tổ code không ảnh hưởng logic
	•	docs: cập nhật README
	•	chore: cấu hình CI/CD

3. Không commit trực tiếp vào nhánh chính
	•	Luôn tạo nhánh riêng (feature/bugfix/hotfix), mở Pull Request (PR).
	•	PR cần được review trước khi merge.

4. Ghi chú thay đổi (CHANGELOG)
	•	Cập nhật file CHANGELOG.md cho mỗi phiên bản chính thức.
	•	Ghi rõ những gì đã thay đổi, thêm, sửa, xóa.
