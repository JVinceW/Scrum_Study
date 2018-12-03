# Hướng dẫn dùng Kanban cho Scrum Team

Tháng 4 năm 2018

Scrum Homepage: [Scrum.org]

English version: [Original Page]

<!-- Start Document Outline -->
* [Hướng dẫn dùng Kanban cho Scrum Team](#hướng-dẫn-dùng-kanban-cho-scrum-team)
	* [Mục đích:](#mục-đích)
	* [Mối liên hệ với Scrum Guide:](#mối-liên-hệ-với-scrum-guide)
	* [Định nghĩa của Kanba:](#định-nghĩa-của-kanba)
	* [Kanban và lí thuyết Scrum:](#kanban-và-lí-thuyết-scrum)
	* [Định nghĩa của workflow:](#định-nghĩa-của-workflow)
	* [Service Level Expectation:](#service-level-expectation)
	* [Thực hành Kanban:](#thực-hành-kanban)
		* [Trực quan hóa workflow - Bảng kanban:](#trực-quan-hóa-workflow---bảng-kanban)
		* [Giới hạn WIP (Work in Progress):](#giới-hạn-wip-work-in-progress)
		* [Tích cực quản lý các hạn mục công việc đang tiến hành:](#tích-cực-quản-lý-các-hạn-mục-công-việc-đang-tiến-hành)
		* [Thanh tra và thích nghi với Workflow:](#thanh-tra-và-thích-nghi-với-workflow)
	* [Flow Metrics and Analytics :](#flow-metrics-and-analytics-)
		* [Cơ bản về chỉ số lưu lượng (Metrics of Flow):](#cơ-bản-về-chỉ-số-lưu-lượng-metrics-of-flow)
	* [Flow-Based Events:](#flow-based-events)
		* [The Sprint:](#the-sprint)
		* [Kế hoạch Flow-Based Sprint:](#kế-hoạch-flow-based-sprint)
		* [Họp Flow-Based Scrums hàng ngày:](#họp-flow-based-scrums-hàng-ngày)
		* [Sơ kết Flow-Based Sprint:](#sơ-kết-flow-based-sprint)
		* [Cải tiến Flow-Based Sprint:](#cải-tiến-flow-based-sprint)
	* [Lời kết:](#lời-kết)
	* [Acknowledgements:](#acknowledgements)
		* [Lịch sử:](#lịch-sử)
		* [Về bản dịch tiếng Việt:](#về-bản-dịch-tiếng-việt)
<!-- End Document Outline -->

## Mục đích:
Góc nhìn flow-based của Kanban có thể tăng cường và bổ sung cho Scrum framework và cách triển khai của nó. Team có thể áp dụng Kanban cho dù họ vừa bắt đầu dùng scrum hay đã dùng scrum trong một thời gian dài. Bản hướng dẫn Kanban cho Scrum Teams là kết quả của sự cộng tác giữa các thành viên của cộng đồng Scrum.org và các leader của cộng đồng Kanban. Cùng nhau, Họ đứng sau Bản Hướng dẫn dùng Kanban cho Scrum Teams. Đó là niềm tin chung của họ rằng các học viên phần mềm chuyên nghiệp có thể hưởng lợi từ việc áp dụng Kanban cùng với Scrum.

## Mối liên hệ với Scrum Guide:
Bản hướng dẫn này không thay thế hay cắt giảm phần nào của [Scrum Guide]. Nó được thiết kế để tăng cường và mở rộng việc thực hành của Scrum framework. Bản hướng dẫn nàu giả định rằng đọc giả đang điều hành một quy trình sử dụng Scrum framework. Do đó, Toàn bộ [Scrum Guide] áp dụng vào nó.

## Định nghĩa của Kanba:
Kanban (n): một chiến thuật để cải tiến dòng chảy giá trị của các bên liên quan thông qua một quy trình mà nó dùng một hệ thống trực quan, Hạn chế công việc kéo dài.

Trung tâm của định nghĩa kanba là concept(khái niệm) của "flow" (dòng chảy, luồng). Flow là sự dịch chuyên của giá trị khách hàng trên khắp hệ thống phát triển sản phẩm. Kanban cải tiến flow bằng cách nâng cao hiệu quả tổng thể, hiệu quả và khả năng dự đoán của một quy trình.
## Kanban và lí thuyết Scrum:
Đầu tiên, đánh giá nhanh lý thuyết chính của [Scrum Guide]:

* Scrum được xây dựng dựa trên lý thuyết quản lý tiến trình thực nghiệm, hay thực nghiệm luận. 
* Lý thuyết này chỉ ra rằng tri thức đến từ kinh nghiệm và việc ra quyết định được dựa trên những gì đã biết. 
* Ba yếu tố nòng cốt tạo thành một mô hình quản lý tiến trình thực nghiệm gồm: sự minh bạch,
thanh tra, và thích nghi.

Scrum chỉ định ràng Sprint Backlog minh bạch, nhưng nó lại cung cấp hạn chế về mặt làm thế nào để thực hiện nó. Mà nó cũng không xác định làm cách nào để xác định sự minh bạch rõ ràng cho flow của công việc vào Product Backlog, từ Product Backlog vào Sprint Backlog và bất cứ điều gì xảy ra cho công việc sau khi nó làm cho nó thành một gói tăng trưởng ("Done" increment). Đây là nơi Kanban có thể giúp đỡ. Bằng cách trực quan hóa công việc bằng một cách mới, một Scrum Team có thể áp dụng tập hợp các thực hành được đưa ra trong hướng dẫn này để có thể cải tiến chất lượng chuyển giao hiệu quả hơn. Những thực hành này vay mượn và xây dựng dựa trên các nguyên tắc của suy nghĩ gọn gàng, luồng phát triển sản phẩm và lý thuyết xếp hàng.
Một tác dụng phụ có lợi của việc cải tiến giá trị chuyển giao đó là nó cung cấp rất nhiều cơ hội để thanh tra và thích ứng quy trình và sản phẩm. Thắt chặt vòng phản hồi của khách hàng với Kanban là một chiến lượt đã được chứng minh để thực nghiệm cải thiện một quy trình.
Kanban siêu tập trung vào tính minh bạch, trực quan hóa, và luồng, kết hợp với Scrum framework, hình thành một nền tảng mạnh mẽ để thiết kế quy trình cung cấp tối ưu giá trị của khách hàng.

## Định nghĩa của Workflow:
Cái tiến luồng yêu cầu phải định nghĩa luồng là gì trong context(ngữ cảnh) của Scrum. Mỗi Scrum Team cần tạo ra định nghĩa của nó về "Quy trình làm việc (Workflow)" có chứa các yếu tố sau:
* Xác định các điểm mà tại đó Scrum Team xem xét công việc đã bắt đầu và đã kết thúc.
* Một định nghĩa của các đơn vị cá nhân của giá trị khách hàng mà chúng chảy qua cả hệ thống Scrum (Gần giống với Product Backlog Items(PBIs)).
* Một định nghĩa của trạng thái luồng công việc mà PBIs chảy qua từ lúc bắt đầu đến khi kết thúc (trong đó phải có ít nhất 1 trạng thái hoạt động).
* Chính sách rõ ràng về công việc chảy qua mỗi trạng thái như thế nào (Có thể bao gồm các hạn mục từ định nghĩa "Done" của một Scrum Team và kéo các chính sách giữa các trạng thái ) 
* Một định nghĩa về Work In Progress (WIP) sẽ bị hạn chế như thế nào.
* Một tập hợp các Service Level Expectation (SLE) mà nó có thể truyền đạt dự báo thời gian cần để hoàn thành các hạng mục công việc.

Mặc dù phụ thuộc vào việc Scrum Team định nghĩa "Workflow" của mình, nhưng có một số yếu tố phải bao gồm:
* Xác định các hạng mục công việc chưa trong một trạng thái hoạt động là "chưa bắt đầu".
* Xác định các hạng mục công việc đang bước vào trạng thái hoạt động "đã bắt đầu" là Work in Progress (WIP).
* Xác định các hạng mục công việc đã trải quả tất cả các trạng thái hoạt động được đặt ra cho các hạng mục đó là "đã hoàn thành".

Tóm lại, định nghĩa của "Workflow" bao gồm một sự hiểu biết chung về công việc đươc định nghĩa như thế nào(các hạng mục cộng việc), trạng thái bắt đầu của quá trình, trạng thái hoạt động cho các hạng mục công việc, và trạng thái đã hoàn thành của quá trình trong Scrun Team. 
Lưu ý ràng các trạng thái trong định nghĩa của "Workflow" có thể không trùng khớp với các trạng thái được xác định bởi Sprint Backlog. Ví dụ, Định nghĩa về "Workflow" của một Scrum Team có thể bao gồm các trạng thái như upstream, downstream, inside hoặc outside của Sprint Backlog. Tương tự, các hạn mục công việc dịch chuyện trong workflow sẽ không tương ứng với các hạng mục trong Product Backlog hoặc các phần khác của Sprint Backlog hoặc Scrum. Cuối cùng, một hạng mục công việc cụ thể có thể không chảy qua tất cả các trạng thái hoạt động, và một hạng mục công việc thậm chí có thể không chảy tuần tự qua các trạng thái hoạt động.
Việc tạo và thích ứng với định nghĩa của "Workflow" có thể tác động hoặc bị ảnh hưởng bởi hiện vật hiện có. Các tài khoản và các trách nhiệm của Chủ sản phẩm(Product Owner) và Nhóm phát triển (Development Team) đối với các hiện vật đó vẫn được mô tả trong [Scrum Guide]

## Service Level Expectation:

Một SLE dự báo mất bao lâu để một hạng mục chuyển từ bắt đầu đến kết thúc trong workflow của bạn. bản thân SLE có hai phần: Khoảng vài ngày trôi qua và xác suất được liên kết với khoảng thời gian đó (Ví dụ, "85% hạn mục công việc sẽ được hoàn thành trong 8 ngày hoặc ít hơn). SLE dựa trên lịch sử của chu kì thời gian của Scrum Team, và một lần tính toán, phải được đăng lên bảng Kanban. Nếu không tồn tại dữ liệu lịch sử chu kì thời gian, Scrum Team nên dự đoán một cách tốt nhất and sau đó thay thế dự đoán đó khi nó có đủ dữ liệu lịch sử để làm một tính toán SLE đúng đắn. Bất kể Scrum Team chọn cách tạo ra định nghĩa của nó về "Workflow" như thế nào đi nữa, nó là concept trung tâm của bản hướng dẫn này. Tất cả các yếu tố khác của bản hướng dẫn này phụ thuộc rất nhiều vào chính xác cách Scrum Team chỉ định định nghĩa của "Workflow". Nó có thể và nó nên thay đổi khi Scrum Team thực nghiệm khám phá những cách làm việc tốt hơn. Tương tự, cách dùng thích hợp của định nghĩa "Workflow" là quan trong khi dùng kết hợp với tất cả các yếu tố khác trong bản hướng dẫn này (Ví dụ, chỉ số lưu lượng (flow metrics)). Tính nhất quán đảm bảo tính toàn vẹn của siêu tập trung Kanban vào tính minh bạch.

## Thực hành Kanban:
Scrum Team đạt được sự cải tiến flow bằng cách dùng bốn thực hành sau:
* Trực quan hóa của Workflow
* hạn chế WIP
* Sự quản lý tích cực của các hạng mục công việc đang được tiến hành
* Thanh tra và thích ứng định nghĩa của họ về "Workflow"

### Trực quan hóa workflow - Bảng kanban:
Trực quan hóa thông qua bảng Kanban là cách mà Scrum Team làm cho quy trình làm việc của họ minh bạch. Sự trình bày của bảng nên nhắc nhở cuộ hội thoại phù hợp vào thời điểm phù hợp và chủ động để xuất cơ hội để cải tiến.

### Giới hạn WIP (Work in Progress):
Work in Progress (WIP) để cập đến các hạng mục công việc Scrum Team đã bắt đầu nhưng vẫn chưa hoàn thánh. Scrum Team dùng Kanban cần kiểm soát rõ ràng các hạng mục công việc in-progress  này từ thời điểm họ xem chúng là "đã bắt đầu" cho đến thời điểm họ xem chúng "đã kết thúc". Sự kiểm soát đó thường được diễn tả như 1 con số hoặc các con số trên bảng kanban. Những con số này được gọi là "WIP Limits"(Hạn chế của công việc đang tiến hành). Một WIP Limit có thể bao gồm các hạn mục công việc trong một cột đơn, Nhóm của nhiều cột, hoặc là cả một bảng. Một khi Scrum Team đã thiết lập một WIP Limit, nó kiềm chế việc kéo số lượng hạng mục công việc nhiều hơn con số đó vào một phần nhất định của Workflow. Scrum Team kiểm soát các hạn chế đó là gì và cách áp dụng chúng. tác dụng phụ chính của việc giới hạn WIP là nó tạo ra một "hệ thống kéo" (pull system). Nó được gọi là hệ thống kéo vì Scrum Team bắt đầu làm việc trên một hạng mục (tức là kèo) chỉ khi nó có dấu hiệu rõ ràng rằng đó là lúc phải làm như thế (chú ý, ở đây khác với "hệ thống đẩy" (Push system), hệ thống mà yêu cầu công việc cần bắt đầu bất cứ khi nào nó được yêu cầu). Khi WIP giảm xuống giới hạn đã xác định thì đó là tính hiểu để bắt đầu một việc mới. Bản thân Sprint là một hình thức hạn chế WIP. Bằng định nghĩa, một Sprint là một cách của việc kiểm soát bao nhiêu công việc mà một Development Team sẽ cố gắng trong một khoảng thời gian nhất định. Công việc chỉ được kéo vào một Sprint backlog khi Development Team chọn làm như thế (thông thường nhưng không phải luôn luôn, trong suốt giai đoạn kế hoạch Sprint). Cho dù dự định hay không, Scrum đã chấp nhận thực hành cơ bản này của flow từ lúc nó bắt đầu. Kanban thì chi tiết và rõ ràng hơn hạn chế WIP không chỉ giúp workflow mà còn có thể cải thiện trọng tâm của Scrum Team, cam kết, và thậm chí cộng tác hơn nữa.

### Tích cực quản lý các hạn mục công việc đang tiến hành:
Limiting WIP is a necessary component to achieve flow, but it alone is not sufficient. The third
practice to establish flow is the active management of work items in progress. Active management
can take several forms, including but not limited to the following:
• Responding quickly to blocked work items.
• Making sure that work items are only pulled into the workflow at about the same rate
that they leave the workflow.
• Ensuring work items aren't left to age unnecessarily and are completed according to an
established SLE.
• Unclogging work that piles up in a column or columns.
While many of these topics may be covered during the Daily Scrum (see the Flow-Based Daily
Scrum section below) it is the Scrum Team's responsibility to ensure the continuous proactive,
active, and reactive management of work items in progress.
### Thanh tra và thích nghi với Workflow:
## Flow Metrics and Analytics :
### Cơ bản về chỉ số lưu lượng (Metrics of Flow):
## Flow-Based Events:
### The Sprint:
### Kế hoạch Flow-Based Sprint:
### Họp Flow-Based Scrums hàng ngày:
### Sơ kết Flow-Based Sprint:
### Cải tiến Flow-Based Sprint:
## Lời kết:
## Acknowledgements:
### Lịch sử:
### Về bản dịch tiếng Việt:


[//]: #
[Scrum.org]: <https://www.scrum.org>
[Original Page]: <https://scrumorg-website-prod.s3.amazonaws.com/drupal/2018-04/2018%20Kanban%20Guide%20for%20Scrum%20Teams_0.pdf>
[Scrum Guide]: <https://www.scrumguides.org/scrum-guide.html>

