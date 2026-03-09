# hyprlock
Стильный пиксельный хайперлок, выглядит одинакого на всех мониторах с любым разрешением и размером

<img width="680" height="510" alt="image" src="https://github.com/user-attachments/assets/43159d9d-80bf-4a5b-bfbc-b9a45420dc35" />

### 1. Установка hyprlock:
``` sudo pacman -S hyprlock ```

в *~/.config/hypr/hyprland.conf* активировать hyprlock, например для ноутбука я сделал так:
```
bindl=, switch:on:Lid Switch, exec, hyprlock & sleep 1  && systemctl hibernate

#sleep 1 предотвращает ситуацию когда при активации hyprlock'a на сенунду видно рабочил стол вместо экрана блокировки'
```
### 2. Установка шрифта:
Используется бесплатный шрифт PixelLocale 

Скачать его можно по ссылке:

https://fontstruct.com/fontstructions/show/1765530/pixellocale-v-1-4

Скачайте opentype, распакуйте и переместите в папку */usr/local/share/fonts/*

Обновите кэш командой ```fc-cache -fv```

### 3. Файлы hyprlock.conf перенести в папку *~/.config/hypr/*

Готово, желаю приятного использования!
