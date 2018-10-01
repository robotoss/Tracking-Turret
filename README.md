# Автоматическая турель
Видео сборки и работы турели-  https://www.youtube.com/watch?v=HoRPWUl_sF8

## Инструкция

Убедитесь что pip установлен  
```bash
sudo apt-get install python pip
```

Установите I2C на Ваш Raspberry Pi

https://robotos.in/uroki/nastrojka-i2c

Установите  библиотекуAdafruit stepper motor HAT.

```bash
sudo pip install git+https://github.com/adafruit/Adafruit-Motor-HAT-Python-Library
```

Установите OpenCV 3. Слулуя этой инструкции:

https://robotos.in/uroki/avtomaticheskoe-otslezhivanie-ob-ekta-na-python


Убедитесть что вы создали вирутульную среду с дополнительным флагом. 

```bash
mkvirtualenv cv --system-site-packages -p python2
```

Источник Вашего профиля

```bash
source ~/.profile
```

Активируйте Вашу виртуальную среду

```
workon cv
```

Скопируйте этот репозиторий. 

```
git clone git@github.com:HackerHouseYT/Tracking-Turret.git
```

Перейдите в директорию

```
cd Tracking-Turret
```

Install dependencies to your virtual environment

```
pip install imutils RPi.GPIO
```

Запустите проект!

```
python turret.py
```

## Setting Parameters

turret.py имеет пару параметрова котрые вы можете указать.

```python
### User Parameters ###

MOTOR_X_REVERSED = False
MOTOR_Y_REVERSED = False

MAX_STEPS_X = 30
MAX_STEPS_Y = 15

RELAY_PIN = 22

#######################
```

Они будут расположены в верхней части файла. Используйте `vim turret.py` что бы открыть файл. Нажмите `i` для редактирования.
После внесеныйх изменений, нажмите `esc` затем  `ZZ` что бы сохранить.
