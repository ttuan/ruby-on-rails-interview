# Ruby on Rails Interview

A collection of interview questions about Ruby/Rails.

## Project:
+ Trên trường
+ Trong cty

## Dev basic
+ OOP
+ MVC là gì, công việc của nó như thế nào?
Giả dụ ta có 1 cái TV, thì MVC tương ứng với những bộ phận nào trên cái TV đó.

## Ruby + Rails
+ Rails là gì? Trước có làm việc với framework nào khác không, thấy Rails có ưu, nhược điểm gì so với framework đó?
+ Cách tạo getter và setter
+ Theo RESTful, 1 controller sẽ bao gồm những action gì, kể tên, nhiệm vụ của từng action.
+ Enum là gì
+ Cronjob, activejob là gì? Ví dụ 1 trường hợp ứng dụng nó
+ Strong parameters là gì? Tại sao lại cần thiết.
+ Nested attributes sử dụng như thế nào? Ví dụ trường hợp ứng dụng.
+ Callback trong model sử dụng như thế nào? `after_save` va `after_commit` khac nhau ntn
+ Những constant đặt ở đâu.
+ STI, polymorfic là gì?
+ N + 1 queries la gi? Cach de giai quyet no. [N + 1 queries case-study](https://snippets.cacher.io/snippet/fb6813829f4450481dcd)
+ Includes, preload, joins
+ Asset pipeline là gì?
+ Metaprograming là gì? Đã từng sử dụng kỹ thuật nào liên quan đến nó chưa? Ducktyping là gì, cho 1 ví dụ khi dùng trong Ruby.
+ Sắp tới ra Rails 6, thì nó có bổ sung cái gì hay hay không?
+ Cơ chế của chức năng đăng ký, login qua Facebook như thế nào?
+ Từ khóa `yeild` trong Ruby được dùng ntn
+ Cơ chế phân trang hoạt động như thế nào.

|  So sanh |   |
|---|--:|
|  `save` | `save!`  |
| `Time.now`  | `Time.zone.now`  |
| `Class`  | `Module`  |
| `Gemfile` | `Gemfile.lock` |
| `find` | `find_by` |
| `includes` | `extends`|
|`after_save`|  `after_commit` |

## Unit test
+ Có viết test không? Sử dụng công cụ gì?
+ Tại sao phải viết Unit test, ý nghĩa?

## Database
+ Mô tả các kiểu join.
+ Transaction là gì?, ví dụ trường hợp sử dụng.
+ Index là gì, tại sao giúp truy xuất nhanh hơn, sao không đánh index tất cả cho nhanh.
+ Có biết về Procedure, Trigger, Function, Cursor không?

## Coding style
+ Có sử dụng các design patterns nào để refactor code không? (Service object, decorator, helper, validator, ...)
+ Lam the nao de tranh fat models va fat controllers?

## Workflow
+ Quy trình làm task như thế nào? Từ lúc nhận cho đến lúc hoàn thành.

## Security
+ SQL injection là gì? Phòng chống thế nào
+ Biết về XSS, CSRF atk không? Mô tả. Cai `protect_from_forgery` trong `ApplicationController` de lam gi?
+ Minh nen luu tru password ntn de bao mat?
+ Tại sao khuyến khích sử dụng HTTPS thay vì HTTP?

## Git
- Git flow trong quá trình làm việc ntn? từ bước fork -> gửi PR.
- `git merge` khác với `git rebase` ntn.
- Giờ a code xong tính năng mới, nhưng lại lỡ gõ commit --amend thì sẽ cần fix lại ntn

## Algorithm

## Advanced
1. Questions:
* Ruby co phu thuoc vao whitespace khong? Neu co thi cho vi du?
* Level ke thua cao nhat cua object la gi? => BasicObject
* Co phai moi thu trong Ruby deu la object khong? Neu khong, cho vi du? => method + block khong phai.
* Co the init symbol = Symbol.new duoc khong? tai sao?
* `Rakefile` va `config.ru` trong thu muc cua project Rails dung de lam gi?


2. Sample code - Case study
* [Array and Boolean](https://snippets.cacher.io/snippet/f3a5c617b3d4d6758469)
* [Truly and Falsy](https://snippets.cacher.io/snippet/b99bdbad2bdbef77e66b)
* [Hash.first and Hash.last](https://snippets.cacher.io/snippet/bf8b896d686b5892218c)
