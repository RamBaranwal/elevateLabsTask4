git init
git add .
git commit -m "Initial project setup"

git branch -M main
git checkout -b dev
git checkout -b feature/add-documentation

git add project.md
git commit -m "Add Git best practices documentation"

git remote add origin <repository-url>

git push -u origin main
git push -u origin dev
git push -u origin feature/add-documentation

git pull origin dev
git pull origin main

git tag -a v1.0.0 -m "Task 4 final version"
git push origin v1.0.0

git branch -a
git log --oneline --graph --all
git tag