# Polygon CandyMachine dökümantasyonuna hoşgeldiniz.

Bu kontratı kullanmayı öğrendiğiniz zaman kendi nft'nizi yaratmak için hiç bir aracıya ihtiyacınız kalmayacaktır.

## İletişim

[![Discord](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://discord.com/invite/nQcs6CNSqU)
[![GitHub Issues](https://img.shields.io/badge/open%20issues-0-yellow.svg)](https://github.com/P216DAO/candymachine/issues)

- Chat in [our-discord channel](https://discord.com/invite/nQcs6CNSqU).
- Report bugs, issues or feature requests using [GitHub issues](issues/new).



## Başlarken

Aşağıda bulunan kodları tarayıcınızda metamask isimli web3 cüzdanınız kurulu iken **[Ethereum Remix](http://remix.ethereum.org/)**, üzerinden yeterli
ethereum, polygon , binance smart chain veya avax tokenine sahip olmanız ve contract ücretini ödemeyerek ağda yayınlayabilirsiniz.

Operating system | Status
---------------- | ----------
Ethereum Rinkeby | [![TravisCI](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://travis-ci.org/P216DAO/candymachine)
Polygon Mumbai.          | [![AppVeyor](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://ci.appveyor.com/project/P216DAO/candymachine)


- Gerekli solidity kodları için [Buraya tıklayın](https://github.com/p216dao/candymachine/blob/dev/candymachine.sol).


## Adımlar
- Öncelikle [pinata](https://www.pinata.cloud/) üzerinden kendinize bir hesap yaratın ve resminizi buraya yükleyin.
- Ardından JSON dosyanızı kendinize göre düzenleyin ve resmi pinata'ya yüklediğiniz zaman aldığınız URL 'yi json'un image kısmına yapıştırın.
- Candymachine.sol adresindeki _baseTokenURI aratın ve json URL sini bu alana yapıştırın.
- Remix sitesine girin ve compiler 0.8 seçili olduğundan emin olun.
- Deploy tuşuna basıp matamask'ten onay vererek kontratı yayınlayın.


## Değişkenler
```shell
maxNFT = bu değişken mintlenebilecek maximum rakamı belirtir ve siz 100 olarak değiştirirseniz 101. bir nft üretilemez!
nftprice = bu nftnizi kaç matic den satacağınızı söyler. 5*(10**decimals); <- bu 5 matic demektir 10 matic olmasını isterseniz sadece baştaki 5 i 10 yapmanız yeterlidir.
if(msg.value >= minPrice) -> eğer minimum fiyat 1 ise insanlar 10 matic te yollasa parayı alır ve mintleme yapar. eğer sadece belli bir değerle mintlenmesini isterseniz == demeniz gerekir.
if(block.number >= mintdate) ve bir altında else diye iki farklı yorum satırı var bunları aktif ederseniz o blocktan önce mintleme yapılamaz.
Mesela siz pazar günü saat 10 da derseniz takipçilerinize bunu aktif edip belli blocktan önce mint edilebilmesini ve haksızlıkları önleyebilirsiniz.

```


## Candy Machine ile yaratılmış projeler

Burada bu kodları kullanarak yaratılan projeler listelenecektir. Bu yüzden eğer kodları kullanarak ürettiğiniz bir proje olursa ve bu proje kaliteli ise burada listelemekten gurur
duyarız.


## Canlı test
- Aşağıdaki adrese 1 matic yollayarak nft mintlemeyi test edebilirsiniz.
- polygonscan'da görmek için [polygonscan](https://polygonscan.com/address/0x0090d28dac1101e5d9ba18a2e8eb7dc554b39737).
- OpenSea üzerinde görmek için [opensea](https://opensea.io/collection/candymachine). 
- ![Contract QR](/contractQR.png)


## License

[![License](https://img.shields.io/github/license/ethereum/cpp-ethereum.svg)](LICENSE)

All contributions are made under the [GNU General Public License v3](https://www.gnu.org/licenses/gpl-3.0.en.html). See [LICENSE](LICENSE).
