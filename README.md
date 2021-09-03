#!/bin/bash
#####kurallar#####
printf "
                                                                                  𝙃𝘼𝘾𝙆𝙀𝙍

[1] YOUTUBE
                                                      [2] TİKTOK                                            
[3] TELEGRAM
                                                      [4] İNSTAGRAM                                         
"
#####KULLANICI SECİMİ#####                            read -e -p $'SEÇİM YAZIN : ' secim
#####KODLAMA#####
if [[ $secim == 1 ]];then
        am start -a android.intent.action.VIEW -d https://www.youtube.com
        exit
elif [[ $secim == 2 ]];then
        am start -a android.intent.action.VIEW -d https://www.tiktok.com
        exit
elif [[ $secim == 3 ]];then
        am start -a android.intent.action.VIEW -d https://www.telegram.com
        exit
elif [[ $secim == 4 ]];then
        am start -a android.intent.action.VIEW -d https://www.instagram.com
        ifconfig
else
        printf " HATALI SEÇİM "
fi
