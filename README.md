# Những lý do cho việc sử dụng design pattern
## Giới thiệu

Sau những bài báo về vấn đề Tại sao thiết kế rất quan trọng trong phát triển phần mềm, Tôi muốn tiếp cận một khía cạnh mới, nâng cao hơn trong việc thiết kế phần mềm gọi là: Design Patterns. Như những bài báo trước của tôi, ý tưởng trong suốt cuộc họp với một thành viên dự án là làm sao để thiết kế phần mềm một cách tốt nhất. Cuộc thảo luận xoay quanh ý kiến cho rằng sử dụng Design Patterns quá mất thời gian trong việc phát triển hệ thống thương mại. Mục đích của tôi ở đây là để chứng minh tại sao tôi tin rằng điều đó là sai.

Tôi sẽ không đi chi tiết vào bất kì cấu trúc hay ví dụ nào của Design Patterns.Có nhiều nguồn tham khảo hay về chúng ở khắp nơi.

## Một Design Pattern là gì?

Để bắt đầu, ta tìm hiểu Design Pattern chính xác là cái gì? Ở đây là vài định nghĩa về thuật ngữ này:

Tham khảo từ Wikipedia:

"Một design pattern trong kiến trúc và khoa học máy tính là một phương pháp tiêu chuẩn ghi chép giải pháp để giải quyết vấn đề về thiết kế trong bất kì lĩnh vực chuyên môn nào."

Tham khảo từ Data & Object Factory:

"Design patterns là các giải pháp ~định kì~(**chung**) cho các vấn đề thiết kế phần mềm mà bạn liên tục ~~phải tìm kiếm~~(again and again-**lặp đi lặp lại**) trong khi phát triển phần mềm trong thực tế. Patterns là các thiết kế và tương tác với các đối tượng, giống như là cung cấp 1 ~~phương thức truyền thông 1 cách lịch sự~~ (communication platform concerning elegant-**nền tảng giao tiếp rõ ràng**), giải quyết được thách thức trong vấn đề lập trình là các giải pháp tái sử dụng. "

Vì vậy một Design Pattern là một mục đích chung của một vấn đề, có thể được áp dụng cho một giải pháp cụ thể. Khi các nhà phát triển phần mềm có xu hướng giải quyết nhiều loại vấn đề tương tự, nó làm cho mọi vấn đề trong phần mềm có thể giải quyết được khi kết hợp các giải pháp khác nhau. Tại sao phải phát minh lại bánh xe?


## Tài liệu hay và dễ hiểu

Design Patterns được viết tài liệu hay và dễ hiểu bởi các kĩ sư, các thiết kế, các lập trình viên, sau đó sản phẩm của họ được sử dụng trong các giải pháp cụ thể sẽ dễ hiểu hơn.

Design Patterns cung cấp cho các nhà phát triển phần mềm một loạt các giải pháp đã được thử nghiệm cho các vấn đề cơ bản, do đó, ta giảm được các nguy cơ cho dự án bằng việc không phải sử dụng một bản thiết kế mới và chưa được kiểm tra.

Design Patterns ban đầu có thể tốn nhiều thời gian phát triển, vì nếu đội của bạn chưa làm quen với nó thì phải đi lòng vòng. Tuy nhiên, khi nhìn vào quá trình phát triển, ~~các thói quen sử dụng chúng tăng lên~~(once familiarity with them increases**khi ngày càng quen dần với design pattern**), thời gian để phát triển phần mềm sẽ giảm đi..

## So sánh với kĩ thuật dân dụng

Để đưa ra một sự tương tự của một mẫu thiết kế từ lĩnh vực kỹ thuật dân dụng (như tôi đã nêu trong bài báo của tôi Tại sao thiết kế là quan trọng đối với phát triển phần mềm) có những điểm tương đồng gần giống với công nghệ phần mềm), có thể là tìm kiếm một giải pháp để vượt qua sông. Đây là một vấn đề thường xuyên đối với các kỹ sư dân dụng, trong đó có một số giải pháp được ghi nhận và hiểu rõ. Các kỹ sư dân dụng có thể xây dựng một cây cầu hoặc một đường hầm.

Tại sao một kỹ sư dân dụng cố gắng giải quyết vấn đề này từ đầu khi có những giải pháp trong thế giới thực có thể giải quyết vấn đề này đã được đề cập đến? Có sự tương đồng gần gũi giữa kỹ sư xây dựng giải quyết vấn đề về sông và kỹ sư phần mềm giải quyết vấn đề phần mềm:


