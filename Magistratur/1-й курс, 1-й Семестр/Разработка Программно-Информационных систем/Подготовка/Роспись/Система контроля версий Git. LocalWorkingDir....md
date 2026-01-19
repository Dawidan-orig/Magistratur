Staging Area. Local Repository. Remote Repository. Команды переходов.

Git использует трёхслойную архитектуру: **LocalWorkingDir** (рабочая директория), **Staging Area** (индекс), **Local Repository** (.git), с возможностью синхронизации с **Remote Repository**.

- **LocalWorkingDir (рабочая директория):** Видимые файлы проекта, где редактируете код. Здесь изменения **неотслеживаемы** до `git add`.
- **Staging Area (индекс):** Промежуточный буфер (.git/index). `git add` перемещает файлы сюда для подготовки коммита. `git status` показывает разницу.
- **Local Repository (.git):** Полная история коммитов, веток, объектов. `git commit` сохраняет снимок индекса сюда.
- **Remote Repository:** Удалённый сервер (GitHub). `git push/pull` синхронизирует локальный с remote.

#### Ветки и переходы
- **git checkout {branch}** — переключается на ветку (или коммит); `git checkout -b new` — создает и переходит.
- **git branch** — список веток; `git branch new` — создать; `git branch -d old` — удалить.
