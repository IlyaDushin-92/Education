## Прокачка Linux Mint

### Установить переключение клавиатуры на другой язык:

![GitHub Logo](images/mint_key1.png)

![GitHub Logo](images/mint_key2.png)

![GitHub Logo](images/mint_key3.png)

### Отключить засыпание компьютера:

![GitHub Logo](images/mint_savepower1.png)

![GitHub Logo](images/mint_savepower2.png)

### Отключить скринсервер

![GitHub Logo](images/mint_screen1.png)

![GitHub Logo](images/mint_screen1.png)


### Добавляем источники обновлений:

![GitHub Logo](images/image5.png)![GitHub Logo](images/mint_soft_origin1.png)

![GitHub Logo](images/image5.png)![GitHub Logo](images/mint_soft_origin2.png)

### Запускаем Терминал при помощи клавиатурной комбинации Ctrl-Alt-T и вставляем в него при помощи клавиатурной комбинации Ctrl-Shift-V строку. 

*После вставки текста вводим Y и нажимаем Enter:*

sudo apt list --upgradable -a && sudo apt update && sudo apt full-upgrade -y && reboot

*Эта команда обновит и перезагрузит ОС.*

### Включаем поддержку Snap:

sudo rm /etc/apt/preferences.d/nosnap.pref && sudo apt update && sudo apt install -y snapd

### Устанавливаем необходимые мультимедийные кодеки и шрифты (во время выполнения этой установки браузер лучше закрыть!):

sudo apt update && sudo apt install -y ubuntu-restricted-extras ttf-dejavu-core fonts-crosextra-carlito fonts-crosextra-caladea

### Появится такое окно:![GitHub Logo](images/image3.png)

*В процессе установки программа задаёт пользователю вопросы, на которые нужно отвечать утвердительно (Y/Да), используя TAB и стрелки для перемещения и Enter.*

![GitHub Logo](images/image5.png)![GitHub Logo](images/image7.png)

### Далее по списку:

### Приложения для камеры и звукозаписи:

sudo apt update && sudo apt install -y guvcview gnome-sound-recorder gnome-clocks

### Gifex - GIF запись с экрана в Linuxsudo snap install gifex

### Программа для загрузки видео с таких сайтов (YouTube etc.):

sudo snap install video-downloader

### TeamViewer для Linux для удалённого доступа и поддержки через Интернет:

http://www.teamviewer.com/ru/download/linux.aspx

### Chrome - бесплатный браузер от Google:

https://www.google.ru/chrome/

### Gimp - полноценный редактор графики:

sudo apt update && sudo apt install -y gimp gimp-gmic gimp-gap gimp-data-extras gimp-dcraw abr2gbr

### Pinta - простая рисовалка в духе Paint.net:

sudo snap install pinta

### Karbon - простой редактор векторной графики:

sudo apt update && sudo apt install -y karbon

### Клавиатурный тернажер:

sudo apt update && sudo apt install -y gtypist

*Запуск с русской раскладкой: *

gtypist ru.typ

### Программа видеоконференций ZOOM:

sudo snap install zoom-client

### Telegram - отличный мессенжер!

sudo snap install telegram-desktop

### Читалка формата DJVI:

sudo apt update && sudo apt install -y djview4

### Набор архиваторов:

sudo apt update && sudo apt install -y rar unrar p7zip-full arj

### Простые игры:

sudo apt install -y gnome-chess quadrapasselknetwalk

### FreeCAD - 2D/3D решение для любителей и инженеров с начальной поддержкой формата dwg (Autocad):

sudo snap install freecad

### Cura - слайсер для 3D принтера:

sudo snap install cura-slicer

### Leocad - проектрирование Lego:

sudo snap install leocad --classic

### Kalzium - таблица Менделеева:

sudo snap install kalzium --classic

### Gcompris - набор развивающих игр:

sudo snap install gcompris --classic

### Arduino для Ubuntu 14/16/18 (32/64 bit):

cd ~ ; mkdir Programs ; cd Programs && wget https://downloads.arduino.cc/arduino-1.8.16-linux64.tar.xz && tar -xvf arduino-1.8.16-linux64.tar.xz && cd arduino-1.8.16 && sudo ./install.sh

*Чтобы программный код загружался в контроллер, нужно добавить текущего пользователя в группы dialout и tty:*

