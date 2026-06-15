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

Ссылка на commit:

`https://github.com/CherNetSs/gitlab-hw/commit/0c64e1a1d1060e80138ebcb9b0a628f4972228e0``text
```
