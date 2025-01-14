<h1>Silence of the Siren — Краткое руководство для переводчиков</h1>

Спасибо, что зашли в проект по переводу Silence of the Siren! Если вы хотите принять участие, ниже вы найдёте краткое руководство, с которого можно начать.

<h2>Редактирование</h2>

Вы можете смело редактировать файлы прямо здесь, на GitHub (откройте нужный файл и нажмите на иконку «карандаш» в правом верхнем углу). 
Когда закончите правки, сделайте commit, а затем на следующем шаге нажмите «propose changes», чтобы создать ветку и «pull request», который мы затем примем. Не стесняйтесь редактировать только часть файла, некоторые из них довольно большие.

Если хотите редактировать файлы на своём компьютере, используйте редактор, который умеет работать с XML — например, бесплатный Notepad++. Существует два способа получить файлы на свой компьютер: можно использовать git-клиент или просто скачать весь репозиторий в виде zip-архива, отредактировать нужные файлы, а затем скопировать их содержимое в онлайн-редактор на GitHub.

<h2>Лучшие практики для перевода</h2>

- Для часто встречающихся терминов посмотрите, как они переведены в других файлах. Возможно, стоит создать небольшой глоссарий, если вы — первый, кто начинает перевод.

- Старайтесь, чтобы длина переведённого текста была примерно такой же, как у оригинала на английском. Во многих случаях текстовые блоки автоматически подстраиваются под длину текста, но лучше не слишком отклоняться от оригинальной длины (да, иногда это бывает сложно).

<h2>Форматирование</h2>
Мы используем несколько разных тегов, например \n для переноса строки, а также теги для выделения текста (жирный/курсив) и некоторые цветовые коды. Всё это достаточно просто, старайтесь сохранить их в переводе.

Строки со сложным форматированием используют специальные теги в начале и в конце. Пожалуйста, следите, чтобы они оставались целыми. Чаще всего ошибки случаются именно при нарушении этих тегов. :)

    <![CDATA[   и    ]]>

Примеры некоторых тегов и раскрашенного текста:

    <![CDATA[Now <b><i>do something</i></b>.\nThis is on the next line.]]>
    <![CDATA[<color=SOTS_COLOR_GOLD>Aura Coins</color> generated per phase at this base.]]>

В некоторых текстах встречаются параметры вида {1} и {2}. Это означает, что в эти места будут вставляться имена или другие части текста — не забудьте их сохранить! При этом часто нужно менять порядок слов, чтобы предложение звучало естественно.

<h2>Steam-ключи</h2>

В качестве небольшой благодарности и чтобы помочь процессу перевода, мы предлагаем до 5 ключей Steam для каждого языка. Это также позволит новым переводчикам тестировать переводы прямо в игре. 
Правило такое: любой, кто отправит переведённый файл (минимум 20 строк), может получить ключ, пока они есть в наличии для данного языка (по предыдущему опыту, вряд ли будет более 5 волонтёров на один язык).

Мы рекомендуем сообщать другим, что вы работаете над переводом. Мы стараемся всё организовать на сервере Discord игры: 
https://discord.gg/DAeGEtqHNS

<h2>Тестирование в игре</h2>

Найдите папку Streaming Assets в папке, где установлена игра, и скопируйте все файлы в отдельную папку внутри Modules. Сами файлы .xml должны находиться в подпапке Database, посмотрите на пример LanguagePackCZ.

Если игра не загружается или некоторые переведённые тексты не отображаются, скорее всего, проблема в структуре xml/тегах форматирования. Чтобы разобраться, посмотрите файл журнала (log) игры.

Также проверьте, чтобы весь текст помещался в отведённые поля. Если нет, возможно, это уже проблема на стороне игры — обязательно сообщите нам!

<h2>Атрибуция</h2>

Не забудьте указать свои имена в соответствующей секции каждого файла. Игра собирает их и показывает во всплывающей подсказке для каждого языка в настройках. 
Вот пример (главное показать, что в одном файле может быть сразу несколько имён):

    <Contributors>
        <Name>Первый переводчик, работавший над этим файлом</Name>
        <Name>Другой переводчик, который внёс, например, правки</Name>
    </Contributors>
