# Простая программа для изучения **Windows API**
## Компиляция
### clang++
1. Необходимо установить **Windows SDK**.
2. В момент компиляции необходимо указать путь к библиотеки **user32.lib**, в этой библиотеке содержится имплиментация функций **Windows API**. *По умолчанию **user32.lib** находится по пути "C:\Program Files (x86)\Windows Kits\10\Lib\10.0.18362.0\um\x64\user32.lib"*

clang++ .\main.cc -l"C:\Program Files (x86)\Windows Kits\10\Lib\10.0.18362.0\um\x64\user32.lib"

### CL.exe
1. Установить **Windows Studio** и **Windows SDK**. Все это можно сделать из под **Windows Studio Installer**
2. Открыть командную строчку разработчика.
3. Указать имя библиотеки **user32.lib** с имплементацией **Windows API**

CL .\mian.cc user32.lib
