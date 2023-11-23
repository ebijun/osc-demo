osc-demo
========

Demonstaration setting for NetBSD Booth

観光ガイドのガイド
~~~~~~~~~~~~~~~~~~

総集編：
  AsiaBSDCon2018 http://www.re.soum.co.jp/~jun/asiabsdcon2018.pdf
  JNUG2017       http://www.re.soum.co.jp/~jun/JNUG2017.pdf

  参加マップ　
    http://www.re.soum.co.jp/~jun/2016maps.pdf
    http://www.re.soum.co.jp/~jun/2015maps.pdf
    http://www.re.soum.co.jp/~jun/2014maps.pdf

作り方：
 https://github.com/ebijun/NetBSD/blob/master/Guide/Paper/sphinx.rst

 毎回セブンイレブンで両面カラーコピー1部＋両面白黒コピー15部印刷してます。
 表紙はイラストレータ、裏表紙はscribus、本文はSphinxを使っています。
 それぞれについて、pdf出力したものをpdfshufflerで組み合わせています。
 
印刷する手順
1. evince で印刷→ポストスクリプトで出力するとポストスクリプトファイルができる。
  → 1ページずつまとまったポストスクリプトファイルができる。
2. 配布する形式にポストスクリプトを変換する：
　psbook output.ps |psnup -2
　→ 2ページ/1枚にまとまったポストスクリプトファイルができる。
3. 両面印刷： ポストスクリプトファイルの先頭にコマンドを書く。
   << /Duplex true /Tumble true >> setpagedevice
 → 4ページ/1枚にまとまったポストスクリプトファイルができる。ポストスクリプトプリンタに送るとカラー冊子が印刷できる。
