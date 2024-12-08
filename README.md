# m_tinyml

## Confguracion
Estos son los comandos necesarios para configurar Espressif IDF, una biblioteca que nos permite crear proyectos y flashear firmware para el ESP32.
Comandos: 
```
mkdir -p ~/esp
cd ~/esp
git clone --recursive https://github.com/espressif/esp-idf.git
cd ~/esp/esp-idf
./install.sh esp32
cd ~/esp/esp-idf
./install.sh esp32,esp32s2
export IDF_TOOLS_PATH="$HOME/required_idf_tools_path"
./install.sh

. ./export.sh
```

Con estos comandos se puede itilizar el comando `idf.py` para compilar codigo y flashear el ESP32.

## Compilar y flashear
Para compilar y flashear un proyecto se puede utilizar el comando `idf.py` con las siguientes opciones:
```
idf.py build
idf.py -p /dev/ttyUSB0 flash monitor
```
