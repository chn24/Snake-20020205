# Snake-20020205
* Các thư viện đã dùng:
      - SDL2: https://www.libsdl.org/download-2.0.php
      - 
      - SDL2_ttf : https://www.libsdl.org/projects/SDL_ttf/ (thư viện tải font chữ)
      - 
      - SDL2_mixer : https://www.libsdl.org/projects/SDL_mixer/ (thư viện tải âm thanh)
      - 
* Thuật toán :
      -Thuật toán di chuyển được dựa trên code Key Bord của thầy Hiếu
      - Con rắn và mồi sẽ được đánh dấu vào mảng 2 chiều a[39][29] với  :
                + a[x][y]=1 ứng với phần đầu của rắn
                + a[x][y]=2 ứng với phần thân của con rắn
                + a[x][y]=4 ứng với con mồi
                + a[x][y]=0  là ô đấy không chứa gì cả
      - Mỗi bước di chuyển sẽ xóa phần đuôi, vẽ thêm phần đầu ở vị trí ô tương ứng, đổi màu ô thân thứ 2(ngay sau phần đầu) về màu đen(màu của phần thân con rắn), các phần thân còn lại dữ nguyên;  
      các phần thân còn lại dữ nguyên; nếu con rắn ăn mồi sẽ ko xóa ô đuôi con rắn
      - Khi bắt đầu hoặc lúc con rắn ăn được mồi, môi mới sẽ được random 1 vị trí mói, nếu ở vị trí đó đã có tương ứng với 1 phần con rắn thì sẽ random đến lúc nào có vị trí thích hợp.
* Di chuyển : 
       Dùng các phím lên, xuống, trái, phải để di chuyển con rắn
               (con rắn chưa tự du chuyển )
