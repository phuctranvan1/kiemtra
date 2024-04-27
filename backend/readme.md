# LƯU Ý
## Cài đặt SQL cho NHÀ PHÁT TRIÊN
- Mở VSCODE 2022:
    - Đổi tên `appsettings.Development_Example.json` thành `appsettings.Development.json`
    - Thêm `connection-string ` của bạn vào đó
    - Mở package manager console
    - `add-migration [TÊN CỦA THAY ĐỔI]`
    - `update-database`

## THÊM USER VÀO CSDL
- Cần thêm tài khoản ở Swagger
    - Thêm ROLE bằng cổng 'seed-role'
    - Tạo 1 User ở sign-in
    - Đăng nhập bằng user đó
    - Lấy token rồi thêm nó vò Author...
    - Test API thoải mái
# Todo
## Hướng dẫn lấy modal từ CSDL
```powershell
scaffold-dbcontext "Data Source=localhost\\sqlexpress;Initial Catalog=BACKEND_CRM;User ID=sa;Password=123;Encrypt=True;Trust Server Certificate=True" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -ContextDir Contexts -force
```
