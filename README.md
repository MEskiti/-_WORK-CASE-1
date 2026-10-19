Звіт до виконання Work-case 4

Тема: Менеджери пакетів та встановлення програмного забезпечення в ОС Linux

Словник англ. термінів:

Package — an archive file containing software binaries, libraries, and metadata required for installation.

Repository — a centralized server where software packages are hosted and maintained for download.

Package Manager — a tool that automates installing, upgrading, configuring, and removing software.

Dependency — a software module or library required by another package to function properly.

CLI (Command Line Interface) — a text-based interface used to execute system commands directly.

GUI (Graphical User Interface) — a visual interface allowing interaction via windows, icons, and buttons.

Update — refreshing local package lists from repositories.

Upgrade — installing newer versions of already installed software packages.

Purge — removing a package completely along with all its configuration files.

1. Основні поняття та огляд менеджерів пакетів

Пакет (Package): Це стандартизований архівний файл, який містить скомпільовані бінарні файли програми, бібліотеки, конфігураційні файли,
 а також метадані (інформацію про версію, автора, опис та залежності — інші пакети, необхідні для коректної роботи програми).

Репозиторій (Repository): Це централізоване сховище (сервер або хмарне сховище), 
де зберігається та підтримується програмне забезпечення для конкретного дистрибутива Linux. 
Репозиторії дозволяють безпечно завантажувати, інсталювати та автоматично оновлювати програми разом із усіма залежностями.

Огляд менеджерів пакетів у Linux:

APT (Advanced Packaging Tool) / dpkg: Основний інструмент для дистрибутивів на базі Debian (Ubuntu, Debian, Linux Mint, Kali Linux). Працює з пакетами у форматі .deb.

DNF / YUM / rpm: Використовується в дистрибутивах сімейства Red Hat Enterprise Linux (Fedora, RHEL, CentOS, AlmaLinux). Працює з пакетами .rpm.

Pacman: Швидкий і легкий менеджер пакетів для Arch Linux та його похідних (Manjaro, EndeavourOS). Відомий своєю роботою з репозиторієм AUR (Arch User Repository).

Zypper: Офіційний менеджер пакетів для openSUSE та SUSE Linux Enterprise.

Універсальні менеджери (Snap, Flatpak, AppImage): Незалежні від дистрибутивів формати, 
які пакують додаток разом із усіма залежностями всередину контейнера, забезпечуючи роботу на будь-якому дистрибутиві Linux.

2 та 3:

![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_134348.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_134358.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_134422.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_134454.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_134521.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_135105.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_135124.png)
![Image alt](https://github.com/MEskiti/-_WORK-CASE-1/blob/main/2026-10-19_135154.png)

4. Методи встановлення через GUI:

Магазини додатків (App Center / GNOME Software / Ubuntu Software):

Принцип роботи: Надають візуальний каталог програм, розсортованих за категоріями (Ігри, Офіс, Розробка, Мультимедіа). Пошук здійснюється через рядковий фільтр, а інсталяція виконується натисканням однієї кнопки («Install» / «Встановити»).

Приклад: Відкриття центру додатків Ubuntu, пошук за запитом «VLC», перегляд рейтингу та описів, і натискання кнопки встановлення.

Спеціалізовані менеджери пакетів (наприклад, Synaptic):

Принцип роботи: Це потужна графічна оболочка для apt. Вона дозволяє здійснювати точковий пошук пакетів за назвою, станом та категоріями, керувати репозиторіями PPA та виконувати масові операції.

Приклад: Запуск Synaptic, введення пароля адміністратора, знаходження пакету через кнопку «Search» (наприклад, geany або vlc), вибір пункту меню «Mark for Installation» (Позначити для встановлення) та застосування змін кнопкою «Apply».

5. Conclusions:
During Work-case 4, we gained practical experience with software and package management in Linux. We explored the core concepts of packages and repositories, and mastered working with the APT package manager in the command line. Using CLI commands, we successfully updated system package lists, searched for software, installed required applications (VLC media player and C++ build tools), and managed dependencies. Additionally, we reviewed graphical installation methods via App Centers and GUI package managers like Synaptic. 
