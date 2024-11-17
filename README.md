# WEBAPP
Git Workflow
Initial Setup
Create your branch
git checkout -b [yourname]
youname: viết liền ko dấu (chỉ tạo 1 lần duy nhất)

Push your branch into Github
git push origin [yourname]
Workflow
After completing any feature
git add -A 
git commit -m "Message"
git pull origin main
Resolve conflicts if any, add commit again
Push to your branch
git push origin [yourname]
Go to Github, create Pull request
Base: main , compare: yourname
Review Process
Checkout to the branch which you want to review
First time
git checkout main
git pull origin main
git checkout -b [branchname]
Later

git checkout [branchname]
Pull data from this branch to check
git pull origin [branchname]
Resolve conflicts
Add commit
Push data
Go to Github -> Request-> Add your Review -> Approve -> Merge
Lưu ý chết người:
Trước khi code phải check brand xem mình đang ở branch nào:
git status
Nếu đang ở branch main thì back về branch cá nhân:
git checkout [yourname]
Nếu lỡ làm việc trên branch main khi về branch cá nhân bị mất data local:
git merge main
để lấy data về
