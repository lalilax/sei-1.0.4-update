# SEI 1.0.4 Güncelleme Scripti | Upgrade Script SEI 1.0.4beta

![three](https://cdn.discordapp.com/attachments/987875932129886231/989551097158975578/ssss.png)

## Sunucu Kurulumu | Server Installation

### [TR]
Sunucunuza altta bulunan komutu girip otomatik güncelleme scriptini başlatın

### [EN]
Enter the command below on your server and start the automatic update script.

wget -q -O lalilax104.sh https://raw.githubusercontent.com/lalilax/sei-1.0.4-update/main/lalilax104.sh && chmod +x lalilax104.sh && sudo /bin/bash lalilax104.sh

## Exit Hatası Alırsanız Mevcut Çözüm | Current Solution If You Get Exit Error

![three](https://cdn.discordapp.com/attachments/978297777329164359/989615932575985714/seinode.png)

wget -q -O seifix.sh https://raw.githubusercontent.com/lalilax/sei-1.0.4-update/main/seifix.sh && chmod +x seifix.sh && sudo /bin/bash seifix.sh

## Eğer Unjail Olursanız | If You Unjail

![three](https://cdn.discordapp.com/attachments/987875932129886231/989551527628787732/unknown.png)

### [TR]
Validatör sayfanıza girdiğinizde sağ üst köşede bu şekilde bir görüntü varsa alttaki komutu yazmanız gerekiyor.  
- --from=walletname  
Kısmında cüzdan adınızı walletname yazısını silip yazmanız gerekiyor.

### [EN]
When you enter the validator page, if there is an image like this in the upper right corner, you need to type the command below.  
- --from=walletname  
In the section, you need write your wallet name

```
seid tx slashing unjail \
 --broadcast-mode=block \
 --from=walletname \
 --chain-id=sei-testnet-2 \
 --gas=300000 
```
