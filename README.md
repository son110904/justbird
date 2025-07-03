# JustBird 

Một phiên bản đơn giản của trò chơi Flappy Bird được viết bằng Python và Pygame.

## Mô tả

JustBird là một trò chơi arcade đơn giản nơi bạn điều khiển một con chim bay qua các ống dẫn. Mục tiêu là bay càng xa càng tốt mà không va chạm vào các chướng ngại vật.

## Tính năng

-  Gameplay đơn giản, dễ hiểu
-  Đồ họa pixel art đẹp mắt
-  Âm thanh hiệu ứng 
-  Điều khiển đơn giản chỉ với một phím
-  Hoạt ảnh mượt mà cho chim và môi trường

## Yêu cầu hệ thống

- Python 3.x
- Pygame

## Cài đặt

1. Clone repository:
```bash
git clone https://github.com/yourusername/justbird.git
cd justbird
```

2. Cài đặt Pygame:
```bash
pip install pygame
```

3. Đảm bảo có đủ các file assets trong thư mục `assets/`:
```
assets/
├── sprites/
│   ├── bluebird-upflap.png
│   ├── bluebird-midflap.png
│   ├── bluebird-downflap.png
│   ├── pipe-green.png
│   ├── base.png
│   ├── background-day.png
│   └── message.png
└── audio/
    ├── wing.wav
    └── hit.wav
```

## Cách chơi

1. Chạy game:
```bash
python flappy.py
```

2. Điều khiển:
   - **Phím Space** hoặc **Phím mũi tên lên**: Làm chim bay lên
   - **ESC**: Thoát game

3. Luật chơi:
   - Điều khiển chim bay qua các khe hở giữa các ống dẫn
   - Tránh va chạm vào ống dẫn hoặc mặt đất
   - Game kết thúc khi chim va chạm vào chướng ngại vật

## Cấu trúc code

- `Bird`: Class điều khiển chim với animation và physics
- `Pipe`: Class tạo các ống dẫn (cả trên và dưới)
- `Ground`: Class tạo mặt đất di chuyển
- Collision detection sử dụng pygame mask để có độ chính xác cao

## Tùy chỉnh

có thể điều chỉnh các thông số trong phần VARIABLES:

```python
SCREEN_WIDHT = 400      # Chiều rộng màn hình
SCREEN_HEIGHT = 600     # Chiều cao màn hình
SPEED = 20              # Tốc độ bay lên của chim
GRAVITY = 2.5           # Trọng lực
GAME_SPEED = 15         # Tốc độ di chuyển của game
PIPE_GAP = 150          # Khoảng cách giữa các ống dẫn
```

## Đóng góp

Mọi đóng góp đều được hoan nghênh, Hãy tạo pull request hoặc mở issue để báo cáo lỗi.


*Lưu ý: Đây là một dự án học tập được lấy cảm hứng từ trò chơi Flappy Bird gốc.*
