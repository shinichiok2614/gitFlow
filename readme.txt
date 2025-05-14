--
public key
git status
git init
git add .
git commit -m "first commit"
git remote add origin git@github.com:shinichiok2614/projectMovie.git
git push 
git push --set-upstream origin master
--
hello world
issue
    Tuan - add file cart.model.js #1
    submit new issue
git branch develop
git branch
git checkout develop
git push -u origin develop //cập nhật branch develop lên remote

git branch feature/1-add-file-cart
git checkout -b feature/1-add-file-cart develop   //tách nhánh trên nhánh develop
git add cart.model.js 
git commit -m '#1 - Tuan add file cart'  
git push     

Code>Compare & pull request-->Comparing changes  -->* chuyển nhánh qua develop** chứ không phải main
Add a description: I do! #1 
create pull request
-->This branch has no conflicts with the base branch
Add a comment: Good job!-->comment
merge pull request

git checkout develop
git pull

git checkout -b release-1.0.0 develop  //tạo release trước
git tag 'v1.0.0'
git push --tags

git merge develop                      //xong mới merge develop qua nó
git push --set-upstream origin relase-1.0.0

//Compare release qua main

git checkout main
git pull
git tag 'v1.0.0'
git push --tags

git branch -d release-1.0.0              //xoá ở local
git push origin -d release-1.0.0         //xoá ở remote
git branch -d feature/1-add-cart
git push origin -d feature/1-add-cart

hehe

 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git config --global user.name 'Linh Huynh'                 
 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git config --global user.email 'huynhdanglinh1988@gmail.com' 
 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git config user.name
Linh Huynh
 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git config user.email
huynhdanglinh1988@gmail.com
 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git status    ░▒▓ ✔ 
On branch feature/30-update-main
Your branch is up to date with 'origin/feature/30-update-main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   BT.QuanLyDeTai - form Main va Login/QuanLyDeTai/Main.cs

 ~/De/r/QuanLyDeTaiKhoaHoc  feature/30-update-main +1 ▓▒░ git commit -m '#30 - Kien update form main'
[feature/30-update-main 1c8fed2] #30 - Kien update form main
 1 file changed, 1 insertion(+)

--
Nếu bạn vừa mới code sai và muốn quay lại thời điểm code còn đúng trước đó, bạn có thể làm theo 1 trong 3 cách sau tùy tình huống, đảm bảo an toàn và không mất code trừ khi bạn muốn xoá.

📌 Trường hợp 1: Bạn chưa commit (chỉ mới chỉnh sửa file)
👉 Dùng lệnh sau để hoàn tác tất cả thay đổi và quay về trạng thái commit gần nhất:

git restore .

Hoặc để chỉ hoàn tác 1 file:

git restore path/to/file.js

🔴 Lưu ý: Mất toàn bộ thay đổi chưa lưu commit. Nếu muốn backup, nên copy thư mục trước.

📌 Trường hợp 2: Bạn đã commit nhưng muốn quay lại commit trước đó
➤ Giữ lại thay đổi để chỉnh sửa lại:
git reset --soft HEAD~1
Quay lại commit trước nhưng giữ code trong staged.

➤ Hoặc quay lại commit trước đó và giữ code nhưng không staged:

git reset --mixed HEAD~1

➤ Nếu bạn chắc chắn muốn xoá toàn bộ thay đổi:

git reset --hard HEAD~1

⚠️ Dùng --hard sẽ xoá sạch mọi thay đổi kể từ commit đó — không thể khôi phục lại nếu không backup.

📌 Trường hợp 3: Bạn biết commit đúng là commit nào trong git log
Xem danh sách commit:

git log --oneline

Ví dụ:

a1b2c3d Fix login issue
9f8e7g6 Add new feature (code sai)
Quay lại commit đúng (ví dụ a1b2c3d):

git reset --hard a1b2c3d

✅ Nếu muốn khôi phục code nhưng không thay đổi lịch sử:
Tạo 1 nhánh mới từ commit đúng:

git checkout -b recovery a1b2c3d
--
