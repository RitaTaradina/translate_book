---
description: 5.1 Установка предварительных условий
---

# 5. УСТАНОВКА КОДА ROS НА ПРИМЕРЕ

Перед установкой самого кода ROS By Example это сэкономит некоторое время, если мы установим большинство дополнительных пакетов ROS, которые нам понадобятся позже. \(Также будут предоставлены инструкции по установке отдельных пакетов по мере необходимости в книге.\) Просто скопируйте и вставьте следующую команду \(без знака $\) в окно терминала, чтобы установить необходимые нам пакеты Debian. Символ  в конце каждой строки делает весь блок похожим на одну строку для Linux при выполнении копирования и вставки:

```text
$ sudo apt-get install ros-indigo-turtlebot-bringup \ ros-indigo-turtlebot-create-desktop ros-indigo-openni-* \ ros-indigo-openni2-* ros-indigo-freenect-* ros-indigo-usb-cam \ ros-indigo-laser-* ros-indigo-hokuyo-node \ ros-indigo-audio-common gstreamer0.10-pocketsphinx \ ros-indigo-pocketsphinx ros-indigo-slam-gmapping \ ros-indigo-joystick-drivers python-rosinstall \ ros-indigo-orocos-kdl ros-indigo-python-orocos-kdl \ python-setuptools ros-indigo-dynamixel-motor-* \
libopencv-dev python-opencv ros-indigo-vision-opencv \ ros-indigo-depthimage-to-laserscan ros-indigo-arbotix-* \ ros-indigo-turtlebot-teleop ros-indigo-move-base \ ros-indigo-map-server ros-indigo-fake-localization \ ros-indigo-amcl git subversion mercurial
```

Если вы читаете печатную версию книги, копирование и вставка, вероятно, не вариант. Вместо этого вы можете использовать следующие команды для загрузки небольшого сценария оболочки с именем rbx1-prereq.sh, который запустит команду apt-get, описанную выше:

```text
$ cd ~
$ wget https://raw.githubusercontent.com/pirobot/rbx1/indigo-devel/\
rbx1-prereq.sh
$ sh rbx1-prereq.sh
```

