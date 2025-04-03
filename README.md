# Folder Cấu trúc dự án ReactJS (React + TypeScript + Vite)

```
📦src
┣ 📂Apis
┃ ┣ 📂Commons
┃ ┗ 📂Modules-a
┃ ┗ 📂Modules-b
┣ 📂Assets
┃ ┣ 📂Images
┃ ┗ 📂Icons
┣ 📂Components
┣ 📂Configs
┣ 📂Constants
┣ 📂Layouts
┣ 📂Middlewares
┣ 📂Pages
┃ ┣ 📂Admins
┃ ┣ 📂Clients
┃ ┃ ┣ 📂Module-a
┃ ┃ ┃ ┣ 📂_Components
┃ ┃ ┃ ┗ 📂_Contexts
┃ ┃ ┗ 📂Module-b
┃ ┗ 📂Login
┣ 📂Routes
┃ ┣ 📂RouteModules
┃ ┣ 📂RouteNavigates
┃ ┣ 📜privateRoutes.tsx
┃ ┗ 📜publicRoutes.tsx
┣ 📂Services
┃ ┣ 📂Hooks
┃ ┣ 📂Queries
┃ ┣ 📂Utils
┃ ┗ 📂Validations
┣ 📜App.css
┣ 📜App.tsx
┣ 📜index.css
┣ 📜main.tsx
┗ 📜vite-env.d.ts
```

## 📂 Apis

-   Chứa các hàm gọi API, giúp quản lý các request đến backend.

-   📂 Commons: Chứa các API chung, không thuộc module cụ thể nào. Ví dụ: API xử lý authentication, upload file, hoặc các API dùng chung trên toàn hệ thống.

-   📂 Modules-A, 📂 modules-b: Chứa các API đặc thù cho từng module cụ thể trong dự án.

## 📂 Assets

-   Chứa tài nguyên tĩnh như hình ảnh và icon.

-   📂 Images: Chứa ảnh nền, banner, logo, hoặc các hình ảnh khác được sử dụng trong UI.

-   📂 Icons: Chứa các biểu tượng SVG hoặc icon tĩnh được sử dụng trong dự án.

## 📂 Components

-   Chứa các component UI có thể tái sử dụng, độc lập với các page cụ thể.

-   Ví dụ: Button, Input, Modal, Table, Card, Tooltip...

## 📂 Configs

-   Chứa các cấu hình quan trọng của dự án như:

    -   Cấu hình http fetch api,

    -   Cấu hình biến hệ thống

    -   Cấu hình theme, global styles,

## 📂 Constants

-   Chứa các hằng số (constants) được sử dụng trong toàn bộ ứng dụng. Ví dụ:

    -   Các giá trị mặc định (DEFAULT_PAGE_SIZE, MAX_UPLOAD_SIZE).

    -   Các key lưu trữ trên localStorage.

    -   Các enum dùng trong logic ứng dụng.

## 📂 Layouts

-   Chứa các bố cục giao diện (layout) chung cho ứng dụng, giúp tái sử dụng UI cho nhiều trang.

-   Ví dụ:

    -   AdminLayout.tsx: Layout dành cho trang admin.

    -   ClientLayout.tsx: Layout dành cho người dùng.

    -   AuthLayout.tsx: Layout cho trang login.

## 📂 Middlewares

-   Chứa các middleware dùng để kiểm soát hành vi ứng dụng.

-   Ví dụ:

    -   Middleware kiểm tra quyền truy cập trước khi hiển thị một trang.

    -   Middleware xử lý lỗi API response.

    -   Middleware xác thực token.

## 📂 Pages

-   Chứa các trang của ứng dụng, tổ chức theo các nhóm người dùng hoặc module.

-   Ví dụ:

    -   📂 Admins: Chứa các trang dành cho quản trị viên.

    -   📂 Clients: Chứa các trang dành cho người dùng thông thường.

    -   📂 Module-a, 📂 module-b: Chia nhỏ theo từng module chức năng.

        -   📂 \_Components: Chứa các component chỉ dùng riêng cho module đó.

        -   📂 \_Contexts: Chứa các context API dùng trong module đó.

    -   📂 Login: Chứa trang đăng nhập, đăng ký, quên mật khẩu.

## 📂 Routes

-   Chứa các định nghĩa về route trong ứng dụng.

-   📂 RouteModules: Tổ chức các nhóm route theo module cụ thể.

-   📂 RouteNavigates: Chứa các hàm điều hướng, xử lý logic chuyển trang.

-   📜 privateRoutes.tsx: Chứa danh sách các route yêu cầu xác thực.

-   📜 publicRoutes.tsx: Chứa danh sách các route công khai.

## 📂 Services

-   Chứa các dịch vụ xử lý logic không liên quan đến UI.

-   📂 Hooks: Chứa các custom hooks dùng trong toàn bộ ứng dụng.

-   📂 Queries: Chứa các query React Query, giúp quản lý dữ liệu.

-   📂 Utils: Chứa các hàm tiện ích như format ngày tháng, xử lý chuỗi, debounce...

-   📂 Validations: Chứa các schema validation sử dụng với Yup hoặc Zod.

## 📂 Types

-   Chứa các định nghĩa type