* Các giải pháp (cầu hoặc đường hầm) đều được hiểu và ghi lại
* Các giải pháp (cầu hoặc đường hầm) giải quyết các vấn đề kỹ thuật xây dựng định kỳ
* Các giải pháp (cầy hoặc đường hầm) không cần phải xác định hay quy định nhưng nó khá trừu tượng và có thể điều chỉnh với các vấn đề cụ thể bằng tay ( các ví dụ như vật liệu xây cầu hay đường hầm có thể được lựa chọn để thể hiện cho sự liên kết trong các vấn đề cụ thể của họ)
*Lập luận chống lại design parttern cho thấy chúng không phù hợp với mục đích thương mại do chúng mất quá nhiều thời gian để triển khai, nó không thể kéo dài. Design parrterm tiết kiệm thời gian (khi được xem qua suốt vòng đời của ứng dụng) bằng cách cho nhà phát triển lựa chọn các giải pháp đã được thử và thử nghiệm sẵn có mà họ có thể tùy chỉnh theo nhu cầu cụ thể của riêng họ.

Vấn đề duy nhất tôi đã gặp với Design Patterns là họ mất thời gian để tìm hiểu. Một số người trong số họ có thể khó nắm bắt và hiểu được chúng. Đây thật sự là một lý do thích hợp, do đó nó đòi hỏi cần có kĩ năng tốt hơn để có thể sử dụng chúng. Điều này có thể khiến chi phí dự án ban đầu tăng lên. Tuy nhiên, khi nhìn vào vòng đời của một ứng dụng, tôi sẽ hoàn toàn mong đợi những chi phí phát triển ban đầu này sẽ được bù đắp lại do chi phí bảo trì thấp hơn do sự hiểu biết cao hơn và khả năng mở rộng dễ dàng hơn (làm cho ứng dụng dễ dàng mở rộng trong tương lai để đáp ứng những cơ hội ~~đang mới~~(**mở rộng**)).

Design Patterns giảm bớt sự phức tạp, và giúp các giải pháp trở nên dễ hiểu hơn.

Design Patterns là các giải pháp đã được kiểm tra và thử nghiệm, nhà phát triển không cần phải bắt đầu từ đầu, và có thể chạy như giải pháp tái sử dụng điều đó đã được chứng minh là có hiệu quả (miễn là Mẫu Thiết kế được sử dụng giải quyết một vấn đề tương tự). Sẽ là sai khi mong đợi một cây cầu để giải quyết vấn đề băng qua đại dương, nơi một cây cầu chỉ đơn giản là không phù hợp.

## Những lợi ích khi sử dụng các Design Pattern.

* Cung cấp cho các nhà phát triển một loạt các giải pháp đã được kiểm tra và thử nghiệm để làm việc với chúng.
* Chúng là ngôn ngữ trung lập ( trung gian ) và vì thế có thể áp dụng vào bất cứ ngôn ngữ nào có hỗ trợ hướng đối tượng.
* Chúng được hỗ trợ bởi truyền thông vì thực tế chúng đã được công nhận và có thể được nghiên cứu nếu nó không chỉ là một trường hợp cụ thể.
* Chúng có một bản theo dõi chứng minh chúng được sử dụng rộng rãi và giảm các lỗi kĩ thuật cho các dự án.
* Chúng có độ linh hoạt cao và có thể sử dụng trong bất kì ứng dụng hay tên miền nào.

## Kết luận

Design Patterns, là một khoản đầu tư rất đáng, mặc dù quá trình học tập ban đầu khó khăn. Chúng cho phép bạn thực hiện các giải pháp cho các vấn đề đã được thử nghiệm và kiểm tra do đó tiết kiệm được thời gian và sức lực trong suốt quá trình triển khai và phát triển phần mềm.  Bằng các sử dụng các giải pháp đã được làm rõ và có tài liệu rõ ràng, sản phẩm cuối cùng sẽ có mức độ hoàn thiện cao hơn nhiều. Nếu giải pháp dễ hiểu hơn, sau đó bằng cách mở rộng nó, nó sẽ được bảo trì dễ dàng hơn.

Practice
https://coderoncode.com/design-patterns/programming/php/coding/development/2014/01/19/design-patterns-php-factories.html
https://www.binpress.com/tutorial/the-factory-design-pattern-explained-by-example/142
https://www.codeproject.com/Articles/852232/PHP-Singleton-Pattern-A-Step-by-Step-And-Problem-s
http://www.fluffycat.com/PHP-Design-Patterns/
Keyword: how to separate code to package php, step by step php design pattern singleton(change singleton to other for more result)
