# Как загрузить Vegas на GitHub

## Шаг 1: Создай репозиторий на GitHub

1. Перейди на github.com
2. Кликни "+ New" → New repository
3. Назови его: `vegas-android`
4. Description: "AI Agent for Android"
5. Выбери Public
6. **НЕ** инициализируй README, .gitignore, license
7. Кликни "Create repository"

## Шаг 2: Загрузи код в Termux

```bash
cd ~/vegas-android
git init
git add .
git commit -m "Initial commit: Vegas MVP"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/vegas-android.git
git push -u origin main
```

Замени `YOUR_USERNAME` на своё имя пользователя GitHub.

## Шаг 3: Проверь GitHub Actions

1. Перейди на страницу репозитория
2. Кликни на вкладку "Actions"
3. Найди workflow "Build Vegas APK"
4. Жди, пока закончится сборка (2-3 минуты)
5. Должно быть **BUILD SUCCESSFUL** ✓

## Шаг 4: Скачай APK

1. Кликни на успешную сборку
2. Внизу будет секция "Artifacts"
3. Кликни "Vegas-debug" → Download
4. Распакуй ZIP и установи на телефон

---

**Готово!** Теперь Vegas собирается автоматически при каждом push 🚀

Все файлы проекта находятся в папке `/home/claude/vegas-android`
