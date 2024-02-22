##Quy tắc đặt tên branch
1. Tên branch nên được viết thường và không có khoảng trắng.
2. Tên branch nên mô tả một cách rõ ràng và ngắn gọn nội dung của branch đó.
3. Tên branch nên bắt đầu bằng từ "feature/" hoặc "bugfix/" tương ứng với tính năng hoặc sửa lỗi.
4. Tên branch nên được đặt dựa trên ticket hoặc issue liên quan để dễ dàng theo dõi và tìm kiếm.

> [Type]
> * feature: A new feature
> * refactor: A code change that neither fixes a bug or add a feature
> * fix: A fix bug
> * style: Change style css
> * docs: Documentation only changes
> .......

*Example*
```
  format: [Type]/[Ticket-ID]/[Branch Name]
  branchName: "feature/VWA-811-home-page"
  cmd: git checkout -b feature/VWA-811-home-page
```

##Quy tắc viết commit message
1. Độ dài commit message nên trong khoảng 50-72 ký tự.
2. Commit message nên bắt đầu bằng một động từ nguyên mẫu (ví dụ: Add, Update, Fix, Remove, Refactor, etc.)
3. Nội dung commit message nên mô tả chi tiết và đầy đủ những thay đổi đã được thực hiện.
4. Sử dụng chữ viết hoa cho ký tự đầu tiên của từ đầu tiên trong commit message.
5. Tránh sử dụng các dấu câu không cần thiết và tránh sử dụng chữ viết hoa toàn bộ câu.
6. Sử dụng mã số liên kết tới các công việc hoặc yêu cầu liên quan nếu có.
7. Sử dụng ngôn ngữ bằng tiếng Anh, tránh sử dụng tiếng lóng hoặc quá đơn giản.

*Example*
```
  format: [Ticket-ID]/[type]: [Short Message]
  commit Message: [VWA-811]/feature: UI project page and integrate API 
  cmd: git commit -m "[VWA-811]/feature: UI project page and integrate API"
```

Step by step finished task (Ticket)
> Step 1: Create new branch with format *[Type]/[Ticket-ID]/[Branch Name]* from branch with name "dev"
> Step 2: Coding
> Step 3: Testing and record evd (evidence)
> Step 4: Commit code with format *[Ticket-ID]/[type]: [Short Message]*
> Step 5: Rebase code branch dev (git pull origin dev --rebase)
> Step 5: Create PR (Pull request) to brach dev
> Step 6: Update status ticket in Jira