
# Шпаргалка по Git

## Основные команды

- `git init` — инициализация нового репозитория.
- `git add <file>` — добавление файла в индекс (стейджинг).
- `git commit -m "Сообщение"` — создание коммита.
- `git status` — проверка состояния репозитория.
- `git log` — просмотр истории коммитов.
- `git clone <url>` — клонирование удаленного репозитория.
- `git push` — отправка изменений на удаленный сервер.
- `git pull` — получение изменений с удаленного репозитория.

## Работа с ветками

- `git branch` — список веток.
- `git checkout -b <branch-name>` — создание и переход на новую ветку.
- `git merge <branch-name>` — слияние ветки с текущей.
- `git branch -d <branch-name>` — удаление ветки.

## Основная информация о хеше
- Хеш: Уникальный идентификатор коммита, создаваемый на основе содержимого файлов и метаданных. Обычно используется SHA-1 или SHA-256. Позволяет отслеживать изменения и идентифицировать коммиты.

## Основная информация о логе
- Git log: Команда, отображающая историю коммитов в репозитории. Можно использовать git log --oneline для компактного вывода.

## Основная информация о HEAD
- HEAD: Указатель на текущую ветку или коммит. Обычно указывает на последний коммит в текущей ветке. Используется для навигации и выполнения операций над коммитами.

## Статусы файлов в Git
- Untracked: Файл, который еще не добавлен в индекс.
- Tracked: Файл, который отслеживается Git.
- Staged: Файл, который был добавлен в индекс и готов к фиксации.
- Modified: Файл, который был изменен после последнего коммита.

```mermaid
    A[Untracked] -->|git add| B[Staged]
    B -->|git commit| C[Tracked]
    C -->|modify| D[Modified]
    D -->|git add| B
    D -->|git commit| C
```

