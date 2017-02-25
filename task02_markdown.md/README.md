##Task 2
------------------------
>Người thực hiện: Hồ Nguyễn Tường Vi
>
>Tên tài liệu: 
 + [http://nukeviet.edu.vn/news/Chia-se-kien-thuc-web/Git-la-gi-Tai-sao-su-dung-Git-16.html](http://nukeviet.edu.vn/news/Chia-se-kien-thuc-web/Git-la-gi-Tai-sao-su-dung-Git-16.html)
 + [https://thachpham.com/](https://thachpham.com/)
 + [http://rogerdudler.github.io/git-guide/index.vi.html](http://rogerdudler.github.io/git-guide/index.vi.html)
 + [https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%E1%BA%A5u-H%C3%ACnh-Git-L%E1%BA%A7n-%C4%90%E1%BA%A7u](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%E1%BA%A5u-H%C3%ACnh-Git-L%E1%BA%A7n-%C4%90%E1%BA%A7u)
 >
 >Ngày cập nhật: 27/02/2017
 >
 ----------------------------
 
##Mục lục:

[1. Git là gì? Dùng để làm gì?](#1)

[2. Cài đặt Git trên máy tính](#2)

[3. Cách sử dụng Git trên CMD (terminal)](#3)

[4. Sử dụng Git để commit/push file README.md lên GitHub](#4)

##Nội dung:

####1. Git là gì? Dùng để làm gì?<a name="1"></a>

<img src="http://i.imgur.com/XJgvEVw.jpg">

**Git là gì?**

Git là một hệ thống [VCS](http://wiki.nukeviet.vn/programming:vcs) (Version Control System) dùng để quản lý và kiểm tra các phiên bản mã nguồn khác nhau trong quá trình phát triển mã nguồn. Git là thế hệ mới nhất của các phần mềm này. Từ phiên bản NukeViet 4.0, nhóm phát triển NukeViet sẽ sử dụng git thay thế cho [Subversion](http://wiki.nukeviet.vn/programming:vcs:subversion) (SVN) đang được sử dụng để quản lý code của NukeViet trên Google code trước đây. Mặc dù Google code cũng đã hỗ trợ Git từ tháng 7 năm 2011, tuy nhiên chúng ta sẽ lựa chọn Github làm nơi lưu trữ code mới cho NukeViet vì tính chuyên nghiệp của Github đối với Git.

Có rất nhiều bạn khi nghe nói đến Git sẽ nghĩ ngay đến [Github](https://github.com) và có thể sẽ có một số hiểu lầm với họ. Cũng xin nhắc lại rằng, Git là tên gọi của một mô hình hệ thống. Như mình đã giải thích ở trên, các máy tính có thể clone lại mã nguồn từ một repository và Github chính là một dịch vụ máy chủ repository công cộng, mỗi người có thể tạo tài khoản trên đó để tạo ra các kho chứa của riêng mình để có thể làm việc.

**Git dùng để làm gì?**

Git có nhiều ưu điểm, đặc biệt nó đã thay đổi cách các lập trình viên chia tách và nhập các nhánh phần mềm. Trong khi với SVN, việc này luôn là ác mộng vì các xung đột trong quá trình tách/nhập, còn với Git việc này quá dễ dàng.

GIT hoạt động theo mô hình Local và Remote repositories: Bạn hoàn toàn có thể làm mọi thao tác/công việc trên bản sao (local) repository trên máy tính. Sau khi hoàn thiện công việc rồi có thể đẩy lên Remote repository để chia sẻ cho người khác.

####2. Cài đặt Git trên máy tính<a name="2"></a>

Đầu tiên, bạn phải chọn cho mình một phiên bản phù hợp với hệ điều hành của máy tính mình và tải về:

**Cài đặt Git trên Linux**

- Bước 1: Download git dành cho Linux: [Git Linux](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

- Bước 2:
Nếu bạn đang sử dụng hệ điều hành Ubuntu/Debian thì có thể sử dụng lệnh sau để cài Git.

  ```sh
  $ sudo apt-get install git
  ```

Hoặc lệnh sau để cài trên CentOS/Fedora/RHEL.

```sh
$ yum install git
```

**Cài đặt Git trên Windown**

- Bước 1: Download git dành cho Window: [Git Window](https://git-for-windows.github.io/)

- Bước 2: Sau khi cài đặt Git vào Windows, bạn sẽ cần mở ứng dụng Git Bash lên để bắt đầu sử dụng các dòng lệnh của Git.

- Bước 3: Việc đầu tiên bạn nên làm khi cấu hình Git là chỉ định tên tài khoản và địa chỉ e-mail. Điều này rất quan trọng vì mỗi Git sẽ sử dụng chúng cho mỗi lần commit, những thông tin này được gắn bất di bất dịch vào các commit:

```sh
$ git config --global user.name "Username"
$ git config --global user.email "Email"
```

- Bước 4: Kiểm tra cấu hình:

Nếu như bạn muốn kiểm tra các cấu hình cài đặt, bạn có thể sử dụng lệnh sau để liệt kê tất cả các cài đặt của Git:

```sh
$ git config --list
```

####3. Cách sử dụng Git trên CMD (terminal)<a name="3"></a>

Để mở CMD, bạn nhập "CMD" vào ô tìm kiếm. Ở đây có Command Prompt và Git CMD, bạn có thể lựa chọn bất cứ 1 trong 2.

<img src="http://i.imgur.com/C38z5r5.png">

Sau đó, bạn nên tạo một Repository mới, gõ dòng lệnh:

```sh
git init
```

Kế tiếp, sao chép (clone) một repository:

```sh
git clone /đường-dẫn-đến/tên-repository
```

*Chú ý:* Để biết được tên đường dẫn, bạn làm như sau:

<img src="http://i.imgur.com/m2B8o4G.png">

<img src="http://i.imgur.com/u6afn6R.png">

<img src="http://i.imgur.com/mGbUEvj.png">

Nhấn Enter để chạy chuong trình.

####4. Sử dụng Git để commit/push file readme.md lên github<a name ="4"></a>

Đầu tiên, bạn mở Git Bash từ ô tìm kiếm.

<img src ="http://i.imgur.com/qeWeWLi.png">

Tiếp theo, dùng dòng lệnh sau để đến được thư mục chính:

<img src="http://i.imgur.com/DHiJz87.png">

Bạn có thể đề xuất thay đổi (thêm nó vào chỉ mục Index) bằng cách:

```sh
git add *
```

Đây là bước đầu tiên trong quy trình git cơ bản. Để thật sự commit những thay đổi, bạn sử dụng:

```sh
git commit -m "ghi-chú-commit"
```

Thay đổi của bạn hiện đang nằm tại HEAD của bản sao cục bộ đang làm việc. Để gửi những thay đổi đó đến repository remote, bạn thực thi:

```sh
git push origin master
```

Sau khi đã thực hiện các câu lệnh như trên, việc commit/push file readme.md lên github đã thành công khi màn hình thông báo như sau:

<img src="http://i.imgur.com/8zDyglt.png">

*Chúc các bạn thành công*













