# Push_Code_To_Github
* Các bước để đẩy code lên github :
- Tạo repository
- Vào cmd, tìm đường dẫn muốn đẩy code
- Tạo folder .git bằng câu lệnh git init
- Liên kết folder trên máy vs repository bằng câu lệnh :
 	git remote add origin https://github.com/ChillMyMan/<Tên_repository>.git 
- Đẩy tất cả code lên repository bằng lệnh “git add .” với dấu chấm thể hiện cho tất cả các file
- Thêm tin nhắn bằng lệnh “git commit -m “<Text>””
- Hoàn thành việc đẩy bằng câu lệnh “git push -u origin main”
Chú ý : Nếu trong repository không có main thì tạo main bằng câu lệnh “git branch –m main”
	Sau đó, sử dụng lại câu lệnh “git push -m origin main” để hoàn thành
* Sửa đổi code : 
- Sau khi sửa đổi code, ta thêm câu lệnh “git add .” để github đồng bộ code với máy tính
* Nếu xảy ra lỗi 2 branch commit, ta sử dụng câu lệnh “git pull –rebase <tên_branch>” để merge 2 branch
   Sau đó push lại để đẩy code lên github
 * Nếu gặp lỗi  ![rejected]  main-> main (non-fast-forward) :
- git fetch origin main:tmp
- git rebase tmp
- git push -u origin main
