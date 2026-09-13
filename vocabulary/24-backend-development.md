# Từ vựng chuyên ngành: Backend Development

Danh sách thuật ngữ chuyên sâu dành cho backend developer — vượt ra ngoài từ vựng lập trình chung ở [20-software-development.md](20-software-development.md). Dùng để đọc tài liệu kỹ thuật, viết báo cáo/PR description, và giao tiếp trong team kỹ thuật quốc tế.

## 1. Cơ sở dữ liệu (Databases)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **schema** | lược đồ dữ liệu | We need to update the database *schema* before deploying. |
| **query** | truy vấn | This *query* is taking too long to execute. |
| **index (database)** | chỉ mục | Adding an *index* on that column sped up the query significantly. |
| **primary key / foreign key** | khóa chính / khóa ngoại | Each table needs a *primary key*. |
| **normalization** | chuẩn hóa dữ liệu | We applied *normalization* to reduce data duplication. |
| **denormalize** | phi chuẩn hóa | We *denormalized* the table for faster read performance. |
| **transaction** | giao dịch (CSDL) | Wrap those operations in a single *transaction*. |
| **rollback / commit** | hoàn tác / xác nhận (giao dịch) | If the update fails, the system will automatically *roll back*. |
| **ACID (compliance)** | tuân thủ nguyên tắc ACID | The database guarantees *ACID* compliance for transactions. |
| **migration (database)** | di chuyển/thay đổi cấu trúc CSDL | Run the *migration* before starting the server. |
| **seed data** | dữ liệu khởi tạo mẫu | We use *seed data* for local development. |
| **connection pool** | nhóm kết nối (CSDL) | The app ran out of connections because the *connection pool* was too small. |
| **replica / replication** | bản sao / sao chép dữ liệu | We set up read *replicas* to reduce load on the main database. |
| **sharding** | phân mảnh dữ liệu | The team implemented *sharding* to scale the database horizontally. |
| **ORM (Object-Relational Mapping)** | ánh xạ đối tượng-quan hệ | We use an *ORM* instead of writing raw SQL. |
| **NoSQL** | cơ sở dữ liệu phi quan hệ | We chose a *NoSQL* database for this use case. |
| **stored procedure** | thủ tục lưu trữ | The legacy system relies heavily on *stored procedures*. |
| **deadlock** | tình trạng khóa chéo | Two transactions caused a *deadlock*. |
| **cache invalidation** | vô hiệu hóa bộ nhớ đệm | *Cache invalidation* is one of the hardest problems in computer science. |

## 2. API & Dịch vụ web (APIs & Web Services)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **endpoint** | điểm cuối (API) | This *endpoint* returns user data in JSON format. |
| **request / response** | yêu cầu / phản hồi | The server sent back a 500 error in the *response*. |
| **payload** | dữ liệu gửi kèm (request/response) | Check the *payload* to see what data was sent. |
| **REST / RESTful** | kiến trúc REST | We designed the API to be fully *RESTful*. |
| **GraphQL** | ngôn ngữ truy vấn API GraphQL | We migrated from REST to *GraphQL* for more flexible queries. |
| **status code** | mã trạng thái HTTP | A *status code* of 404 means the resource wasn't found. |
| **rate limiting** | giới hạn tần suất truy cập | We added *rate limiting* to prevent abuse. |
| **webhook** | webhook (gọi lại tự động) | The payment provider sends a *webhook* when a transaction completes. |
| **authentication / authorization** | xác thực / phân quyền | You need proper *authentication* to access this endpoint. |
| **token (JWT)** | mã token (JWT) | The API requires a valid *JWT token* in the header. |
| **idempotent** | bất biến (gọi nhiều lần vẫn ra cùng kết quả) | This endpoint is *idempotent* — retrying it is safe. |
| **versioning (API)** | đánh phiên bản API | We follow strict *API versioning* to avoid breaking clients. |
| **serialize / deserialize** | tuần tự hóa / giải tuần tự hóa | The object is *serialized* into JSON before sending. |
| **middleware** | phần mềm trung gian | This *middleware* logs every incoming request. |
| **third-party integration** | tích hợp bên thứ ba | We built a *third-party integration* with the shipping provider. |

