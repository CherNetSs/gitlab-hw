# Задание 1

## Выполненные действия

### 1. Использование существующего GitHub-аккаунта

Для выполнения задания был использован ранее зарегистрированный аккаунт на [GitHub](https://github.com?utm_source=chatgpt.com).

---

### 2. Создание публичного репозитория

Был создан отдельный публичный репозиторий с инициализацией файла `README.md`.

---

### 3. Клонирование репозитория

Репозиторий был склонирован на локальный компьютер по HTTPS:

```bash
git clone https://github.com/USERNAME/git-hw.git
```

Переход в каталог репозитория:

```bash
cd git-hw
```

---

### 4. Первоначальная настройка Git

```bash
git config --global user.name "Артем Чернецов"
git config --global user.email "YOUR_EMAIL@example.com"
```

Проверка настроек:

```bash
git config --global --list
```

---

### 5. Проверка состояния репозитория

```bash
git status
```

Результат:

```text
On branch main
nothing to commit, working tree clean
```

---

### 6. Редактирование README.md

Файл `README.md` был изменён.

После редактирования выполнена повторная проверка:

```bash
git status
```

Результат:

```text
modified: README.md
```

---

### 7. Просмотр изменений

```bash
git diff
```

```bash
git diff --staged
```

---

### 8. Добавление файла в staged

```bash
git add README.md
```

Проверка состояния:

```bash
git status
```

---

### 9. Повторная проверка изменений

```bash
git diff
```

```bash
git diff --staged
```

---

### 10. Создание commit

```bash
git commit -m "First commit"
```

---

### 11. Отправка изменений на GitHub

```bash
git push origin main
```

---

## Ссылка на commit


[Ссылка на commit](https://github.com/CherNetSs/gitlab-hw/commit/0c64e1a1d1060e80138ebcb9b0a628f4972228e0)


# Задание 2

## Создание файла .gitignore

Был создан файл `.gitignore`.

Проверка статуса репозитория:

```bash
git status
```

Результат:

```text
Untracked files:
  .gitignore
```

---

## Добавление правил игнорирования

В файл `.gitignore` были добавлены правила:

```gitignore
*.pyc
cache/
```

Данные правила:

* игнорируют все файлы с расширением `.pyc`;
* игнорируют директорию `cache` и всё её содержимое.

---

## Добавление файла в commit

```bash
git add .gitignore
```

---

## Создание commit

```bash
git commit -m "added gitignore"
```

---

## Отправка изменений на GitHub

```bash
git push
```

---

## Ссылка на commit

[Ссылка на commit](https://github.com/CherNetSs/gitlab-hw/commit/4e3d804d775bb285d8b12fb87f8a4d974a036b5b)


# Задание 3

## Работа с ветками

Была создана новая ветка `dev`:

```bash
git checkout -b dev
```

В ветке `dev` был создан файл `test.sh`:

```bash
#!/bin/bash
echo "Dev version 1"
```

Был выполнен первый commit и push:

```bash
git add test.sh
git commit -m "add test script"
git push -u origin dev
```

Затем файл `test.sh` был изменён:

```bash
#!/bin/bash
echo "Dev version 1"
echo "Dev version 2"
```

Был выполнен второй commit и push:

```bash
git add test.sh
git commit -m "update test script"
git push
```

---

## Работа в основной ветке

После этого выполнено переключение в основную ветку:

```bash
git checkout main
```

В основной ветке был создан файл `main.sh`:

```bash
#!/bin/bash
echo "Main branch script"
```

Был выполнен commit и push:

```bash
git add main.sh
git commit -m "add main script"
git push
```

---

## Слияние ветки dev в main

Ветка `dev` была объединена с основной веткой:

```bash
git merge dev --no-ff
```

Сообщение merge commit:

```text
Merge dev branch into main
```

После этого изменения были отправлены на GitHub:

```bash
git push
```

---

## Ссылка на граф коммитов

[Граф коммитов](https://github.com/CherNetSs/gitlab-hw/network)
