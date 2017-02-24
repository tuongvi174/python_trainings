##Task 1
------------------------
>Người thực hiện: Hồ Nguyễn Tường Vi
>
>Tên tài liệu: 
 + [http://bit.ly/2cxplkv](https://github.com/hocchudong/git-github-for-sysadmin#ngonngumarkdown)
 + [http://bit.ly/2cxrr2B](https://help.ghost.org/hc/en-us/articles/224410728-Markdown-Guide)
 + [https://vi.wikipedia.org/wiki/Markdown](https://vi.wikipedia.org/wiki/Markdown)
 >
 >Ngày cập nhật: 25/02/2017
 >
 ----------------------------
##Mục lục: 

 [1. Github là gì? Dùng để làm gì?](#1)

 [2. Tạo repository đặt tên là python_trainings](#2)

 [3. Markdown là gì? Dùng để làm gì?](#3)

 [4. Các cú pháp thường gặp](#4)

 [5. Cài đặt Sublime Text và tìm kiếm, cài đặt các công cụ hỗ trợ markdown (export HTML, markdown preview, ...)](#5)

 [6. Các công cụ viết Markdown khác](#6)

##Nội dung:

####1. Github là gì? Dùng để làm gì?<a name="1"></a>

**Github là gì?**

<img src="http://i.imgur.com/Mbyi3bK.png">

>Git là một phần mềm dùng để quản lý phiên bản của mã nguồn tương tự như SVN nhưng có nhiều ưu điểm hơn, Git đang được sủ dụng rộng rãi hiện nay.
>Lấy ví dụ, bạn có một đoạn script dài 20 dòng, hôm sau bạn tối ưu nó đi, chỉ còn 15 dòng, một ngày khác bạn sửa ở script đó một vài chỗ. Git ghi lại những thời điểm thay đổi đó của bạn và source code của bạn tại thời điểm đó.

Github là một trang web, cho phép bạn lưu source code của mình lên đó. Sự kết hợp hoàn hảo giữa Git và Github mang lại một sự thuận tiện không hề nhỏ cho người dùng. Bạn có thể thay đổi đoạn code của mình mọi lúc mọi nơi mà không sợ bị ghi đè lên hay bị mất dữ liệu do hỏng hóc vì dữ liệu của bạn được lưu cả trên trang web Github và máy cá nhân. Bạn cũng có thể khôi phục được code của mình về một thời điểm bất kỳ nào đó.

Github có bản free và mất phí. Với Github free thì source code của bạn sẽ công khai, có nghĩa là ai cũng có thể xem code của bạn. Nó phù hợp với các phần mềm nguồn mở, và cũng có thể trở thành một blog cá nhân của chính các bạn như các trang blogspot, wordpress,...

Muốn có thể tạo một kho code bí mật của riêng mình thì bạn phải trả phí.

Đối với cá nhân tôi thì github free là quá đủ cho mục đích lưu trữ và chia sẻ thông tin.

**Github dùng để làm gì?**

Github chủ yếu được sử dụng để lưu trữ mã nguồn phần mềm, nhưng cũng thường được sử dụng với nhiều loại tập tin như Final Cut hoặc các tài liệu Word.

Ngoài mã nguồn, Github hỗ trợ các định dạng và các tính năng sau đây:

<ul>
<li>3D làm cho các tập tin mà có thể được xem trước bằng cách sử dụng tích hợp trình xem file STL mới hiển thị các tập tin trên một khung 3D. Người xem được hỗ trợ bởi WebGL và Three.js.</li>

<li>Nguồn gốc định dạng PSD của Photoshop có thể được xem trước và so với các phiên bản trước của cùng một tập tin.</li>

<li>Lồng nhiệm vụ danh sách.</li>

<li>Tài liệu và Wiki.</li>

<li>Các trang web nhỏ có thể được lưu trữ từ kho công cộng trên Github. Định dạng URL là http://projectname.github.io. Và có thể được tạo ra bằng cách bắt đầu một kho lưu trữ được định dạng như projectname.io</li>

<li>Code Snippets (bằng cách sử dụng tên miền phụ Gist).</li>

<li>Theo dõi vấn đề và tính năng yêu cầu.</li>

<li>Trực quan của dữ liệu không gian địa lý.</li>

<li>Biểu đồ Gantt.</li>
</ul>
####2. Tạo repository đặt tên là python_trainings<a name="2"></a>

**Tạo một repo mới trên trang github.com**

*Bước 1: Truy cập vào trang github.com và đăng nhập vào tài khoản cá nhân*

*Bước 2: Click chọn New Repository*

<img src="http://i.imgur.com/iE9JLQo.png">

*Bước 3: Ở phần Repository name nhập tên python_trainings sau đó chọn Create repository*

<img src="http://i.imgur.com/ZHdngn0.png">

####3. Markdown là gì? Dùng để làm gì?<a name ="#3"></a>

**Markdown là gì?**

<img src="http://i.imgur.com/1EmlOtW.png">

Markdown là một ngôn ngữ đánh dấu với cú pháp văn bản thô, được thiết kế để có thể dễ dàng chuyển thành HTML và nhiều định dạng khác sử dụng một công cụ cùng tên. Nó thường được dùng để tạo các tập tin readme, viết tin nhắn trên các diễn đàn, và tạo văn bản có định dạng bằng một trình biên tập văn bản thô.

**Markdown dùng để làm gì?**

Sự phổ biến của HTML khiến ngôn ngữ đánh dấu này được sử dụng rộng rãi trong các ứng dụng sử dụng internet từ các trang web tới nội dung email hay rất nhiều các tài liệu hướng dẫn online cũng đều sử dụng ngôn ngữ này. Tuy nhiên một vấn đề gặp phải của HML đó là cú pháp của ngôn ngữ này không được thân thiện lắm với người dùng. Ví dụ khi chúng ta có 1 đoạn văn bản HTML gồm 1 tiêu đề và 3 đoạn văn thì mã lệnh trông sẽ giống như sau:
```sh
<h1>Tiêu Đề</h1>
<p>Đoạn văn thứ nhất</p>
<p>Đoạn văn thứ 2</p>
<p>Đoạn văn thứ 3</p>
```

Nếu như không có kiến thức về ngôn ngữ HTML thì bạn rất khó có thể đọc được nôi dung của đoạn văn bản trên. Và ngay cả khi bạn đã hiểu về HTML thì đoạn mã trên vẫn gây rối mắt.

Markdown giải quyết vấn đề trên bằng việc đưa ra cú pháp để giúp đánh dấu văn bản một cách dễ hiểu và ngắn gọn hơn. Vẫn như ví dụ trên nhưng sử dụng Markdown thì kết quả sẽ như sau:

```sh
## Tiêu Đề
Đoạn văn thứ 3

Đoạn văn thứ 2

Đoạn văn thứ 3
```

Rõ ràng bạn thấy được cách viết thứ 2 ngắn gọn và dễ hiểu hơn rất nhiều so với cách viết đầu tiên dùng HTML.

####4. Các cú pháp thường gặp<a name="#4"></a>

**4.1. Thẻ tiêu đề**

Markdown sử dụng kí tự # để bắt đầu cho các thẻ tiêu đề, có thể dùng từ 1 đến 6 ký tự # liên tiếp. Mức độ tiêu đề giảm dần từ 1 đến 6.

Tùy mục đích và ý thích bạn có thể sử dụng cách này để thể hiện các chỉ mục khác nhau.

>Ví dụ:
>
>```sh
>#1. Tiêu đề cấp 1
>```
>
>#1. Tiêu đề cấp 1
>
>```sh
>##2. Tiêu đề cấp 2
>```
>
>##2. Tiêu đề cấp 2
>
>```sh
>######6. Tiêu đề cấp 6
>```
>
>######6. Tiêu đề cấp 6

**4.2. Chèn link, chèn ảnh**

<li>Để chèn hyperlink bạn chỉ cần paste luôn link đó vào file .md</li>

```sh
http://github.com
```

http://github.com.md 

Hoặc bạn cũng có thể sử dụng cú pháp sau để thu ngắn đường dẫn của link

```sh
[Github](https://github.com)
```

Kết quả là

[Github](https://github.com)

<li>Để chèn ảnh thì bạn hãy sử dụng cú pháp sau:</li>

```sh
<img src="link_anh_cua_ban">
```

Tôi thường sử dụng công cụ Lightshot để chụp ảnh màn hình và up hình đó lên trang http://i.imgur.com/ để lấy đường dẫn ảnh đưa vào Github

Hai công cụ này khá dễ sử dụng, bạn chỉ cần chụp màn hình bằng Lightshot ấn Ctrl + C để copy và Ctrl + V để paste vào trình duyệt tại trang web http://i.imgur.com/

**4.3. Ký tự in đậm, in nghiêng**

<li>Để in đậm một đoạn text bạn chỉ cần làm như sau:</li>

```sh
**từ cần in đậm**
```

**từ cần in đậm**

<li>Để in nghiêng một đoạn text bạn chỉ cần làm như sau:</li>

```sh
*từ cần in nghiêng*
```

*từ cần in nghiêng*

**4.4. Trích dẫn, bo chữ**

Để bo một đoạn text thì bạn chỉ cần sử dụng cú pháp sau:

```sh
`đoạn cần bo`
```

Kết quả là: `đoạn cần bo`

Để làm nổi bật một đoạn, chẳng hạn như một đoạn shell hay file cấu hình bạn có thể sử dụng cú pháp như ví dụ sau:

```sh
auto eth0
iface eth0 inet static
ipaddress 10.10.10.10
netmask 255.255.255.0
gateway 10.10.10.1
dns-nameservers 8.8.8.8
```

Kết quả như sau:

```sh
auto eth0
iface eth0 inet static
ipaddress 10.10.10.10
netmask 255.255.255.0
gateway 10.10.10.1
dns-nameservers 8.8.8.8
```

**4.5. Gạch đầu dòng**

Để sử dụng gạch đầu dòng bạn chỉ cần sử dụng cú pháp sau:

```sh
- Gạch đầu dòng thứ nhất
  <ul>
  <li>Thụt với đầu dòng 1</li>
  <li>Thụt với đầu dòng 1</li>
  </ul>
- Gạch đầu dòng thứ hai
  <ul>
  <li>Thụt với đầu dòng 2</li>
  <li>Thụt với đầu dòng 2</li>
  </ul>
```

Kết quả là:

- Gạch đầu dòng thứ nhất
  <ul>
  <li>Thụt với đầu dòng 1</li>
  <li>Thụt với đầu dòng 1</li>
  </ul>
- Gạch đầu dòng thứ hai
  <ul>
  <li>Thụt với đầu dòng 2</li>
  <li>Thụt với đầu dòng 2</li>
  </ul>

**4.6. Tạo bảng**

Bạn có thể sử dụng cú pháp sau để tạo bảng:

```sh
| Cột 1 Hàng 1 | Cột 2 | Cột 3| Cột 4 |
|--------------|-------|------|-------|
| Hàng 2 | 2 x 1 | 2 x 2 | 2 x 3 | 2 x 4 |
| Hàng 3 | 3 x 1 | 3 x 2 | 3 x 3 | 3 x 4 |
| Hàng 4 | 4 x 1 | 4 x 2 | 4 x 3 | 4 x 4 |
```

Kết quả:

| Cột 1 Hàng 1 | Cột 2 | Cột 3| Cột 4 |
|--------------|-------|------|-------|
| Hàng 2 | 2 x 1 | 2 x 2 | 2 x 3 | 2 x 4 |
| Hàng 3 | 3 x 1 | 3 x 2 | 3 x 3 | 3 x 4 |
| Hàng 4 | 4 x 1 | 4 x 2 | 4 x 3 | 4 x 4 |

*Mẹo*
<ul>
<li>Sử dụng trang [http://markdownlivepreview.com/](http://markdownlivepreview.com/) paste vào đó đoạn markdown bạn viết và xem trước để chỉnh sửa cho phù hợp.</li>
<li>Bạn cũng có thể sử dụng những đoạn markdown của người khác đã viết trước để tham khảo.</li>
</ul>

Như vậy bạn đã có thể trình bày github của mình một cách sáng sủa bằng markdown.

*Dưới đây là một số phím tắt trong Markdown:*

<img src="http://i.imgur.com/p90UWhI.png">

####5. Cài đặt Sublime Text và tìm kiếm, cài đặt các công cụ hỗ trợ markdown (export HTML, markdown preview, ...)<a name="#5"></a>

**Cài đặt Sublime Text**

<img src="http://i.imgur.com/0AkMnF5.png">

>Trong thế giới lập trình, ắt hẳn bạn đã từng dùng ít nhất một công cụ nào đó để phát triển các ứng dụng của mình. Một trong số đó có thể bạn đã từng nghe hoặc dùng đến là Sublime Text, hiện đã ở bản 3. Nó là một công cụ editor mã nguồn đa nền tảng với Python API. Nó hỗ trợ rất nhiều ngôn ngữ lập trình và ngôn ngữ đánh dấu. Các chức năng của nó có thể được mở rộng bởi user thông qua plugin, về cơ bản là nó do cộng đồng xây dựng lên và có thể được chỉnh sửa theo free-software licenses. Do khả năng mở rộng là rất cao nên rất nhiều các plugin đã được tạo ra để hỗ trợ developer.

*Các bước thực hiện*

#####Bước 1: Cài đặt Package Control

<li>Cài đặt Sublime Text 3 (ST3), download tại [đây](http://www.sublimetext.com/3)</li>

<li>Mở ST3, nhấn tổ hợp phím Ctr+` và nhập code sau:</li>


```sh
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

<li>Khởi động lại ST3</li>

#####Bước 2: Cài đặt Plugins

<li>Vào Preferences > Package Control > Install Package > Nhập Markdown Editing</li>

<li>Tương tự nhưng nhập Markdown Preview</li>

<li>Chờ cài đặt xong, khởi động lại ST3</li>

#####Bước 3: Cài đặt phím tắt

<li>Thiết lập phím tắt để sử dụng Markdown Preview: Vào Preferences > Key Bindings - User nhập (Bạn có thể sử lại alt+m thành phím tắt mà bạn muốn) sau đó lưu lại:</li>

```sh
[
   { "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} }
]
```

#####Bước 4: Kiểm tra thử

<li>Test xem như thế nào, tạo file *.md, nhập thử đoạn markdown:</li>

```sh
### Credits / Thanks
* Alexis Metaireau / Pelican
* Digital Surgeons / Gumby Framework
* Twitter Bootstrap
* traeblain for his [makefile](https://gist.github.com/traeblain/4252511) gist for building Pelican on Windows
```

<li>Nhấn tổ hợp phím Alt+M (mặc định) hoặc tổ hợp phím mà bạn đã cài đặt để xem trước trên trình duyệt.</li>

####6. Các công cụ viết Markdown khác:<a name="#6"></a>

**Stackedit**

<img src="http://i.imgur.com/HUmrlyX.png">


**JBT**

**Tablesgenerator**

Bạn có thể truy cập Tables Generator tại [đây](http://www.tablesgenerator.com/)