4. PDFファイルを白黒に変換する
 gs -sDEVICE=pdfwrite -dProcessColorModel=/DeviceGray -dColorConversionStrategy=/Gray -dPDFUseOldCMS=false -o out.pdf -f in.pdf
 白黒に変換したPDFファイルをもとに白黒冊子が印刷できる。

 194. OSC2023新潟 http://www.re.soum.co.jp/~jun/OSC2023niigata.pdf 
 193. OSC2023広島  http://www.re.soum.co.jp/~jun/OSC2023hiroshima.pdf
 192. KOF2023    http://www.re.soum.co.jp/~jun/KOF2023.pdf
 191. OSC2023島根 http://www.re.soum.co.jp/~jun/OSC2023shimane.pdf
 190. OSC2023東京秋 http://www.re.soum.co.jp/~jun/OSC2023tokyofall.pdf
 189.  ODC2023 http://www.re.soum.co.jp/~jun/ODC2023.pdf
 188. OSC2023京都 http://www.re.soum.co.jp/~jun/OSC2023kyoto.pdf
 187. OSC2023北海道 http://www.re.soum.co.jp/~jun/OSC2023hokkaido.pdf
 186. OSC2022名古屋 http://www.re.soum.co.jp/~jun/OSC2023nagoya.pdf
 185. OSC2023東京春 http://www.re.soum.co.jp/~jun/OSC2023tokyospring.pdf
 184. OSC2023大阪 http://www.re.soum.co.jp/~jun/OSC2023osaka.pdf 
 183. OSC2022福岡 http://www.re.soum.co.jp/~jun/OSC2022fukuoka.pdf
 182. KOF2022    http://www.re.soum.co.jp/~jun/KOF2022.pdf
 181. OSC2022東京秋 http://www.re.soum.co.jp/~jun/OSC2022tokyofall.pdf
 180. OSC2022広島  http://www.re.soum.co.jp/~jun/OSC2022hiroshima.pdf
 179.  ODC2022 http://www.re.soum.co.jp/~jun/ODC2022.pdf
 178. OSC2022京都 http://www.re.soum.co.jp/~jun/OSC2022kyoto.pdf
 177. OSC2022北海道 http://www.re.soum.co.jp/~jun/OSC2022hokkaido.pdf
 176. OSC2022名古屋 http://www.re.soum.co.jp/~jun/OSC2022nagoya.pdf
 175. OSC2022東京春 http://www.re.soum.co.jp/~jun/OSC2022tokyospring.pdf
 174. OSC2022大阪 http://www.re.soum.co.jp/~jun/OSC2022osaka.pdf
 173.  OSC2021福岡 http://www.re.soum.co.jp/~jun/OSC2021fukuoka.pdf
 172. KOF2021    http://www.re.soum.co.jp/~jun/KOF2021.pdf
 171. OSC2021東京秋 http://www.re.soum.co.jp/~jun/OSC2021tokyofall.pdf
 170. OSC2021新潟 http://www.re.soum.co.jp/~jun/OSC2021niigata.pdf 
 169. OSC2021広島  http://www.re.soum.co.jp/~jun/OSC2021hiroshima.pdf
 168. ODC2021 http://www.re.soum.co.jp/~jun/ODC2021.pdf
 167. OSC2021京都 http://www.re.soum.co.jp/~jun/OSC2021kyoto.pdf
 166. OSC2021北海道 http://www.re.soum.co.jp/~jun/OSC2021hokkaido.pdf
 165. OSC2021名古屋 http://www.re.soum.co.jp/~jun/OSC2021nagoya.pdf
 164. OSC2021東京春 http://www.re.soum.co.jp/~jun/OSC2021tokyospring.pdf
 163.  OSC2021大阪 http://www.re.soum.co.jp/~jun/OSC2021osaka.pdf
 162.  ODC2020 http://www.re.soum.co.jp/~jun/ODC2020.pdf
 161.  OSC2020福岡 http://www.re.soum.co.jp/~jun/OSC2020fukuoka.pdf
 160.  KOF2020    http://www.re.soum.co.jp/~jun/KOF2020.pdf
 159.  OSC2020東京秋 http://www.re.soum.co.jp/~jun/OSC2020tokyofall.pdf
 158. OSC2020広島 http://www.re.soum.co.jp/~jun/OSC2020hiroshima.pdf
 157. OSC2020京都 http://www.re.soum.co.jp/~jun/OSC2020kyoto.pdf
 156. OSC2020新潟 http://www.re.soum.co.jp/~jun/OSC2020niigata.pdf
 155. OSC2020北海道 http://www.re.soum.co.jp/~jun/OSC2020hokkaido.pdf
 154.  OSC2020名古屋 http://www.re.soum.co.jp/~jun/OSC2020nagoya.pdf
 153. OSC2020大阪 http://www.re.soum.co.jp/~jun/OSC2020osaka.pdf
 152. OSC2019東京秋 http://www.re.soum.co.jp/~jun/OSC2019tokyofall.pdf
 151.  OSC2019福岡 http://www.re.soum.co.jp/~jun/OSC2019fukuoka.pdf
 150.  KOF2019    http://www.re.soum.co.jp/~jun/KOF2019.pdf
 149.  OSC2019徳島 http://www.re.soum.co.jp/~jun/OSC2019tokushima.pdf
 148.  OSC2019新潟 http://www.re.soum.co.jp/~jun/OSC2019niigata.pdf
 147.  OSC2019島根 http://www.re.soum.co.jp/~jun/OSC2019shimane.pdf
 146.  OSC2019広島 http://www.re.soum.co.jp/~jun/OSC2019hiroshima.pdf
 145.  OSC2019京都 http://www.re.soum.co.jp/~jun/OSC2019kyoto.pdf
 144.  OSC2019名古屋 http://www.re.soum.co.jp/~jun/OSC2019nagoya.pdf
 143.  JNUG2019 http://www.re.soum.co.jp/~jun/JNUG2019.pdf
 142.  OSC2019北海道 http://www.re.soum.co.jp/~jun/OSC2019hokkaido.pdf
 141.  OSC2019沖縄 http://www.re.soum.co.jp/~jun/OSC2019okinawa.pdf
 140.  AsiaBSDCon2019 http://www.re.soum.co.jp/~jun/AsiaBSDCon2019.pdf
 139.  OSC2019東京春 http://www.re.soum.co.jp/~jun/OSC2019tokyospring.pdf
 138.  OSC2019浜名湖 http://www.re.soum.co.jp/~jun/OSC2019hamanako.pdf
 137.	OSC2019大阪 http://www.re.soum.co.jp/~jun/OSC2019osaka.pdf
 136.  OSC2018福岡 http://www.re.soum.co.jp/~jun/OSC2018fukuoka.pdf
 135.  OSC2018島根 http://www.re.soum.co.jp/~jun/OSC2018shimane.pdf
 134.  OSC2018新潟 http://www.re.soum.co.jp/~jun/OSC2018niigata.pdf
 133.  KOF2018    http://www.re.soum.co.jp/~jun/KOF2018.pdf
 132.	OSC2018東京秋 http://www.re.soum.co.jp/~jun/OSC2018tokyofall.pdf
 131.  OSC2018香川 http://www.re.soum.co.jp/~jun/OSC2018kagawa.pdf
 130.  OSC2018広島 http://www.re.soum.co.jp/~jun/OSC2018hiroshima.pdf
 129.  ODC2018 http://www.re.soum.co.jp/~jun/ODC2018.pdf
 128.	OSC2018京都 http://www.re.soum.co.jp/~jun/OSC2018kyoto.pdf
 127.  JNUG2018 http://www.re.soum.co.jp/~jun/JNUG2018.pdf
 126.  OSC2018北海道 http://www.re.soum.co.jp/~jun/OSC2018hokkaido.pdf
 125.  OSC2018沖縄  http://www.re.soum.co.jp/~jun/OSC2018okinawa.pdf
 124.  OSC2018名古屋 http://www.re.soum.co.jp/~jun/OSC2018nagoya.pdf
 123.  AsiaBSDCon2018 http://www.re.soum.co.jp/~jun/AsiaBSDCon2018.pdf
 122.  Raspberry Jam Big Birthday Weekend 2018 in TOKYO http://www.re.soum.co.jp/~jun/RaspberryJam2018.pdf
 121.  OSC2018東京春 http://www.re.soum.co.jp/~jun/OSC2018tokyospring.pdf
 120.  OSC2018浜名湖 http://www.re.soum.co.jp/~jun/OSC2018hamanako.pdf
 119.  OSC2018大阪 http://www.re.soum.co.jp/~jun/OSC2018osaka.pdf
 118.  OSC2017広島 http://www.re.soum.co.jp/~jun/OSC2017hiroshima.pdf
 117.  KOF2017    http://www.re.soum.co.jp/~jun/KOF2017.pdf
 116.  OSC2017長岡 http://www.re.soum.co.jp/~jun/OSC2017nagaoka.pdf
 115.  OSC2017島根 http://www.re.soum.co.jp/~jun/OSC2017shimane.pdf
 114.  OSC2017福岡 http://www.re.soum.co.jp/~jun/OSC2017fukuoka.pdf
 113.  OSC2017東京秋 http://www.re.soum.co.jp/~jun/OSC2017tokyofall.pdf
 112.  OSC2017千葉 http://www.re.soum.co.jp/~jun/OSC2017chiba.pdf
 111.  OSC2017京都   http://www.re.soum.co.jp/~jun/OSC2017kyoto.pdf
 110.  SecCamp2017  http://www.re.soum.co.jp/~jun/SecCamp2017.pdf
 109.  OSC2017北海道 http://www.re.soum.co.jp/~jun/OSC2017hokkaido.pdf
 108.  JNUG2017    http://www.re.soum.co.jp/~jun/JNUG2017.pdf
 107.  OSC2017沖縄  http://www.re.soum.co.jp/~jun/OSC2017okinawa.pdf
 106.  OSC2017名古屋 http://www.re.soum.co.jp/~jun/OSC2017nagoya.pdf
 105.  AsiaBSDCon2017 http://www.re.soum.co.jp/~jun/asiabsdcon2017.pdf
 104.  OSC2017東京春 http://www.re.soum.co.jp/~jun/OSC2017tokyospring.pdf
 103.  OSC2017浜名湖 http://www.re.soum.co.jp/~jun/OSC2017hamanako.pdf
 102.  OSC2017大阪   http://www.re.soum.co.jp/~jun/OSC2017osaka.pdf
 101.  BIGrpiJapan   http://www.re.soum.co.jp/~jun/BIGRPI2016.pdf
 100.  OSC2016広島   http://www.re.soum.co.jp/~jun/OSC2016hiroshima.pdf
 99.   OSC2016福岡    http://www.re.soum.co.jp/~jun/OSC2016fukuoka.pdf
 98.   KOF2016        http://www.re.soum.co.jp/~jun/KOF2016.pdf
 97.   OSC2016東京秋  http://www.re.soum.co.jp/~jun/OSC2016tokyofall.pdf
 96.   OSC2016長岡   http://www.re.soum.co.jp/~jun/OSC2016nagaoka.pdf
 95.	OSC2016島根   http://www.re.soum.co.jp/~jun/OSC2016shimane.pdf
 94.   OSuC2016金沢　http://www.re.soum.co.jp/~jun/OSuC2016kanazawa.pdf
 93.   SecCamp2016  http://www.re.soum.co.jp/~jun/SecCamp2016.pdf
 92.   OSC2016京都   http://www.re.soum.co.jp/~jun/OSC2016kyoto.pdf
 91.   JNUG2016     http://www.re.soum.co.jp/~jun/JNUG2016.pdf
 90.   OSC2016沖縄   http://www.re.soum.co.jp/~jun/OSC2016okinawa.pdf
 89.   OSC2016北海道 http://www.re.soum.co.jp/~jun/OSC2016hokkaido.pdf
 88.	OSC2016名古屋	http://www.re.soum.co.jp/~jun/OSC2016nagoya.pdf
 87.	OSC2016群馬	http://www.re.soum.co.jp/~jun/OSC2016gunma.pdf
 86.   AsiaBSDCon2016 http://www.re.soum.co.jp/~jun/asiabsdcon2016.pdf
 85.	OSC2016東京春	http://www.re.soum.co.jp/~jun/OSC2016tokyospring.pdf
 84.   OSC2016浜名湖  http://www.re.soum.co.jp/~jun/OSC2016hamanako.pdf
 83.   WIDE2016       http://www.re.soum.co.jp/~jun/WIDE201512.pdf
 82.   OSC2015徳島　  http://www.re.soum.co.jp/~jun/OSC2015tokushima.pdf
 81.   KOF2015        http://www.re.soum.co.jp/~jun/KOF2015.pdf
 80.   OSC2015東京秋  http://www.re.soum.co.jp/~jun/OSC2015tokyofall.pdf
 79.   OSC2015福岡    http://www.re.soum.co.jp/~jun/OSC2015fukuoka.pdf
 78.   OSC2015広島    http://www.re.soum.co.jp/~jun/OSC2015hiroshima.pdf
 77.   OSC2015新潟    http://www.re.soum.co.jp/~jun/OSC2015niigata.pdf
 76.   OSC2015島根    http://www.re.soum.co.jp/~jun/OSC2015shimane.pdf
 75.   OSC2015京都    http://www.re.soum.co.jp/~jun/OSC2015kyoto.pdf
 74.   JNUG2015       http://www.re.soum.co.jp/~jun/JNUG2015.pdf
 73.   OSC2015沖縄    http://www.re.soum.co.jp/~jun/OSC2015okinawa.pdf
 72.   OSC2015北海道  http://www.re.soum.co.jp/~jun/OSC2015hokkaido.pdf
 71.   OSC2015名古屋  http://www.re.soum.co.jp/~jun/OSC2015nagoya.pdf
 70.   AsiaBSDCon2015 http://www.re.soum.co.jp/~jun/asiabsdcon2015.pdf
 69.   OSC2015東京春  http://www.re.soum.co.jp/~jun/OSC2015tokyospring.pdf
 68.   OSC2015浜名湖  http://www.re.soum.co.jp/~jun/OSC2015hamanako.pdf
 67.   OSC2015大分    http://www.re.soum.co.jp/~jun/OSC2015oita.pdf
 66.   OSC2014福岡    http://www.re.soum.co.jp/~jun/OSC2014fukuoka.pdf
 65.   KOF2014        http://www.re.soum.co.jp/~jun/KOF2014.pdf
 64.   OSC2014東京秋  http://www.re.soum.co.jp/~jun/OSC2014tokyofall.pdf
 63.   OSC2014広島    http://www.re.soum.co.jp/~jun/OSC2014hiroshima.pdf
 62.   OSC2014島根    http://www.re.soum.co.jp/~jun/OSC2014shimane.pdf
 61.   OSC2014京都    http://www.re.soum.co.jp/~jun/OSC2014kyoto.pdf
 60.   JNUG2014       http://www.re.soum.co.jp/~jun/JNUG2014.pdf
 59.   OSC2014名古屋  http://www.re.soum.co.jp/~jun/OSC2014nagoya.pdf
 58.   OSC2014北海道  http://www.re.soum.co.jp/~jun/OSC2014hokkaido.pdf
 57.   OSC2014沖縄    http://www.re.soum.co.jp/~jun/OSC2014okinawa.pdf
 56.5  OSuC2014川越   http://www.re.soum.co.jp/~jun/OSuC2014kawagoe.pdf
 56.   OSuC2014香川   http://www.re.soum.co.jp/~jun/OSuC2014kagawa.pdf
 55.   OSC2014浜名湖  http://www.re.soum.co.jp/~jun/OSC2014hamanako.pdf
 54.   AsiaBSDCon2014 http://www.re.soum.co.jp/~jun/asiabsdcon2014.pdf
 53.   OSC2014東京春  http://www.re.soum.co.jp/~jun/OSC2014tokyospring.pdf
 52.   OSC2013大分    http://www.re.soum.co.jp/~jun/OSC2013oita.pdf
 51.   OSC2013福岡    http://www.re.soum.co.jp/~jun/OSC2013fukuoka.pdf
 50.   KOF2013        http://www.re.soum.co.jp/~jun/KOF2013.pdf
 49.   OSC2013東京秋  http://www.re.soum.co.jp/~jun/OSC2013tokyofall.pdf
 48.   OSC2013広島    http://www.re.soum.co.jp/~jun/OSC2013hiroshima.pdf
 47.   OSC2013北海道  http://www.re.soum.co.jp/~jun/OSC2013hokkaido.pdf
 46.   OSC2013島根    http://www.re.soum.co.jp/~jun/OSC2013shimane.pdf
 45.5  OSUS2013川越   http://www.re.soum.co.jp/~jun/OSUC2013kawagoe.pdf
 45.   OSC2013京都    http://www.re.soum.co.jp/~jun/OSC2013kyoto.pdf
 44.   JNUG2013       http://www.re.soum.co.jp/~jun/JNUG2013.pdf
 43.   OSC2013沖縄    http://www.re.soum.co.jp/~jun/OSC2013okinawa.pdf
 42.   OSC2013名古屋　http://www.re.soum.co.jp/~jun/OSC2013nagoya.pdf
 41.   AsiaBSDCon2013 http://www.re.soum.co.jp/~jun/asiabsdcon2013.pdf
 40.   OSC2013徳島　  http://www.re.soum.co.jp/~jun/OSC2013tokushima.pdf
 39.   OSC2013東京春  http://www.re.soum.co.jp/~jun/OSC2013tokyospring.pdf
 38.   OSC2013浜松    http://www.re.soum.co.jp/~jun/OSC2013hamamatsu.pdf
 37.   OSC2012福岡    http://www.re.soum.co.jp/~jun/OSC2012fukuoka.pdf
 36.   KOF2012        http://www.re.soum.co.jp/~jun/KOF2012.pdf
 35.   OSC2012会津    http://www.re.soum.co.jp/~jun/OSC2012aizu.pdf
 34.   OSC2012大分秋  http://www.re.soum.co.jp/~jun/OSC2012oitafall.pdf
 33.   OSC2012広島    http://www.re.soum.co.jp/~jun/OSC2012hiroshima.pdf
 32.   OSC2012沖縄    http://www.re.soum.co.jp/~jun/OSC2012okinawa.pdf
 31.   OSC2012東京秋  http://www.re.soum.co.jp/~jun/OSC2012tokyofall.pdf
 30.   OSC2012島根    http://www.re.soum.co.jp/~jun/OSC2012shimane.pdf
 29.   OSC2012京都    http://www.re.soum.co.jp/~jun/OSC2012kyoto.pdf
 28.   OSC2012仙台    http://www.re.soum.co.jp/~jun/OSC2012sendai.pdf
 27.   JNUG2012       http://www.re.soum.co.jp/~jun/JNUG2012.pdf
 26.   OSC2012北海道  http://www.re.soum.co.jp/~jun/OSC2012hokkaido.pdf
 25.   OSC2012名古屋  http://www.re.soum.co.jp/~jun/OSC2012nagoya.pdf
 24.   OSC2012岩手    http://www.re.soum.co.jp/~jun/OSC2012iwate.pdf
 23.   OSC2012愛媛    http://www.re.soum.co.jp/~jun/OSC2012ehime.pdf
 22.   OSC2012東京春  http://www.re.soum.co.jp/~jun/OSC2012tokyospring.pdf
 21.   OSC2012大分    http://www.re.soum.co.jp/~jun/OSC2012oita.pdf
 20.   OSC2011福岡    http://www.re.soum.co.jp/~jun/OSC2011fukuoka.pdf
 19.   OSC2011東京秋  http://www.re.soum.co.jp/~jun/OSC2011tokyofall.pdf
 18.   OSC2011島根    http://www.re.soum.co.jp/~jun/OSC2011shimane.pdf
 17.   KOF2011        http://www.re.soum.co.jp/~jun/KOF2011.pdf
 16.   OSC2011広島    http://www.re.soum.co.jp/~jun/OSC2011hiroshima.pdf
 15.   OSC2011沖縄    http://www.re.soum.co.jp/~jun/OSC2011okinawa.pdf
 14.   OSSC2011会津   http://www.re.soum.co.jp/~jun/OSSC2011aizu.pdf
 13.   OSC2011名古屋  http://www.re.soum.co.jp/~jun/OSC2011nagoya.pdf
 12.   OSC2011京都    http://www.re.soum.co.jp/~jun/OSC2011kyoto.pdf
 11.   JNUG2011       http://www.re.soum.co.jp/~jun/JNUG2011-11.pdf
 10.   OSC2011北海道  http://www.re.soum.co.jp/~jun/OSC2011sapporo.pdf
  9.    OSC2011仙台   http://www.re.soum.co.jp/~jun/OSC2011sendai.pdf
  8.    OSC2011神戸   http://www.re.soum.co.jp/~jun/OSC2011kobe.pdf
  7.    OSC2011大分   http://www.re.soum.co.jp/~jun/OSC2011oita.pdf
  6.    OSC2011東京春 http://www.re.soum.co.jp/~jun/OSC2011tokyospring.pdf
  5.    OSC2011香川   http://www.re.soum.co.jp/~jun/OSC2011kagawa.pdf
  4.    OSC2010福岡   http://www.re.soum.co.jp/~jun/OSC2010fukuoka.pdf
  3.    OSC2010島根   http://www.re.soum.co.jp/~jun/OSC2010shimane.pdf
  2.    KOF2010       http://www.re.soum.co.jp/~jun/KOF2010.pdf
  1.    OSC2010新潟   http://www.re.soum.co.jp/~jun/OSC2010niigata.pdf

