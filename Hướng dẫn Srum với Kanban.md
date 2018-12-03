# Hướng dẫn dùng Kanban cho Scrum Team

Tháng 4 năm 2018

Scrum Homepage: [Scrum.org]

English version: [Original Page]

<!-- Start Document Outline -->
* [Hướng dẫn dùng Kanban cho Scrum Team](#hướng-dẫn-dùng-kanban-cho-scrum-team)
	* [Mục đích](#mục-đích)
	* [Mối liên hệ với Scrum Guide](#mối-liên-hệ-với-scrum-guide)
	* [Định nghĩa của Kanba](#định-nghĩa-của-kanba)
	* [Kanban và lí thuyết Scrum](#kanban-và-lí-thuyết-scrum)
	* [Định nghĩa của Workflow](#định-nghĩa-của-workflow)
	* [Service Level Expectation](#service-level-expectation)
	* [Thực hành Kanban](#thực-hành-kanban)
		* [Trực quan hóa workflow - Bảng kanban](#trực-quan-hóa-workflow---bảng-kanban)
		* [Giới hạn WIP (Work in Progress)](#giới-hạn-wip-work-in-progress)
		* [Tích cực quản lý các hạn mục công việc đang tiến hành](#tích-cực-quản-lý-các-hạn-mục-công-việc-đang-tiến-hành)
		* [Thanh tra và thích nghi với Workflow](#thanh-tra-và-thích-nghi-với-workflow)
	* [Flow Metrics and Analytics](#flow-metrics-and-analytics)
		* [Cơ bản về chỉ số lưu lượng (Metrics of Flow)](#cơ-bản-về-chỉ-số-lưu-lượng-metrics-of-flow)
	* [Flow-Based Events](#flow-based-events)
		* [The Sprint](#the-sprint)
		* [Kế hoạch Flow-Based Sprint](#kế-hoạch-flow-based-sprint)
		* [Họp Flow-Based Scrums hàng ngày](#họp-flow-based-scrums-hàng-ngày)
		* [Sơ kết Flow-Based Sprint](#sơ-kết-flow-based-sprint)
		* [Cải tiến Flow-Based Sprint](#cải-tiến-flow-based-sprint)
	* [Lời kết](#lời-kết)
	* [Acknowledgements](#acknowledgements)
		* [Lịch sử](#lịch-sử)
		* [Về bản dịch tiếng Việt](#về-bản-dịch-tiếng-việt)
<!-- End Document Outline -->

## Mục đích
Góc nhìn flow-based của Kanban có thể tăng cường và bổ sung cho Scrum framework và cách triển khai của nó. Team có thể áp dụng Kanban cho dù họ vừa bắt đầu dùng scrum hay đã dùng scrum trong một thời gian dài. Bản hướng dẫn Kanban cho Scrum Teams là kết quả của sự cộng tác giữa các thành viên của cộng đồng Scrum.org và các leader của cộng đồng Kanban. Cùng nhau, Họ đứng sau Bản Hướng dẫn dùng Kanban cho Scrum Teams. Đó là niềm tin chung của họ rằng các học viên phần mềm chuyên nghiệp có thể hưởng lợi từ việc áp dụng Kanban cùng với Scrum.

## Mối liên hệ với Scrum Guide
Bản hướng dẫn này không thay thế hay cắt giảm phần nào của [Scrum Guide]. Nó được thiết kế để tăng cường và mở rộng việc thực hành của Scrum framework. Bản hướng dẫn nàu giả định rằng đọc giả đang điều hành một quy trình sử dụng Scrum framework. Do đó, Toàn bộ [Scrum Guide] áp dụng vào nó.

## Định nghĩa của Kanba
Kanban (n): một chiến thuật để cải tiến dòng chảy giá trị của các bên liên quan thông qua một quy trình mà nó dùng một hệ thống trực quan, Hạn chế công việc kéo dài.

Trung tâm của định nghĩa kanba là concept(khái niệm) của "flow" (dòng chảy, luồng). Flow là sự dịch chuyên của giá trị khách hàng trên khắp hệ thống phát triển sản phẩm. Kanban cải tiến flow bằng cách nâng cao hiệu quả tổng thể, hiệu quả và khả năng dự đoán của một quy trình.
## Kanban và lí thuyết Scrum
Đầu tiên, đánh giá nhanh lý thuyết chính của [Scrum Guide]:

* Scrum được xây dựng dựa trên lý thuyết quản lý tiến trình thực nghiệm, hay thực nghiệm luận.
* Lý thuyết này chỉ ra rằng tri thức đến từ kinh nghiệm và việc ra quyết định được dựa trên những gì đã biết. 
* Ba yếu tố nòng cốt tạo thành một mô hình quản lý tiến trình thực nghiệm gồm: sự minh bạch,
thanh tra, và thích nghi.

Scrum chỉ định ràng Sprint Backlog minh bạch, nhưng nó lại cung cấp hạn chế về mặt làm thế nào để thực hiện nó. Mà nó cũng không xác định làm cách nào để xác định sự minh bạch rõ ràng cho flow của công việc vào Product Backlog, từ Product Backlog vào Sprint Backlog và bất cứ điều gì xảy ra cho công việc sau khi nó làm cho nó thành một gói tăng trưởng ("Done" increment). Đây là nơi Kanban có thể giúp đỡ. Bằng cách trực quan hóa công việc bằng một cách mới, một Scrum Team có thể áp dụng tập hợp các thực hành được đưa ra trong hướng dẫn này để có thể cải tiến chất lượng chuyển giao hiệu quả hơn. Những thực hành này vay mượn và xây dựng dựa trên các nguyên tắc của suy nghĩ gọn gàng, luồng phát triển sản phẩm và lý thuyết xếp hàng.
Một tác dụng phụ có lợi của việc cải tiến giá trị chuyển giao đó là nó cung cấp rất nhiều cơ hội để thanh tra và thích ứng quy trình và sản phẩm. Thắt chặt vòng phản hồi của khách hàng với Kanban là một chiến lượt đã được chứng minh để thực nghiệm cải thiện một quy trình.
Kanban siêu tập trung vào tính minh bạch, trực quan hóa, và luồng, kết hợp với Scrum framework, hình thành một nền tảng mạnh mẽ để thiết kế quy trình cung cấp tối ưu giá trị của khách hàng.

## Định nghĩa của Workflow
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

## Service Level Expectation

Một SLE dự báo mất bao lâu để một hạng mục chuyển từ bắt đầu đến kết thúc trong workflow của bạn. bản thân SLE có hai phần: Khoảng vài ngày trôi qua và xác suất được liên kết với khoảng thời gian đó (Ví dụ, "85% hạn mục công việc sẽ được hoàn thành trong 8 ngày hoặc ít hơn). SLE dựa trên lịch sử của chu kì thời gian của Scrum Team, và một lần tính toán, phải được đăng lên bảng Kanban. Nếu không tồn tại dữ liệu lịch sử chu kì thời gian, Scrum Team nên dự đoán một cách tốt nhất and sau đó thay thế dự đoán đó khi nó có đủ dữ liệu lịch sử để làm một tính toán SLE đúng đắn. Bất kể Scrum Team chọn cách tạo ra định nghĩa của nó về "Workflow" như thế nào đi nữa, nó là concept trung tâm của bản hướng dẫn này. Tất cả các yếu tố khác của bản hướng dẫn này phụ thuộc rất nhiều vào chính xác cách Scrum Team chỉ định định nghĩa của "Workflow". Nó có thể và nó nên thay đổi khi Scrum Team thực nghiệm khám phá những cách làm việc tốt hơn. Tương tự, cách dùng thích hợp của định nghĩa "Workflow" là quan trong khi dùng kết hợp với tất cả các yếu tố khác trong bản hướng dẫn này (Ví dụ, chỉ số lưu lượng (flow metrics)). Tính nhất quán đảm bảo tính toàn vẹn của siêu tập trung Kanban vào tính minh bạch.

## Thực hành Kanban
Scrum Team đạt được sự cải tiến flow bằng cách dùng bốn thực hành sau:
* Trực quan hóa của Workflow
* hạn chế WIP
* Sự quản lý tích cực của các hạng mục công việc đang được tiến hành
* Thanh tra và thích ứng định nghĩa của họ về "Workflow"

### Trực quan hóa workflow - Bảng kanban
Trực quan hóa thông qua bảng Kanban là cách mà Scrum Team làm cho quy trình làm việc của họ minh bạch. Sự trình bày của bảng nên nhắc nhở cuộ hội thoại phù hợp vào thời điểm phù hợp và chủ động để xuất cơ hội để cải tiến.

### Giới hạn WIP (Work in Progress)
Work in Progress (WIP) để cập đến các hạng mục công việc Scrum Team đã bắt đầu nhưng vẫn chưa hoàn thánh. Scrum Team dùng Kanban cần kiểm soát rõ ràng các hạng mục công việc in-progress  này từ thời điểm họ xem chúng là "đã bắt đầu" cho đến thời điểm họ xem chúng "đã kết thúc". Sự kiểm soát đó thường được diễn tả như 1 con số hoặc các con số trên bảng kanban. Những con số này được gọi là "WIP Limits"(Hạn chế của công việc đang tiến hành). Một WIP Limit có thể bao gồm các hạn mục công việc trong một cột đơn, Nhóm của nhiều cột, hoặc là cả một bảng. Một khi Scrum Team đã thiết lập một WIP Limit, nó kiềm chế việc kéo số lượng hạng mục công việc nhiều hơn con số đó vào một phần nhất định của Workflow. Scrum Team kiểm soát các hạn chế đó là gì và cách áp dụng chúng. tác dụng phụ chính của việc giới hạn WIP là nó tạo ra một "hệ thống kéo" (pull system). Nó được gọi là hệ thống kéo vì Scrum Team bắt đầu làm việc trên một hạng mục (tức là kèo) chỉ khi nó có dấu hiệu rõ ràng rằng đó là lúc phải làm như thế (chú ý, ở đây khác với "hệ thống đẩy" (Push system), hệ thống mà yêu cầu công việc cần bắt đầu bất cứ khi nào nó được yêu cầu). Khi WIP giảm xuống giới hạn đã xác định thì đó là tính hiểu để bắt đầu một việc mới. Bản thân Sprint là một hình thức hạn chế WIP. Bằng định nghĩa, một Sprint là một cách của việc kiểm soát bao nhiêu công việc mà một Development Team sẽ cố gắng trong một khoảng thời gian nhất định. Công việc chỉ được kéo vào một Sprint backlog khi Development Team chọn làm như thế (thông thường nhưng không phải luôn luôn, trong suốt giai đoạn kế hoạch Sprint). Cho dù dự định hay không, Scrum đã chấp nhận thực hành cơ bản này của flow từ lúc nó bắt đầu. Kanban thì chi tiết và rõ ràng hơn hạn chế WIP không chỉ giúp workflow mà còn có thể cải thiện trọng tâm của Scrum Team, cam kết, và thậm chí cộng tác hơn nữa.

### Chủ động quản lý các hạn mục công việc đang tiến hành
Limiting WIP là một thành phần quan trọng để đạt được flow, nhưng một mình nó thì không đủ. Thực hành thứ ba để thiết lập flow là sự Chủ động quản lý của các hạng mục đang tiến hành. Sự Chủ động quản lý có thể có nhiều hình thức, bao gồm nhưng không giới bị giới hạn tới các mục sau:
* Phản hồi nhanh đến các công việc bị chặn.
* Chắc rằng các hạng mục công việc chỉ được kéo vào workflow ở tỷ lệ gần bằng tỷ lệ chúng rời khỏi workflow.
* Đảm bảo các hạng mục công việc không được kéo dài không cần thiết và được hoàn thành theo một thiết lập SLE.
* Ngắt công việc mà nó chất đống trong một cột hoặc nhiều cột.
Mặc dù nhiều chủ đề trong số này được đề cập trong quá trình Daily Scrum (Xem [Họp Flow-Based Scrums hàng ngày](#họp-flow-based-scrums-hàng-ngày)) đó là trách nhiệm của Scrum Team để đảm bảo tính chủ động liên tục, chủ động, và tái chủ động quản lý của các hạng mục công việc đang tiến hành.

### Thanh tra và thích nghi với Workflow
Hãy nghĩ chính sách như là "Luật lệ của trò chơi" cho "Workflow" của Scrum Team. Những thay đổi nhỏ đến những chính sách có thể có tác động vật chất đến cách Scrum Team thực hiện tổng thể. 
[Scrum Guide] cung cấp một tập hợp@ tối thiểu của các chính sách rõ ràng cũng như hướng dẫn cách tìm ra vài chính sách "context-specific"(khái niệm cụ thể) (Ví dụ, định nghĩa về Done của Scrum Team). 
Khi áp dụng Kanban, Scrum Team sẽ muốn bổ sung [Scrum Guide] với các chính sách rõ ràng hơn cho quy trình của mình.
Những chính sách đó sẽ được bắt gặp trong một định nghĩa "Workflow" của Scrum Team. 
Rõ ràng nghĩa là những chính sách này đước viết ra hoặc được trực quan hóa bằng cách nào đó và cả Scrum Team hiểu chúng. 
Bảng Kanban nên hiển thị tất cả những chính sách liên quan hoặc hướng cho những thành viên của Scrum Team tìm chúng ở đâu.
Một ví dụ điển hình về một chính sách cần phải rõ ràng là cách Scrum Team xác định thời điểm khi các mục đi từ chưa được bắt đầu đến bắt đầu và từ trong tiến trình đi đến đã hoàn thành. Không nghi ngờ gì khi Scrum Team sẽ thêm vào các chính sách khác trên đầu của những chính sách cụ thể được gọi trong bản hướng dẫn này. 

## Flow Metrics and Analytics
Việc áp dụng Kanban trong Scrum Context yêu cầu thu thập và phân tích tập hợp chỉ số lưu lượng tối thiểu. Những chỉ số này là cần thiết cho thực hành của quản lý chủ động của các hạng mục công việc trong tiến trình. Nó cũng làm cho tính minh bạch của flow và cho phép định hướng luồng thanh tra và thích ứng. Những chỉ số này phản ánh sức sống và hiệu suất hiện tại của hướng tiếp cận của Scrum Team. Họ cũng sẽ chỉ ra các can thiệp có thể cải thiện chức năng của nhóm Scrum và giá trị mà nó mang lại.

### Cơ bản về chỉ số lưu lượng (Metrics of Flow)
Bốn chỉ số cơ bản của flow mà Scrum teams dùng Kanban sẽ cần để track là những điều sau:
* Work in Progress (WIP): Số lượng các công việc đã được bắt đầu nhưng chưa được hoàn thành () The number of work items started but not finished (Theo định nghĩa "Workflow" của Scrum Team).
* Cycle Time (Vòng thời gian): Lượng thời gian trôi qua giữa thời điểm mục công việc "bắt đầu" và khi nào mục công việc "kết thúc".
* Work Item Age (Tuổi thọ mục công việc): Lượng thời gian trôi qua giữa thời điểm mục công việc "đã bắt đầu" và thời điểm hiện tại.
* Throughput (Thông lượng): Số lượng của các mục công việc đã hoàn thành trên đơn vị thời gian. Lưu ý việc đo lường thông lượng là số lượng công việc chính xác.

Tính toán các vòng thời gian và tuổi mục công việc yêu cầu Scrum Team (ở mức ít nhất) trach ngày bắt đầu và ngày đã hoàn thành của mỗi mục công việc.
Nhưng chỉ số này cần được giám sát trong suốt Sprint - đặc biệt là trong Scrum Event (xem [Flow-Based Events](#flow-based-events)). Như thường lệ, Nó còn có nhiều chỉ số khác mà Scrum Team cần xem xét, nhưng trên đây là những yêu cầu tối thiểu.

## Flow-Based Events
Kanban trong Scrum Context không yêu cầu bất kì sự kiện bổ sung nào cho các sự kiện được nêu trong [Scrum Guide]. Tuy nhiên dùng quan điểm flow-based có thể tăng cường cho các sự kiện Scrum.

### The Sprint
Một Sprint là một nhịp điệu hoặc một "nhịp tim" đều đặn cho sự thanh tra và sự thích nghi. 
Chu kì đều đặn và các phần tử của Sprint phù hợp một cách tự nhiên với quy trình quản lý. 
Một Sprint chứa kế hoạch Sprint (Sprint Planning), Họp Scrum hàng ngày (Daily Scrum), công việc phát triển, Sơ kết Sprin (Sprint Review), và hồi tưởng Sprint (Sprint Retrospective).
Các sự kiện trong một Sprint có thể làm việc như một vòng lặp phản hồi (feedback loop) cho sự thanh tra chỉ số Kanban flow, và hướng tiếp cận Kanban cũng có thể hoạt động như một vòng lặp phản hổi (feedback loop) cho sự thanh tra trong triển khai Scrum.

### Kế hoạch Flow-Based Sprint
Một cuộc họp kế hoạch Sprint flow-based dùng các chỉ số flow như một sự trợ giúp để phát triển Sprint Backlog. Ví dụ, dùng lịch sử thông lượng để hiểu sức chứa của Scrum Team cho Sprint tiếp theo. Một SL của Scrum Team có thể ảnh hưởng đến công việc đã lên kế hoạch cho những ngày đầu tiền của Sprint.

### Họp Flow-Based Scrums hàng ngày
Một cuộc họp Scrum flow-based  hàng ngày tập trung vào việc đảm bảo Scrum Team làm tất cả những gì nó có thể để duy trì flow mỗi ngày. Trong khi goal của họp Scrum hàng ngày vẫn như cũ như của [Scrum Guide], bản thân cuộc họp diễn ra xung quanh bảng kanban và tập trung vào chỗ mà flow bị thiếu sót và bằng những cách nào mà Scrum Team có thể làm cho dòng chảy công việc chảy trở lại.
Vài điều bổ sung để xem xét trong thời gian một Flow-based Daily Scrum như sau:

* Những hạng mục công việc nào đang bị chặn và những gì Scrum Team có thể làm để làm cho nó không bị chặn đứng?
* Tuổi đời của mỗi hạng mục công việc đang tiến hành là gì? Các mục công việc nào đã vi phạm hoặc sắp vi phạm SLE của chúng và Scrum Team có thể làm gì để công việc đó có thể được hoàn thành? 

• Có bất kỳ điều gì có thể ảnh hưởng đến khả năng để hoàn thành công việc hôm nay của Scrum Team mà không được thể hiện trên bảng không?

### Sơ kết Flow-Based Sprint
[Scrum Guide] cung cấp một phác thảo chi tiết của chu trình sơ kết Sprint. Ngoài các hoạt động này ra, Thanh tra chỉ số lưu lượng kanban như một phần của sơ kết Sprint tạo ra cơ hội cho những cuộ hội thoại mới về giám sát tiến trình để đi đến goal.
Xem xet thông lượng có thể cung cấp vài thông tin bổ sung khi Chủ sản phẩm (PO) thảo luận về mục tiêu và ngày có khả năng chuyển giao hàng.
Sơ kết một SLE của Scrum Team có thể làm cho Chủ sản phẩm (PO) sửa đổi Product Backlog.

### Cải tiến Flow-Based Sprint
A flow-based Sprint Retrospective adds the inspection of flow metrics and analytics to help
determine what improvements the Scrum Team can make to its processes, including the Sprint
Retrospective itself. The Scrum Team using Kanban also inspects and adapts the definition of
“Workflow” to optimize the flow in the next Sprint. Using a cumulative flow diagram to visualize
a Scrum Team’s Work in Progress, average approximate Cycle Time and average Throughput may
be valuable.
The Scrum Guide dictates that the Sprint Retrospective take place after the Sprint Review and
before the next Sprint Planning. This does not change when using Kanban. However, flow-based
retrospective opportunities need not coincide within the boundaries of a Sprint. They can occur
"just in time”. Correspondingly, changes to a team’s definition of “Workflow” may happen at any
time, however, as these changes will have a material impact on how the Scrum Team performs,
changes made during the regular cadence provided by the Sprint Retrospective event will reduce
complexity and improve transparency.

## Lời kết
Scrum is not a process or technique. It is a framework within which people can address complex
adaptive problems, while productively and creatively delivering products of the highest possible
value. As The Scrum Guide points out, it functions well as a container for other techniques,
methodologies, and practices. 
The flow optimization practices of Kanban provide Scrum Teams with additional opportunities to
inspect the right thing, at the right time, and then based on that inspection, adapt as needed.
Kanban's hyperfocus on transparency, visualization, and flow maximizes feedback, empiricism,
and ultimately the delivery of customer value.
## Acknowledgements
### Lịch sử
The set of practices commonly referred to as Kanban mostly originated on a team at Corbis in 2006. Those practices quickly spread to encompass a large and diverse international community
who over the years continued to enhance and evolve the approach.
This guide was developed collaboratively by Scrum.org, our Professional Scrum Trainer
Community, Steve Porter, Yuval Yeret, and Daniel Vacanti.
A special thank you to Louis-Philippe Carignan and Charles Bradley for their contributions in this
effort. We also owe a debt of gratitude to all those practitioners who have in the past contributed
to make Kanban a viable and successful lean-agile strategy. 

### Về bản dịch tiếng Việt


[//]: #
[Scrum.org]: <https://www.scrum.org>
[Original Page]: <https://scrumorg-website-prod.s3.amazonaws.com/drupal/2018-04/2018%20Kanban%20Guide%20for%20Scrum%20Teams_0.pdf>
[Scrum Guide]: <https://www.scrumguides.org/scrum-guide.html>

