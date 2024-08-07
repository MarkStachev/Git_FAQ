# Основы работы с Git.  

:bulb: Git – это один из видов системы контроля версий, или VCS (от англ. Version Control System) / SCM (от англ. Source Control Management), — это программное обеспечение, которое помогает отслеживать изменения в программах, текстовых файлах, больших документах, веб-сайтах и так далее.

Зачем нужен Git?
- хранить историю изменений в виде отдельных ревизий;
- манипулировать историей: например, менять порядок ревизий, полностью удалять версии, возвращаться назад в истории;
- анализировать изменения: например, смотреть кто и когда вносил изменения, кто чаще всего вносит изменения в определённый файл и так далее.

## Установка Git
**Для Windows**  
1. Скачать и установить Git с [официального сайта](https://git-scm.com/download/win).
2. Убедиться, что Git установлен введя команду проверки версии Git `git version`, если версия отображается, значит Git установлен.     

**Для macOS**  
Первый способ  
1. Открыть программу "Терминал" и ввести команду `/usr/bin/git`.
2. В открывшемся установщике нажать на кнопку "Установить".
3. Убедиться, что Git установлен введя команду проверки версии Git `git version`, если версия отображается, значит Git установлен.   

Второй способ. Через менеджер пакетов Homebrew.
1. На [официальном сайте](https://brew.sh) Homebrew скопировать команду для установки.
2. Открыть программу "Терминал" и ввести скопированную команду для установки.
3. Установить Git с помощью Homebrew введя команду `brew install git`.
4. Убедиться, что Git установлен введя команду проверки версии Git `git version`, если версия отображается, значит Git установлен. 

**Для Linux**
1. На [официальном сайте](https://git-scm.com/download/linux) Git найти команду установки для своей версии Linux, скопируйте ее.
2. Открыть программу "Терминал" и вставить скопированную команду.
3. Убедиться, что Git установлен введя команду проверки версии Git `git version`, если версия отображается, значит Git установлен. 

___
### Материалы и полезные инструменты
- [Яндекс Практикум. Базовый онлайн-курс "Основы работы с Git"](https://practicum.yandex.ru/git-basics/)
- [Синтаксис Markdown](https://github.com/sandino/Markdown-Cheatsheet/blob/master/README.md)
- [Markdown live editor](https://markdown-here.com/livedemo.html)
- [Статья о диаграммах Mermaid.js в README-файлах GitHub](https://habr.com/ru/articles/652867/)
- [Mermaid live editor](https://mermaid.live/edit#pako:eNpVkEFrg0AQhf_KMKcG9A94KCTa5pLSQnOqehh0dJdkd5Z1JQT1v3eNLbRzmuF97zG8CRtpGTPsrnJrFPkA56KyEGdf5srrIRgaakjT5_nIAYxYvs9weDoKDEqc07bfbfxhhSCfTivGEJS2l2WT8of_3fIMRXkiF8TVf5XzTWZ4KfWHivH_FeU5ul7LjrKO0oY85ORrTNCwN6Tb-Pq0GioMig1XmMW1JX-psLJL5GgM8nm3DWbBj5ygl7FXGMOuQ7xG11LgQlPvyfwi3Oog_m0r5tFPgo7sl4j5MS7f0pBlZg)
- [LearnGitBranching – интерактивный учебник по Git](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://learngitbranching.js.org/&ved=2ahUKEwiIpdT-iOiHAxVCh1YBHY3BES8QFnoECBcQAQ&usg=AOvVaw2Rj9ViDXwUjaqtPhqYhCCH)