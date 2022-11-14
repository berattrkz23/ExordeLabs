# <h1 align="center"> Exorde </h1>


![image](https://user-images.githubusercontent.com/101149671/201298361-b48bc53b-7858-42c2-b6ab-5cf7270e3429.png)

<h1 align="center"> Selamlar, Coinlist tarafından desteklenen ExordeLabs testnet rehberi, aşağıda gerekli linkler ve rehber mevcut:
</h1>

### Linkler:

 * [Exorde Türkiye Kanalı](https://t.me/ExordeTurkish)
 * [Exorde Discord Kanalı](https://discord.gg/44KzbSWB)
 * [Sıralama](https://explorer.exorde.network/leaderboard) ve [Explorer](https://explorer.exorde.network/)

## Gerekli notlar:

 * Bugün node kuranlar Kasım 22'e kadar %5 fazla ödül alacak
 * Testnet Şubat ayına kadar sürecek. (ekibin söylediği)
 * Hala ağ stabil çalışmıyor "Please try restarting your application." gibi hatalar alırsanız endişe etmeyin, tekrar deneyin.
 * Skale Network'ü bilirsiniz, (BlockPI ile Klaynt gibi düşünebilirsiniz..) ona bağlı olduğu için tek tük hatalar olur.

## Sistem gereksinimi:

 * Net bilgi yok, kendim test ettim:

```
CPU : 2 cores
RAM: 4Gb
SSD: 20Gb
```
## Docker ve güncellemeler::

```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
```

## Screen:
```
sudo apt install -y build-essential libssl-dev libffi-dev git curl screen
```

## Git clone çekiyoruz
```
git clone https://github.com/exorde-labs/ExordeModuleCLI.git
```

## Burası uzun bir yükleme sürecek:
```
sudo su
cd ExordeModuleCLI
docker build -t exorde-cli .
```

## Bir screen açıyoruz:
```
screen -S exorde
```

## Metamask yazdığım yere 0xli başlayan metamask adresi giriyoruz:

 * Testnet cüzdanı kullanın

```
docker run -it exorde-cli -m metamask -l 2
```

## Ve gördüğünüz gibi çalışıyor:

 
 * Çalıştığı zaman ctrl a d ile çıkın ve dokunmayın, arada kontrol edersiniz.

## Gerekli komutlar:

 * Screen açma:

```
screen -S screenadı
```

 * Screen içersine girme:

```
screen -r screenadı
```

 * Screenleri görme:

```
screen -ls
```

 * Screen silme:

```
screen -XS screenadı quit
```

 * Tüm screenleri silme:

```
pkill screen
```

## Böylede bir tokenomics var, detaylı incelemedim:

![image](https://user-images.githubusercontent.com/101149671/201303557-755bcdc8-47f6-4a3e-a1a1-941e62342a37.png)





