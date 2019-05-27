# Ruby on Rails Interview

A collection of interview questions about Ruby/Rails.

## Project:
+ Trên trường
+ Trong cty

Trong các dự án đã làm, trình bày 1 vài vấn đề gì hay ho/khó khăn mà mình đã giải quyết được.

## Web
#### 1. Basic
+ MVC:
	* Khái niệm.
	* Giả dụ ta có 1 cái TV, thì MVC tương ứng với những bộ phận nào trên cái TV đó.
	* Rails áp dụng theo mô hình MVC, tức là chỉ cần 3 thư mục `app/model`, `app/controllers`, `app/views` là đủ, em nghĩ có cần thêm các thư mục `assets`, `helpers`, ... vào không?
+ Authenticate:

   * Sau khi người dùng đăng nhập trên website, ở những request tiếp theo làm thế nào server biết được là user đó đã đăng nhập?

#### 2. Middle
+ RESTful:
	* Khái niệm
	* So sánh REST với SOAP/GraphQL thì có ưu, nhược điểm gì?
	* Có giao thức là `gRPC`, có dùng thử bao giờ không?
+ HTTP Status code đại diện cho thông tin gì? (1xx, 2xx, 3xx, 4xx, 5xx) - [source](https://kipalog.com/posts/An-so-tu-nhung-HTTP-status-code)
+ Flow của Basic Authentication là gì, bạn đã dùng nó trong trường hợp nào? - [source](https://kipalog.com/posts/Authentication-story-part-1--Authentication-la-lam-gi)
+ Flow của Oauth2 là gì? - [source](https://viblo.asia/p/introduction-to-oauth2-3OEqGjDpR9bL)
#### 3. Advanced
+ HTTPS hoạt động như thế nào? Tại sao nó bảo mật hơn HTTP? - [source](https://viblo.asia/p/hieu-hon-ve-https-voi-vi-du-bo-cau-dua-thu-OeVKBojQZkW)

## Rails
#### 1. Basic
+ Rails là gì? Trước có làm việc với framework nào khác không, thấy Rails có ưu, nhược điểm gì so với framework đó?
+ RESTful:
	* 1 controller sẽ bao gồm những action gì? Kể tên, nhiệm vụ của từng action.
	* Trong file `config/route.rb` nếu khai báo `resources` và `resource` thì có gì khác nhau?
+ STI, polymorfic là gì? Cho ví dụ.
+ N + 1 queries:
	* N + 1 queries là gì? Có những cách nào để giải quyết vấn đề này.
	* Phân biệt `includes`, `preload` và `eager_load`. Các câu lệnh SQL nào sẽ được sinh ra?
	* [Case Study](https://snippets.cacher.io/snippet/fb6813829f4450481dcd)
+ Enum:
	* Enum là gì?
	* Khi khai báo `enum status: [:active, :deactive]` thì sẽ có những hàm nào được tự động sinh ra?
+ Nested attributes:
	* Thường được sử dụng trong quan hệ nào? (1-1, 1-n, n-n)
	* Lấy 1 ví dụ.
+ Strong parameters:
	* Khái niệm và cách dùng.
	* Lý do tại sao ta lại cần dùng strong parameters.
+ Phân biệt: `find` vs `find_by`, `Time.now` vs `Time.zone.now`, `save` and `save!`
+ Phân biệt `Gemfile` và `Gemfile.lock`.
+ Phân biệt `scope` và class method.
+ Cơ chế phân trang hoạt động như thế nào.


#### 2. Middle
+ Asset pipeline là gì?
+ Cronjob, activejob là gì? Ví dụ 1 trường hợp ứng dụng nó
+ Cơ chế của chức năng đăng ký, login qua Facebook như thế nào?
+ Callback:
	* Trong Rails có những loại callback nào? (b/a_validation, save, create, save, destroy, around_create/save, after_commit, after_rollback)
	* Phân biệt `after_save` và `after_commit`.
+ `Rakefile` và `config.ru` trong thư mục Rails project để làm gì?
+ Gems:
	* Đã thử viết gems bao giờ chưa?
	* Lấy vd về 1 số gem cơ bản (`devise`, ..) xem mức hiểu biết ntn? (biết dùng, override lại hàm, ...)


#### 3. Advanced
+ Rails session hoạt động như thế nào? - [Source](https://www.justinweiss.com/articles/how-rails-sessions-work/)
+ Rack middleware là gì? Bạn đã làm việc với Rack middleware bao giờ chưa?

#### 4. Fun facts
\# TODO

## Ruby
#### 1. Basic
+ OOP là gì? Áp dụng vào trong Ruby như thế nào?
+ Cách tạo getter và setter
+ Từ khóa `yeild` trong Ruby được dùng như thế nào? Liên hệ với `yield` trong file `application.html.erb` của Rails app.
+ Phân biệt `public`, `protected` và `private` trong Ruby.
	* Tại sao class con lại có thể gọi được method private của class cha?
	* [Case Study](https://snippets.cacher.io/snippet/fe39ac92580f09e0b0bd)
	* Gọi tường minh và không tường minh trong Ruby.

#### 2. Middle
+ Metaprograming là gì? Đã từng sử dụng kỹ thuật nào liên quan đến nó chưa?
+ Ducktyping là gì, cho 1 ví dụ khi dùng trong Ruby.
+ Module:
	* Em biết gì về Method lookup path?
	* `include`, `extend`, `prepend` khác nhau ntn?
	* Trong Ruby, để lấy list các module, class cha, ta dùng lệnh gì? (`Class.ancestors`)

Case study:

* [Array and Boolean](https://snippets.cacher.io/snippet/f3a5c617b3d4d6758469)
* [Truly and Falsy](https://snippets.cacher.io/snippet/b99bdbad2bdbef77e66b)
* [Hash.first and Hash.last](https://snippets.cacher.io/snippet/bf8b896d686b5892218c)

#### 3. Advanced
* Ruby có phụ thuộc vào whitespace không? Nếu có thì cho ví dụ?
* Level kế thừa cao nhất của object là gì? (`BasicObject`)
* Có thể init symbol bằng `Symbol.new` được không? Tại sao?
* So sánh symbol và string. [Source](https://viblo.asia/p/string-and-symbol-in-ruby-3Q75wW1e5Wb)

#### 4. Fun facts
* Có phải mọi thứ trong Ruby đều là object không? Nếu không thì cho ví dụ? (method vs block không phải)


## Unit test
#### 1. Basic
+ Có viết test không? Sử dụng công cụ gì?
+ Tại sao phải viết Unit test, ý nghĩa?

#### 2. Middle

#### 3. Advanced


## Database

#### 1. Basic
+ Mô tả các kiểu join.
+ Transaction là gì?, ví dụ trường hợp sử dụng.
+ Index là gì, tại sao giúp truy xuất nhanh hơn, sao không đánh index tất cả cho nhanh.
+ Có biết về Procedure, Trigger, Function, Cursor không?

#### 2. Middle
* Mô tả về mô hình Master - Slave và cách thức hoạt động của nó. [source](https://viblo.asia/p/gioi-thieu-ve-mysql-replication-master-slave-bxjvZYwNkJZ)
* Mô tả về sharding trong database. [source](https://www.digitalocean.com/community/tutorials/understanding-database-sharding)
* [Case Study](https://snippets.cacher.io/snippet/2a9306a2e0defb9abff4) về Optimistic Locking và Pessimistic Locking.
  [Source](https://viblo.asia/p/optimistic-locking-va-pessimistic-locking-trong-ung-dung-rails-bWrZngOplxw)
#### 3. Advanced



## Refactoring

\# TODO: Add more from: [Decopling Rails Components](https://www.toptal.com/ruby-on-rails/decoupling-rails-components), [Best Ruby on rails refactoring talks](https://infinum.co/the-capsized-eight/best-ruby-on-rails-refactoring-talks).

#### 1. Basic
+ Làm thế nào để tránh fat models và fat controllers?
+ Có sử dụng các patterns nào để refactor code không? (Service object, decorators, validators, ...)

#### 2. Middle

#### 3. Advanced

## DevOps/Infrastructure
#### 1. Basic
+ Deploy app
+ Docker

#### 2. Middle

#### 3. Advanced

## Security
\# TODO: Add more questions from [common rails security](https://www.sitepoint.com/common-rails-security-pitfalls-and-their-solutions/?utm_source=rubyweekly&utm_medium=email)!

#### 1. Basic
+ SQL injection là gì? Phòng chống thế nào?
+ Biết về XSS, CSRF atk không? Mô tả. Cái `protect_from_forgery` trong `ApplicationController` để làm gì?
+ Nên lưu trữ password của user như thế nào?

#### 2. Middle

#### 3. Advanced

## Git

#### 1. Basic
- Git flow trong quá trình làm việc như thế nào? Từ bước fork -> gửi PR.
- `git merge` khác với `git rebase` như thế nào?
- Giờ anh code xong tính năng mới, nhưng lại lỡ gõ `git commit --amend` thì sẽ cần fix lại như thế nào?
- Lỡ làm task và commit trên branch A, nhưng giờ muốn đưa phần code đó sang bên branch B thì làm thế nào?
#### 2. Middle

#### 3. Advanced

## Algorithm

## Workflow
+ Quy trình làm task như thế nào? Từ lúc nhận cho đến lúc hoàn thành.

## Tech news
+ Sắp tới ra Rails 6, thì nó có bổ sung cái gì hay hay không?
+ Có hay tham khảo qua các blog công nghệ, github trending không?

## Third party services
\# TODO: AWS, GG Cloud, Firebase, ...


