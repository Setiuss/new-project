# PowerShell

# Створіть в своєму середовищі новий каталог з назвою "new-project".
New-Item -ItemType Directory -Path .\new-project

# Ініціалізуйте новий публічний Git-репозиторій всередині каталогу "new-project".
git init new-project

# Перейдіть до каталогу "new-project".
sl .\new-project\

# Створіть новий файл з назвою "README.md" і додайте до нього початковий текст.
New-Item -ItemType File -Path .\README.md

# Підготуйте файл "README.md" до коміту.
# Закомітьте зміни у репозиторій з коміт повідомленням “init”.
git commit -m "init"

# Створіть нову гілку з назвою "development" і перейдіть до неї.
New-Item -ItemType Directory -Path .\development
sl .\development\

# Додайте інструкцію до файлу "README.md" і підготуйте їх до коміту.
# Закомітьте зміни у гілці "development" з повідомленням про коміт.
git add README.md
git commit -m "create folder development"

# Об'єднайте зміни з гілки "development" у гілку "main".

# Перевірте статус, переконайтеся, що все актуально.
git status

# Закомітьте зміни
git commit -a