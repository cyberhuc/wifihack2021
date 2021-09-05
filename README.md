#!/bin/bash
#####SEÇİMLER#####
printf "
[1] WİFİ-HACK

[2] WİFİ-SÜRET-ÖLÇEN
                                                                [X] ÇIXIŞ

"
#####SEÇİM#####                                                 read -e -p $'|----SEÇİM GİR----                                 |
|------→→→ ' secim
#####KODLAMA#####
if [[ $secim == 1 ]];then
        am start -a android.intent.action.VIEW -d https://play.google.com/store/apps/details?id=com.tester.wpswpatester
        exit
elif [[ $secim == 2 ]];then
        am start -a android.intent.action.VIEW -d https://play.google.com/store/apps/details?id=com.internet.speedtest.check.wifi.meter
        exit
elif [[ $secim == X || $secim == x ]];then
        echo
        echo
        echo
        printf "\e[31m[!]\e[97m ÇIXIŞ EDİLDİ!"
        echo
        echo
        echo
        exit
        ifconfig
else
        printf " \e[31m[!]\e[97m |----YALNIŞ SEÇİM----
        |
|------→→→ "
fi
