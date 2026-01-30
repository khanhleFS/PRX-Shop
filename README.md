# PRX Shop - Paper Rex Official Merchandise Store

## 📖 Giới thiệu

PRX Shop là cửa hàng bán lẻ chính thức của đội Paper Rex, một phần của mạng lưới sản phẩm IMPLS Entertainment. Đây là một ứng dụng e-commerce full-stack cho phép người dùng mua sắm các sản phẩm độc quyền của đội Paper Rex bao gồm áo đấu, áo thun, hoodie, phụ kiện và các bộ sưu tập đặc biệt.

**Website tham khảo:** [https://shop.pprx.team/](https://shop.pprx.team/)

## ✨ Tính năng chính

### Sản phẩm
- **Team Kit**: Áo đấu chính thức của đội (DinoMarine, Raptor, v.v.)
- **Collections**: 
  - PRX Seoul Mission 2025
  - PRX Basics
  - PRX Accessories
- **Collaborations**: Hợp tác với các thương hiệu như EDG, Pulsar, EPT, Secretlab
- **Danh mục sản phẩm**: T-Shirts, Hoodies & Sweatshirts, Jackets, Gift Ideas

### Tính năng E-commerce
- Duyệt và tìm kiếm sản phẩm
- Giỏ hàng và thanh toán
- Hỗ trợ đa quốc gia và đa tiền tệ
- Miễn phí vận chuyển cho đơn hàng trên SGD $100
- Đăng ký newsletter với ưu đãi 10% cho đơn hàng đầu tiên
- Quản lý tài khoản người dùng

## 🛠️ Công nghệ sử dụng

### Backend
- **Framework**: Spring Boot 4.0.2
- **Language**: Java 21
- **Database**: Microsoft SQL Server
- **ORM**: Spring Data JPA
- **Security**: Spring Security
- **Validation**: Spring Validation
- **Build Tool**: Maven
- **Libraries**: 
  - Lombok
  - Spring Boot DevTools

### Frontend
- **Framework**: React 19.2.0
- **Build Tool**: Vite 7.2.4
- **UI Library**: Material-UI (MUI) 7.3.7
- **Routing**: React Router DOM 6.30.3
- **HTTP Client**: Axios 1.13.4
- **Styling**: Emotion (CSS-in-JS)
- **Icons**: Material-UI Icons

## 📁 Cấu trúc dự án

```
PRX-Shop/
├── backend/                 # Spring Boot Backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── Khanhle/Shop/
│   │   │   │       └── PrxShopApplication.java
│   │   │   └── resources/
│   │   │       ├── application.properties
│   │   │       ├── static/
│   │   │       └── templates/
│   │   └── test/
│   ├── pom.xml
│   └── mvnw
│
├── frontend/                # React Frontend
│   ├── src/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── main.jsx
│   │   ├── index.css
│   │   └── assets/
│   ├── public/
│   ├── package.json
│   ├── vite.config.js
│   └── eslint.config.js
│
└── README.md
```

## 🚀 Cài đặt và chạy dự án

### Yêu cầu hệ thống
- **Java**: JDK 21 trở lên
- **Node.js**: phiên bản 18 trở lên
- **Maven**: 3.6+ (hoặc sử dụng Maven Wrapper)
- **SQL Server**: Microsoft SQL Server (hoặc SQL Server Express)

### Backend Setup

1. **Di chuyển vào thư mục backend:**
   ```bash
   cd backend
   ```

2. **Cấu hình database trong `application.properties`:**
   - Cập nhật thông tin kết nối SQL Server (URL, username, password)

3. **Chạy ứng dụng Spring Boot:**
   ```bash
   # Windows
   ./mvnw.cmd spring-boot:run
   
   # Linux/Mac
   ./mvnw spring-boot:run
   ```
   
   Hoặc sử dụng Maven trực tiếp:
   ```bash
   mvn spring-boot:run
   ```

4. Backend sẽ chạy tại: `http://localhost:8080` (mặc định)

### Frontend Setup

1. **Di chuyển vào thư mục frontend:**
   ```bash
   cd frontend
   ```

2. **Cài đặt dependencies:**
   ```bash
   npm install
   ```

3. **Chạy development server:**
   ```bash
   npm run dev
   ```

4. Frontend sẽ chạy tại: `http://localhost:5173` (mặc định Vite)

### Build cho Production

**Backend:**
```bash
cd backend
./mvnw clean package
java -jar target/Shop-0.0.1-SNAPSHOT.jar
```

**Frontend:**
```bash
cd frontend
npm run build
```
Files build sẽ được tạo trong thư mục `dist/`

## 📝 API Endpoints

*(Cần cập nhật khi backend được phát triển)*

Dự kiến các endpoints:
- `GET /api/products` - Lấy danh sách sản phẩm
- `GET /api/products/{id}` - Lấy chi tiết sản phẩm
- `POST /api/cart` - Thêm vào giỏ hàng
- `GET /api/cart` - Lấy giỏ hàng
- `POST /api/orders` - Tạo đơn hàng
- `POST /api/auth/login` - Đăng nhập
- `POST /api/auth/register` - Đăng ký

## 🎨 Giao diện

Dự án sử dụng Material-UI để tạo giao diện hiện đại và responsive, phù hợp với thương hiệu Paper Rex. Các thành phần UI chính bao gồm:
- Header với navigation menu
- Product grid/cards
- Shopping cart
- Checkout flow
- User account management

## 🔒 Bảo mật

- Spring Security được tích hợp để xử lý authentication và authorization
- Validation được áp dụng cho các input từ người dùng
- CORS được cấu hình để cho phép frontend giao tiếp với backend

## 📦 Sản phẩm nổi bật

Dựa trên website chính thức, các sản phẩm bao gồm:
- **PRX Official Match Jersey 2026/27 DinoMarine** - Áo đấu mới nhất
- **PRX Official Match Jersey 2025/26 Raptor** - Áo đấu bestseller
- **PRX Windbreaker** - Áo khoác gió
- **PRX Zip Hoodie** (Black/Grey) - Áo hoodie có khóa kéo
- **PRX Seoul Mission Collection** - Bộ sưu tập đặc biệt
- **PRX Basics** - Dòng sản phẩm cơ bản
- **PRX Accessories** - Phụ kiện (lanyard, sticker pack, card holder, plushie)

## 🌍 Hỗ trợ đa quốc gia

Website hỗ trợ nhiều quốc gia và tiền tệ, bao gồm:
- Singapore (SGD)
- United States (USD)
- United Kingdom (GBP)
- Và nhiều quốc gia khác...

## 🤝 Đóng góp

Dự án này đang trong giai đoạn phát triển. Mọi đóng góp đều được chào đón!

## 📄 License

*(Cần cập nhật license phù hợp)*

## 📧 Liên hệ

- **Website chính thức**: [https://shop.pprx.team/](https://shop.pprx.team/)
- **About Us**: Paper Rex Shop là cửa hàng merch chính thức của đội Paper Rex

---

**Note**: Đây là dự án clone/inspiration của Paper Rex Shop. Để mua sản phẩm chính thức, vui lòng truy cập [shop.pprx.team](https://shop.pprx.team/)