## 3. Server & Hạ tầng (Server & Infrastructure)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **load balancer** | bộ cân bằng tải | The *load balancer* distributes traffic across multiple servers. |
| **container (Docker)** | container (đóng gói ứng dụng) | We package our app into a *container* for consistent deployment. |
| **orchestration (Kubernetes)** | điều phối container | We use Kubernetes for *orchestration* across our cluster. |
| **cluster** | cụm máy chủ | The application runs on a three-node *cluster*. |
| **node** | nút (một máy trong cụm) | One of the *nodes* in the cluster went down. |
| **instance** | phiên bản máy chủ (ảo) | We spun up a new EC2 *instance* to handle the extra load. |
| **provisioning** | cấp phát tài nguyên | *Provisioning* new servers now takes just a few minutes. |
| **infrastructure as code (IaC)** | hạ tầng dưới dạng mã | We manage our infrastructure using *IaC* tools like Terraform. |
| **CI/CD pipeline** | quy trình tích hợp/triển khai liên tục | Every push triggers our *CI/CD pipeline* automatically. |
| **environment (dev/staging/prod)** | môi trường (phát triển/thử nghiệm/thực tế) | Test it in *staging* before deploying to *production*. |
| **rollback (deployment)** | quay lại phiên bản trước | We had to *roll back* the deployment after the incident. |
| **hotfix** | bản sửa lỗi khẩn cấp | We pushed a *hotfix* to fix the critical bug. |
| **monitoring / observability** | giám sát / khả năng quan sát hệ thống | Good *observability* helped us catch the issue early. |
| **logging** | ghi log | We centralized all our *logging* in one dashboard. |
| **alerting** | cảnh báo tự động | The *alerting* system paged the on-call engineer immediately. |
| **on-call (duty)** | trực (xử lý sự cố) | I'm *on-call* this weekend. |
| **incident** | sự cố (hệ thống) | We're still investigating the root cause of the *incident*. |
| **postmortem** | báo cáo phân tích sự cố sau khi xảy ra | We wrote a *postmortem* after the outage. |
| **SLA (Service Level Agreement)** | thỏa thuận mức dịch vụ | We're required to meet a 99.9% *SLA*. |

## 4. Kiến trúc hệ thống (System Architecture)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **microservices** | kiến trúc vi dịch vụ | We broke the monolith into *microservices*. |
| **monolith / monolithic** | kiến trúc nguyên khối | The old system is a huge *monolith*, hard to maintain. |
| **message queue** | hàng đợi tin nhắn | We use a *message queue* to process orders asynchronously. |
| **event-driven (architecture)** | kiến trúc hướng sự kiện | The system follows an *event-driven* architecture. |
| **asynchronous / synchronous** | bất đồng bộ / đồng bộ | This task runs *asynchronously* in the background. |
| **decoupling** | tách rời (giữa các thành phần) | *Decoupling* the services made the system easier to scale. |
| **single point of failure** | điểm lỗi duy nhất (gây sập cả hệ thống) | This service is a *single point of failure* — we need redundancy. |
| **fault tolerance** | khả năng chịu lỗi | The system is designed with *fault tolerance* in mind. |
| **latency** | độ trễ | We reduced *latency* by caching frequent queries. |
| **throughput** | thông lượng (xử lý) | The new system handles much higher *throughput*. |
| **scalability (horizontal/vertical)** | khả năng mở rộng (theo chiều ngang/dọc) | We scaled *horizontally* by adding more servers. |
| **technical debt** | nợ kỹ thuật | We accumulated a lot of *technical debt* rushing that feature. |
| **legacy system** | hệ thống cũ, lỗi thời | Maintaining the *legacy system* takes up a lot of our time. |
| **refactor** | tái cấu trúc mã | We need to *refactor* this module — it's hard to maintain. |
| **design pattern** | mẫu thiết kế | The team follows common *design patterns* for consistency. |

