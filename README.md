git checkout develop
git checkout -b feature/complex-integration
echo "def new_function():\n    pass" >> featureX.py
echo "# Bug fixed" >> bugfix.py
echo "## Оновлено документацію" >> README.md
git add featureX.py bugfix.py README.md 
git commit -m "Додано нову функцію, виправлено помилку та оновлено документацію" 
git checkout develop
git pull origin develop
git merge feature/team-member
git checkout feature/complex-integration
git rebase develop
git add <conflict-file>
git rebase --continue
git rebase -i develop
git checkout develop
git merge --no-ff feature/complex-integration -m "Об'єднання гілки feature/complex-integration"
git push origin develop
git log --oneline
