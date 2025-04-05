<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Tiệm Gạo</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper/swiper-bundle.min.css"/>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/js/all.min.js"></script>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f4f4f4;
    }

    header {
      background-color: #441752;
      color: white;
      padding: 30px;
      text-align: center;
      font-size: 48px;
      font-family: 'Pacifico', cursive;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    nav {
      background-color: #fff;
      border-bottom: 1px solid #ccc;
      padding: 15px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .menu-icon {
      font-size: 30px;
      cursor: pointer;
      color: #333;
    }

    .nav-center {
      display: flex;
      align-items: center;
      gap: 25px;
      margin-left: 20px;
    }

    .nav-center a {
      text-decoration: none;
      color: #333;
      font-weight: bold;
      font-size: 20px;
      transition: color 0.3s;
    }

    .nav-center a:hover {
      color: #FF69B4;
    }

    .search-bar {
      display: flex;
      align-items: center;
      background-color: #f1f1f1;
      padding: 8px 15px;
      border-radius: 20px;
      flex-grow: 1;
      max-width: 500px;
      margin: 10px;
      position: relative;
    }

    .search-bar i.fa-search {
      margin-right: 10px;
      color: gray;
      font-size: 15px;
    }

    .search-bar input {
      border: none;
      background: transparent;
      outline: none;
      flex-grow: 1;
      font-size: 16px;
    }

    .search-bar i.fa-camera {
      margin-left: 15px;
      color: gray;
      cursor: pointer;
      font-size: 18px;
    }

    .icons-right i {
      font-size: 20px;
      color: #333;
      margin-left: 20px;
      cursor: pointer;
    }

    .category {
      margin: 30px 20px;
      padding: 20px;
      background-color: white;
      border-radius: 5px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    .category h2 {
      color: #FF69B4;
      border-left: 5px solid #FF69B4;
      padding-left: 10px;
      font-size: 28px;
      margin-bottom: 20px;
    }

    .swiper-container {
      position: relative;
      padding: 20px 0;
    }

    .swiper-slide {
      width: 280px !important;
      height: 300px;
      background: white;
      border-radius: 5px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      text-align: center;
      padding: 15px;
      box-sizing: border-box;
      transition: transform 0.3s;
      margin: 0 20px;
    }

    .swiper-slide:hover {
      transform: scale(1.05);
    }

    .swiper-slide img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 5px;
    }

    .swiper-button-next,
    .swiper-button-prev {
      width: 50px;
      height: 50px;
      background: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
      transition: background 0.3s;
      font-size: 24px;
      color: #FF69B4;
    }

    .swiper-button-next:hover,
    .swiper-button-prev:hover {
      background: #FF69B4;
      color: white;
    }

    footer {
      background-color: #333;
      color: white;
      padding: 15px;
      text-align: center;
      font-size: 14px;
    }

    /* Gallery styles */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
      padding: 20px;
    }
    .gallery img {
      width: 320px;
      border: 1px solid #ccc;
      border-radius: 10px;
      padding: 5px;
      box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }

    /* Tạo hiệu ứng cho menu */
    .menu-icon {
      cursor: pointer;
    }

  </style>
</head>
<body>

  <header>Tiệm Gạo</header>

  <nav>
    <i class="fas fa-bars menu-icon" onclick="toggleMenu()"></i>

    <div class="nav-center">
      <a href="#home">Trang chủ</a>
      <a href="#featured-products">Sản phẩm</a>
    </div>

    <div class="search-bar">
      <i class="fas fa-search"></i>
      <input type="text" placeholder="Tìm sản phẩm...">
      <i class="fas fa-camera"></i>
    </div>

    <div class="icons-right">
      <i class="fas fa-shopping-cart"></i>
    </div>
  </nav>

  <!-- Danh mục 1 -->
  <div class="category" id="featured-products">
    <h2>Sản phẩm nổi bật</h2>
    <div class="swiper-container swiper1">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/J0FXcNs6/Messenger-creation-D12-D46-B7-7-ADB-438-F-82-DA-6704435-EF3-C0.jpg" alt="Sản phẩm 1">
          <h4>Móc khóa</h4>
          <p style="color: red;">20.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/RhW6FWgc/Messenger-creation-B760-FA82-FF48-47-AF-B9-EE-9-FE5-D0114-D7-A.jpg" alt="Sản phẩm 2">
          <h4>Washi tape</h4>
          <p style="color: red;">85.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/25YZw85D/Messenger-creation-AF4977-F1-6-D0-A-473-F-A31-A-923-B91-C3-E3-D4.jpg" alt="Sản phẩm 3">
          <h4>Cây móc len</h4>
          <p style="color: red;">12.000 VNĐ</p>
        </div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </div>

  <!-- Danh mục 2 -->
  <div class="category" id="accessories">
    <h2>Phụ kiện</h2>
    <div class="swiper-container swiper2">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/J0FXcNs6/Messenger-creation-D12-D46-B7-7-ADB-438-F-82-DA-6704435-EF3-C0.jpg" alt="Sản phẩm 1">
          <h4>Móc khóa</h4>
          <p style="color: red;">20.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/d0R8PZf3/Messenger-creation-46-FB549-E-BAA7-44-E2-8-B62-29-DEC7-AB16-F5.jpg" alt="Len">
          <h4>Vòng tay</h4>
          <p style="color: red;">35.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/cLw3w80h/Messenger-creation-1-D53-E5-F5-0-F79-4-B35-9-A38-56-A1-E31-DF0-CE.jpg" alt="Cây móc len">
          <h4>Móc điện thoại</h4>
          <p style="color: red;">30.000 VNĐ</p>
        </div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </div>

  <!-- Danh mục 3 -->
  <div class="category" id="materials">
    <h2>Nguyên liệu</h2>
    <div class="swiper-container swiper3">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/T2Nn66tV/Messenger-creation-907-E39-B0-1-B66-4617-9121-7-E89164-B32-EE.jpg" alt="Móc khóa">
          <h4>Len</h4>
          <p style="color: red;">30.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/25YZw85D/Messenger-creation-AF4977-F1-6-D0-A-473-F-A31-A-923-B91-C3-E3-D4.jpg" alt="Sản phẩm 3">
          <h4>Cây móc len</h4>
          <p style="color: red;">25.000 VNĐ</p>
        </div>
        <div class="swiper-slide">
          <img src="https://i.postimg.cc/bNGkYB5K/Messenger-creation-162043-DC-90-BD-43-DC-8679-0437767-F574-F.jpg" alt="Bộ thủ công">
          <h4>Gấu bông</h4>
          <p style="color: red;">100.000 VNĐ</p>
        </div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </div>

  <footer>
    <p>&copy; Kim Thy 12D6 | Địa chỉ Lý Thường Kiệt, trường THPT Nguyễn Du, Tân Phú, Đồng Xoài, Bình Phước.</p>
  </footer>

</body>
</html>
