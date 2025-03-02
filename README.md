# Cách viết blog 1 cách chi tiết nhất


### Bước 1: Tạo 1 thư mục mới đặt tên tóm tắt nội dung blog đang viết gì

Ví dụ:
```
top-dia-diem-hue-check-in
```
Đây là 1 thư mục dành cho blog viết về những địa điểm check-in ở Huế. Trong thư mục này nên chứa tất cả các hình ảnh, video (không khuyến khích vì yêu cầu web bộ nhớ có hạn), ...

<br>

Sau đó phải tạo 1 file `index.html` nằm trong thư mục đó và làm dưới dạng mẫu sau:
<br>
[Template file](https://github.com/TrendBattles/travel-blogs/blob/master/template.html)


### Bước 2: Làm quen format 1 blog
- Điều đầu tiên là cần chỉnh tiêu đề của trang nằm ở:

```html
<!DOCTYPE html5>

<head>
    <title></title>
    ....
</head>
....
```
<br>

Mình để ý ở trong [file CSS có sẵn](https://github.com/TrendBattles/travel-blogs/blob/master/style.css), ở mấy dòng đầu có xuất hiện các class như:

```
.text-red, .text-yellow, .text-green, ...
.text-justify, .text-center, .text-left, .text-right
.medium-size, .small-size
```
- Đây là những class giúp thực hiện trong việc định dạng màu chữ, hướng của chữ và kích cỡ chữ (mà không cần quá đắn đo về sự phù hợp của nó trong web).


### Bước 3: Thêm nội dung vào
- Nên nhớ mọi nội dung mình thêm vào chỉ được phép trong phạm vi:
```html
<div class = "blog-box quicksand">
  <!-- Nội dung chính sẽ được viết ở trong này-->

  <div class = "text-right text-green medium-size">
    <em>
      Updated: <!-- Chỗ này là update thời gian lần cuối-->
    </em>
  </div>
</div>
```
- Để thêm được 1 block nội dung **chữ** mới vào thì mình sẽ thêm vào như sau:
```html
<div class = "text medium-size">
      <h1>....</h1>

      <br> <!-- nhớ thêm vào nếu như cần 1 khoảng hở giữa các dòng chữ -->

      <h3>....</h3>

      <br>

      <p>...</p>
</div>
```
- Thường thì các phần nội dung **chữ** sẽ ở kích cỡ chữ bình thường và ở trạng thái cân đối hai bên, tag ```<h1>``` đến ```<h6>``` dành cho mục lớn và ```<p>``` dành cho chi tiết nội dung mục đó.

<br>

Tuy nhiên, trong 1 số trường hợp, nếu như muốn chỉnh 1 số định dạng cho nội dung mình điền vào thì mình có thể thêm vào các class cho ```<h1>``` đến ```<h6>``` và ```<p>``` để phù hợp với cách mình muốn phân bố nội dung.

<br>

Ví dụ:
```html
<div class = "text medium-size">
  <h1 class = "text-orange text-right">
    1. Sông Hương – địa điểm chụp ảnh áo dài đẹp ở Huế
  </h1>

  <br>

  <p>
    <b class = "text-red">Địa chỉ:</b> trục đường Trần Hưng Đạo và Lê Lợi, trung tâm thành phố Huế
  </p>
</div>
```
**Thêm vào là sẽ thấy được hiệu ứng liền**

<br>

- Để thêm 1 block nội dung phi văn bản (hình ảnh, video, ...) thì có thể thêm như sau:
```html
Image:
<div class = "attachment text-center small-size">   
    <img src = "./<tên file>" alt = "Image not found">
</div>

Video:
<div class = "attachment text-center small-size">   
    <video src = "./<tên file>" alt = "Video not found">
</div>

iframe (đặc biệt, thường là iframe ở các trang ngoài sẽ định dạng giúp mình sẵn rồi):
<div class = "attachment text-center small-size">   
    <iframe src = "...">
</div>
```
Nhớ thêm định dạng ```width = "100%" height = "60%"``` đối với iframe.
<br>
Mục đích: Thêm nội dung phi văn bản với kich cỡ chữ nhỏ, căn giữa để chú thích (có thể tự điều chỉnh các class có sẵn để định dạng phù hợp).

<br> <br>
### Note: Nếu đến đây vẫn chưa hình dung được cách viết như nào thì có thể ghé thăm [Blog Test](https://github.com/TrendBattles/travel-blogs/blob/master/blog-frame-test)
### Mẫu để check tính năng: [Here](https://trendbattles.github.io/travel-blogs/blog-frame-test/)


# Additional:
Ở phần đầu mọi người sẽ thấy ```<meta>``` đang bị bỏ trống thì mọi người cứ để yên như vậy nhé, có gì admin sẽ dựa vào blog đang viết để thêm vào phù hợp.
<br>
Nếu ai hỏi nó dùng để làm gì thì khi gửi link sẽ xuất hiện thông tin cần thiết theo cái ```<meta>``` đó đã được setup cho từng trang web.
