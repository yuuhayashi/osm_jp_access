# osm_jp_access
OpenStreetMap Japan Key:access draft


 * [日本のaccessキー ドラフト版](http://surveyor.mydns.jp/gitbucket/yuu/osm_jp_access/raw/master/OSMaccess.class.violet.html)  

  ![CC0](https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/CC0_button.svg/88px-CC0_button.svg.png)


## 参考

 * [道路標識、区画線及び道路標示に関する命令 （六）車両の種類の略称](http://elaws.e-gov.go.jp/search/elawsSearch/elaws_search/lsg0500/detail?lawId=335M50004002003&openerCode=1)

 * [OpenStreetMap Wiki - JA:Key:access](https://wiki.openstreetmap.org/wiki/JA:Key:access) の[6.1 陸上交通](https://wiki.openstreetmap.org/wiki/JA:Key:access#.E9.99.B8.E4.B8.8A.E4.BA.A4.E9.80.9A)


```
access=*
┃
┣━ foot=*   歩行者
┃
┗━ vehicle=*    車両
　　　┃
　　　┣━ bicycle=*     自転車
　　　┃
　　　┣━ carriage=*    軽車両
　　　┃
　　　┗━ motor_vehicle 動力付き車両
　　　　　　┃
　　　　　　┣━ trollerbus 「トロリー」 トロリーバス
　　　　　　┃
　　　　　　┣━ tram 路面電車
　　　　　　┃
　　　　　　┗━ motor_car 自動車
　　　　　　　　　┃
　　　　　　　　　┣━ hgv_caravan 「けん引」 重被牽引車をけん引しているけん引自動車
　　　　　　　　　┃
　　　　　　　　　┣━ disabled 「標章車」 高齢運転者等、標章自動車
　　　　　　　　　┃
　　　　　　　　　┣━ agricultural 「小特」 小型特殊自動車
　　　　　　　　　┃
　　　　　　　　　┣━ route_bus   「路線バス」　路線定期運行の用に供する自動車
　　　　　　　　　┃
　　　　　　　　　┣━ taxi=*      「タクシー」　一般乗用旅客自動車運送事業の用に供する自動車
　　　　　　　　　┃
　　　　　　　　　┣━ moped=*,mofa=*,motorcycle=*「二輪」 二輪の自動車及び原動機付自転車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ motorcycle　「自二輪」　大型自動二輪車、普通自動二輪車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ moped　「小二輪」　小型二輪車、原動機付自転車
　　　　　　　　　┃　　　　　┃
　　　　　　　　　┃　　　　　┗━ mofa　「原付」　原動機付自転車
　　　　　　　　　┃
　　　　　　　　　┣━ hgv=*,goods=*  「貨物」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ hgv:l     「大貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:m   「中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:ms  「準中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ goods:normal 「普貨」　
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:l,motor_car:xm,motor_car:xl　「大型等」
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ motor_car:l 「大型」 大型自動車
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┣━ hgv:l  「大貨」　
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┗━ psv:l 「大乗」 大型乗用自動車
　　　　　　　　　┃　　┃　　　　　┃
　　　　　　　　　┃　　┃　　　　　┣━ tourist_bus 「観光バス」
　　　　　　　　　┃　　┃　　　　　┃
　　　　　　　　　┃　　┃　　　　　┣━ bus:l 「大型バス」
　　　　　　　　　┃　　┃　　　　　┃
　　　　　　　　　┃　　┃　　　　　┗━ minibus 「マイクロ」
　　　　　　　　　┃　　┃　　　　　　　　┃
　　　　　　　　　┃　　┃　　　　　　　　┗━ psv:xm 「特定中乗」 特定中型乗用自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ motor_car:m 「中型」 中型自動車
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┣━ goods:m  「中貨」　
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┗━ psv:m 「中乗」 中型乗用自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ motor_car:xm 「特定中型」 特定中型自動車
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┣━ hgv:xm  「特定中貨」　
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┗━ psv:xm 「特定中乗」 特定中型乗用自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ hgv 「大貨等」　
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┣━ hgv:l  「大貨」　
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┣━ mortor_car:xl　「大特」 大型特殊自動車
　　　　　　　　　┃　　┃　　┃
　　　　　　　　　┃　　┃　　┗━ hgv:xm 「特定中貨」
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:ms  「準中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ goods:normal 「普貨」　
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:l 「大型」 大型自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ hgv:l  「大貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ psv:l 「大乗」 大型乗用自動車
　　　　　　　　　┃　　　　　┃
　　　　　　　　　┃　　　　　┣━ tourist_bus 「観光バス」
　　　　　　　　　┃　　　　　┃
　　　　　　　　　┃　　　　　┣━ bus:l 「大型バス」
　　　　　　　　　┃　　　　　┃
　　　　　　　　　┃　　　　　┗━ minibus 「マイクロ」
　　　　　　　　　┃　　　　　　　　┃
　　　　　　　　　┃　　　　　　　　┗━ psv:xm 「特定中乗」 特定中型乗用自動車
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:m 「中型」 中型自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:m  「中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ psv:m 「中乗」 中型乗用自動車
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:xm 「特定中型」 特定中型自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ hgv:xm  「特定中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ psv:xm 「特定中乗」 特定中型乗用自動車
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:ms 「準中型」 準中型自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:ms 「準中貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ psv:ms 「準中乗」 準中型乗用自動車
　　　　　　　　　┃
　　　　　　　　　┣━ motor_car:normal 「普通」 普通自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ goods:normal 「普貨」　
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┣━ motor_car:kei 「軽」 軽自動車
　　　　　　　　　┃　　┃
　　　　　　　　　┃　　┗━ psv:ms 「普乗」 普通乗用自動車
　　　　　　　　　┃
　　　　　　　　　┣━ psv 「乗用」 専ら人を運搬する構造の
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
　　　　　　　　　┃
　　　　　　　　　┣━ 
```
