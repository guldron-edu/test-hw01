# Шпаргалка

## Взаимодействие с гитом

**_git clone_** - забрать проект гита. Ссылку брать с из созданого репозитория в
github. После ссылки можно добавить имя локального репозитария

**_git init_** - инициализация локального репозитория (используется один раз)

**_git remote add [сокращение][url]_**
(`git remote add origin git@github.com:guldron-edu/test-hw01.git`) -
используется для иницализации созданого локально репозитория с репозиторием на
[github](https://github.com/). Необходимо создать на github репозиторий с
названием аналогичным локальному.

**_git push origin master_** - связывает локальный репозиторий с удаленным. и
отправляет коммиты.

**_git push_** - отправляет комиты на привязаный репозиторий

**_git remote -v_** - посмотреть, какому URL соответствует сокращённое имя в Git

**_git fetch [имя удал. сервера]_** - извлекает все наработки, отправленные
(push) на этот сервер после того, как вы склонировали его (или получили
изменения с помощью fetch). Важно отметить, что команда fetch забирает данные в
ваш локальный репозиторий, но не сливает их с какими-либо вашими наработками и
не модифицирует то, над чем вы работаете в данный момент. Вам необходимо вручную
слить эти данные с вашими, когда вы будете готовы.

**_git pull_** - автоматически извлекает и затем сливает данные из удалённой
ветки в вашу текущую ветку

## Работа с локальным репозиторием

**_git status_** - команда для определения состояния файлов в локальном
репозитории

**_git add ._** - добавить все файлы к отслеживанию(индексировать). Возможно
варианты добавлять пофайлово или папками

**_git diff_** - более информативная команда чем `git status`. Позволяет узнать
что конкретно поменялось, а не только какие файлы были изменены

**_git commit -m ""_** - позволяет зафиксировать внесенные изменения. В ""
добавляется комментарий. Зафиксированы будут только те изменения, которые были
проиндексированы с помощью команды `git add`

**_git rm --cached файл_** - удаление файла из индекса. локально останется, но в
гит заливаться не будет

**_git mv file_from file_to_** - переименования файла