sudo gpasswd -a ${USER} tty && sudo gpasswd -a ${USER} dialout && sudo gpasswd -a ${USER} plugdev

*Установить необходимые компоненты для работы с контроллером:*

sudo apt install -y gcc-avr binutils-avr gdb-avr avr-libc avrdude

### Поддержка Java (необходима для некоторых программ. Во время установки браузер лучше закрыть!):

sudo apt update && sudo apt install -y default-jre default-jdk

### Скриншотер (их много, но этот один из лучших):

sudo apt update && sudo apt install -y flameshot

### Инструменты разработчика C++:

sudo apt update && sudo apt install -y build-essential git ghex gdb lldb

### Для создания схем и разводки печатных плат KiCAD EDA:

sudo add-apt-repository --yes ppa:kicad/kicad-5.1-releases -y && sudo apt update && sudo apt install -y --install-recommends kicad kicad-demos kicad-locale-ru

Подробнее о дополнениях к KiCADhttps://progmatikus.livejournal.com/323678.html

### FlatCam - позволяет перенести ваши проекты на фрезерный станок с ЧПУ:

sudo apt install -y python3-pip python3-tk && pip install flatcam

*запускать так:*

/home/user/.local/bin/flatcam

*или так:*

flatcam

### Scratch Desktop 3.6 for Ubuntu Linux:

sudo snap install scratux

### Fritzing - программный комплекс начального уровня для проектирования электронных устройств. Полезен в учебных целях:

sudo apt update && sudo apt install -y fritzing fritzing-data fritzing-parts

### Geany - это мощный, стабильный и легкий текстовый редактор для программистов:

sudo apt update && sudo apt install -y geany geany-plugins

### Dia - приложение для рисования структурированных диаграмм:

sudo apt update && sudo apt install -y dia

### Tilix - тайловый (многооконный) терминал:

sudo add-apt-repository ppa:webupd8team/terminix -y && sudo apt update && sudo apt install -y tilix

### Micro - свободный текстовый редактор для консоли:

cd ~ ; cd Загрузки && wget https://github.com/zyedidia/micro/releases/download/v2.0.10/micro-2.0.10-amd64.deb && sudo apt update && sudo dpkg -i micro-2.0.10-amd64.deb && sudo apt update

### Набор необходимых и полезных утилит:

sudo apt update && sudo apt install -y mc gdebi htop tree mesa-utils sl lm-sensors neofetch winbind wget curl ppa-purge inxi recoll net-tools xclip xsel arp-scan aria2

### SimulIDE - простой и бесплатный симулятор электрических цепей:

git clone https://github.com/rurewa/SimuliDE.git && cp ${HOME}/SimuliDE/SimulIDE.desktop ${HOME}/Рабочий\ стол/

### OpenShot - простой в управлении и мощный по возможностям видеоредактор:

sudo add-apt-repository ppa:openshot.developers/ppa -y && sudo apt update && sudo apt install -y openshot-qt

### Audacity - простой в управлении и мощный по возможностям аудиоредактор:

sudo add-apt-repository ppa:ubuntuhandbook1/audacity -y && sudo apt update && sudo apt install -y audacity

### OBS Studio - бесплатное программное обеспечение с открытым исходным кодом для записи видео и потокового вещания:

sudo add-apt-repository ppa:obsproject/obs-studio -y && sudo apt update && sudo apt install -y ffmpeg obs-studio

### Поддержка snap и flatpack в Центре Приложений:

sudo apt update && sudo apt remove -y mintinstall && sudo apt update && sudo apt install -y flatpak gnome-software gnome-software-plugin-snap gnome-software-plugin-flatpak

### Подключение репозиториев для работы с flatpack:

flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

и

flatpak install -y https://flathub.org/repo/appstream/fr.free.Homebank.flatpakref

### Установка новой версии LibreOffice:

sudo add-apt-repository ppa:libreoffice/ppa -y && sudo apt update && sudo apt dist-upgrade -y

### Установка дополнительных тем для LibreOffice:

sudo apt update && sudo apt install -y libreoffice-style-breeze libreoffice-style-tango libreoffice-style-sifr

### Информация об оборудовании с помощью Inxi:

*запуск этой программы в Терминале:*inxi -Fs

### Перезагрузите компьютер.

## Всё готово!
