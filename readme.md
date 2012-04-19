QtCreator - пропаченная версия QtCreator которая позволяет создавать проекты под андройд, переключаться между сборками андройн\десктоп, ну и еще много плюшек.

Android SDK - куда ж без него то, собственно тут хранятся java классы, тулзы для работы с девайсом, эмулятор, и разные вкусности.
Android NDK - это можно сказать прослойка между Java и C++ кодом.

Пару слов о разработке. Как наверное многим известно разработка под Android ведется на Java, стало быть возникает вопрос, а каким боком тут Qt прикрутили. На самом деле все просто, хоть разработка и ведется на Java ,но никто не мешает подключать библиотеки и использовать их в своем приложении. По сути этим и занимается NDK, из Qt приложения собирается не бинарник (это важно), а библиотека, которая потом подключается из Java кода. 

Приступим к разработке. Для начала инструкция по установке necessitas

Настройка necessitas под ОС Windows
* 1 Распаковать Necessitas.7z в C:\
* 3. В переменную окружения PATH добавить пути:
necessitas/Android/Qt/4762/armeabi/bin/
* 5. Скачать и установить Java jdk http://www.oracle.com/technetwork/java/javase/downloads/jdk-6u26-download-400750.html
* 6. После установки java его нужно пропачить, что под этим подразумевается :
* 6.1. в переменные окружения добавить JAVA_HOME и прописать путь к jdk/bin ( c:\Program Files\Java\jdk1.6.0_25\bin\ ). 
* 6.2. Нужно скопировать C:\Program Files\Java\jdk1.6.0_10\lib\tools.jar в C:\Program Files\Java\jre6\lib\ext
* 7. В настройках QtCreator(Присутствует в Necessitas) Tools→Options→Android→ant location указать путь к apache-ant-1.8.2
* 8. Скачать и установить Ministro http://sourceforge.net/projects/ministro.necessitas.p/files/Ministro-2.0.apk/download
* 9. При первом запуске программы в настройках проекта указать настройку “Install Ministro system wide qt shared libraries installer” и указать путь к Ministro
