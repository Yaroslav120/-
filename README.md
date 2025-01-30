# Створення файлу README.md і додавання тексту
echo "# Pract_work12" >> README.md

# Ініціалізація Git репозиторію
git init

# Додавання файлу README.md до індексу
git add README.md

# Перший коміт
git commit -m "first commit"

# Перемикання на основну гілку main
git branch -M main

# Додавання віддаленого репозиторію на GitHub
git remote add origin https://github.com/Sherenok12/Pract_work12.git

# Пушити в основну гілку репозиторію на GitHub
git push -u origin main

# Додаткові кроки

# Створення нової гілки для нової фічі
git checkout -b new-feature

# Додавання змін в новій гілці
echo "New feature code" >> feature_file.txt
git add feature_file.txt

# Коміт змін
git commit -m "Added new feature"

# Пушити нову гілку на GitHub
git push -u origin new-feature

# Змішаний коміт (Squash): об'єднати кілька комітів в один перед пушем
git rebase -i HEAD~3
# Вибираєте 'squash' для останніх трьох комітів

# Скидання останніх змін (якщо потрібно відкотити останні коміти)
git reset --hard HEAD~1

# Перевірка статусу репозиторію
git status

# Перегляд історії комітів
git log --oneline

# Якщо потрібно оновити локальну копію перед пушем
git pull origin main

# Заміна вмісту remote repo (якщо зробити force push):
git push --force origin main
