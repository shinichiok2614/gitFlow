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