## 5. Quy trình & Cộng tác nhóm (Workflow & Team Collaboration)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **pull request (PR)** | yêu cầu hợp nhất mã | Please review my *pull request* when you get a chance. |
| **code review** | rà soát mã nguồn | This PR still needs a *code review* before merging. |
| **merge conflict** | xung đột khi hợp nhất | I ran into a *merge conflict* on this branch. |
| **sprint** | chu kỳ làm việc (Scrum) | We're planning the next *sprint* on Monday. |
| **backlog** | danh sách công việc chưa làm | This task is still in the *backlog*. |
| **ticket / issue** | công việc/lỗi được ghi nhận | I'm working on *ticket* #452 today. |
| **standup (meeting)** | họp ngắn hằng ngày | We have a *standup* every morning at 9. |
| **spike (investigation)** | tìm hiểu/nghiên cứu kỹ thuật | We did a *spike* to evaluate the new library. |
| **blocked (on)** | bị chặn (chưa thể làm tiếp) | I'm *blocked on* this task until the API is ready. |
| **technical specification (tech spec)** | tài liệu đặc tả kỹ thuật | Please write a *tech spec* before starting implementation. |
| **edge case** | trường hợp đặc biệt/hiếm gặp | Did you handle the *edge case* where the input is empty? |
| **regression (bug)** | lỗi tái diễn (do thay đổi mới) | This update introduced a *regression* in the login flow. |

## 6. Kiểm thử & Chất lượng (Testing & Quality)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **unit test** | kiểm thử đơn vị | Make sure to add *unit tests* for this function. |
| **integration test** | kiểm thử tích hợp | The *integration tests* check how services work together. |
| **mock (data/object)** | dữ liệu/đối tượng giả lập | We used a *mock* API to test the frontend independently. |
| **test coverage** | độ phủ kiểm thử | Our *test coverage* dropped after the last release. |
| **staging environment** | môi trường thử nghiệm | Always test in the *staging environment* first. |
| **QA (Quality Assurance)** | đảm bảo chất lượng | *QA* found a bug before it reached production. |
| **flaky test** | bài test không ổn định (lúc pass lúc fail) | This *flaky test* keeps failing randomly in CI. |
| **load testing** | kiểm thử tải | We ran *load testing* before the big sale event. |

## 7. Bảo mật (Backend Security)

| Từ / Cụm từ | Nghĩa | Ví dụ |
|---|---|---|
| **SQL injection** | tấn công chèn mã SQL | Always sanitize input to prevent *SQL injection*. |
| **input validation / sanitization** | kiểm tra/làm sạch dữ liệu đầu vào | Proper *input validation* prevents many security issues. |
| **hashing** | băm dữ liệu (mật khẩu...) | Passwords should always be stored using *hashing*, not plain text. |
| **environment variable** | biến môi trường | Store your API keys in *environment variables*, not in the code. |
| **least privilege (principle)** | nguyên tắc đặc quyền tối thiểu | Follow the *principle of least privilege* when assigning permissions. |
| **vulnerability** | lỗ hổng bảo mật | The scan found a *vulnerability* in an outdated library. |
| **penetration testing (pen test)** | kiểm thử xâm nhập | We hired a firm to do *penetration testing* on our app. |
| **CORS** | chia sẻ tài nguyên chéo nguồn | We had to configure *CORS* to allow requests from the frontend. |
| **rate limiting** | *(xem mục 2)* | |

## Bài tập nhỏ

Điền từ thích hợp:

1. The team added an ______ on that column to speed up the query.
2. This endpoint requires a valid ______ in the request header for authentication.
3. We broke the old ______ into smaller, independent services.
4. The system has a ______ — if that one server fails, everything goes down.
5. We ran ______ to make sure the system could handle Black Friday traffic.
6. Never store passwords in plain text — always use ______.
7. We use a ______ to distribute incoming traffic across multiple servers.
8. This PR still needs a ______ before it can be merged.
9. We wrote a ______ after the outage to understand what went wrong.
10. This task is ______ until the design team finishes the mockups.

<details>
<summary>Đáp án</summary>

1. index
2. token (JWT)
3. monolith
4. single point of failure
5. load testing
6. hashing
7. load balancer
8. code review
9. postmortem
10. blocked

</details>
