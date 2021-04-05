# ESPEasy_

Plik przygotowano pod platformio i aktualnie espeasy_20210223

1.ESPEasy-mega_20210223\src\Custom-sample.h zmień na Custom.h plik przykładowy dodany.

2.W pliku ESPEasy-mega_20210223\platformio_esp32_envs dodanie
```
; Custom: 4M1M version --------------------------
[env:custom_ESP8266_4M1M_MOJE]
extends                   = esp8266_4M1M
platform                  = ${regular_platform.platform}
platform_packages         = ${regular_platform.platform_packages}
build_flags               = ${regular_platform.build_flags}
                            ${esp8266_4M1M.build_flags}                             
                            -DPLUGIN_BUILD_CUSTOM                            
lib_ignore                = ESP32_ping, ESP32WebServer, ServoESP32, ESP32HTTPUpdateServer, Adafruit GFX Library, LOLIN_EPD, Adafruit ILI9341, Adafruit BusIO, Adafruit Motor Shield V2 Library
extra_scripts             = ${esp8266_custom_common.extra_scripts}
```

3.Rozpakowanie rc-switch-master do ESPEasy-mega_20210223\lib\rc-switch-master
4.Dodanei ESPEasy-mega_20210223\src\_P144_RC-Switch-TX.ino

Powinien utworzyc sie bin na podstawie konfiguracji pobranej z Custom.h (wtyczki)


