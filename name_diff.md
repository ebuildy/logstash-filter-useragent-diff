# Basic


```sql
SELECT DISTINCT t1.name || t2.name, t1.name AS name1,t2.name AS name2 
FROM dfs.tmp.`output1.json` t1 
JOIN dfs.tmp.`output2.json` t2 ON t1.id = t2.id 
WHERE t1.name <> t2.name
```

| duplicate_key | name 1 | name 2 |
| ------------- | ------ | ------ |
| OtherUnknown                | Other              | Unknown            |
| IEInternet Explorer         | IE                 | Internet Explorer  |
| EdgeMicrosoft Edge          | Edge               | Microsoft Edge     |
| Mobile SafariSafari         | Mobile Safari      | Safari             |
| Python RequestsUnknown      | Python Requests    | Unknown            |
| IceweaselFirefox            | Iceweasel          | Firefox            |
| ChromiumChrome              | Chromium           | Chrome             |
| Firefox MobileFirefox       | Firefox Mobile     | Firefox            |
| AndroidSafari               | Android            | Safari             |
| MaxthonChrome               | Maxthon            | Chrome             |
| Chrome MobileChrome         | Chrome Mobile      | Chrome             |
| SeaMonkeyFirefox            | SeaMonkey          | Firefox            |
| Firefox iOSFirefox          | Firefox iOS        | Firefox            |
| OtherMozilla                | Other              | Mozilla            |
| Chrome Mobile iOSChrome     | Chrome Mobile iOS  | Chrome             |
| ChromiumSafari              | Chromium           | Safari             |
| IE MobileInternet Explorer  | IE Mobile          | Internet Explorer  |

# Advanced with UA


```sql
SELECT t1.ua,t1.name AS name1,t2.name AS name2 
FROM dfs.tmp.`output1.json` t1 
JOIN dfs.tmp.`output2.json` t2 ON t1.id = t2.id 
WHERE t1.name <> t2.name
```


| name 1 | name 2 | user agent |
| ------ | ------ | ---------- |
| Chrome Mobile | Chrome | Mozilla/5.0 (Linux; Android 5.1.1; D6603 Build/23.4.A.1.264) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Mobile Safari/537.36 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MASMJS; rv:11.0) like Gecko |
| Mobile Safari | Safari | Mozilla/5.0 (iPhone; CPU iPhone OS 8_3 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12F70 Safari/600.1.4 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android; Mobile; rv:40.0) Gecko/40.0 Firefox/40.0 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MALNJS; rv:11.0) like Gecko |
| Mobile Safari | Safari | Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13D20 Safari/601.1 |
| Maxthon | Chrome | Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Maxthon/4.4.6.1000 Chrome/30.0.1599.101 Safari/537.36 |
| Other | Mozilla | Mozilla/5.0 |
| Iceweasel | Firefox | Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.2.1 |
| Android | Safari | Mozilla/5.0 (Linux; U; Android 4.1.2; fr-fr; GT-N8010 Build/JZO54K) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30 |
| IE | Internet Explorer | Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; ASU2JS) |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 5.0.1; Tablet; rv:44.0) Gecko/44.0 Firefox/44.0 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; MAPBJS; rv:11.0) like Gecko |
| IE | Internet Explorer | Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; managedpc; gdn/adcp) |
| Chrome Mobile | Chrome | Mozilla/5.0 (Linux; Android 5.1.1; D5803 Build/23.4.A.1.264) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Mobile Safari/537.36 |
| Mobile Safari | Safari | Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1 |
| Android | Safari | Mozilla/5.0 (Linux; U; Android 4.0.4; fr-fr; GT-P7510 Build/IMM76D) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30 |
| Chrome Mobile | Chrome | Mozilla/5.0 (Linux; Android 5.1.1; SAMSUNG SM-G920F-ORANGE Build/LMY47X) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.2 Chrome/38.0.2125.102 Mobile Safari/537.36 |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 7_1_1 like Mac OS X) AppleWebKit/537.51.2 (KHTML, like Gecko) Version/7.0 Mobile/11D201 Safari/9537.53 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; BOIE9;FRFR; rv:11.0) like Gecko |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 8_1_3 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B466 Safari/600.1.4 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; Touch; ASU2JS; rv:11.0) like Gecko |
| Chrome Mobile | Chrome | Mozilla/5.0 (Linux; Android 4.4.2; fr-fr; SAMSUNG GT-I9195 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Version/1.5 Chrome/28.0.1500.94 Mobile Safari/537.36 |
| Maxthon | Chrome | Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Maxthon/4.4.6.1000 Chrome/30.0.1599.101 Safari/537.36 |
| Chromium | Chrome | Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/47.0.2526.73 Chrome/47.0.2526.73 Safari/537.36 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 6.0; Mobile; rv:44.0) Gecko/44.0 Firefox/44.0 |
| IE | Internet Explorer | Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; Touch; MASEJS) |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 4.4.2; Tablet; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 5.1.1; Mobile; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; LCJB; rv:11.0) like Gecko |
| Edge | Microsoft Edge | Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Safari/537.36 Edge/14.14271 |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 9_0_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13A452 Safari/601.1 |
| Chrome Mobile iOS | Chrome | Mozilla/5.0 (iPad; CPU OS 9_2_1 like Mac OS X) AppleWebKit/601.1 (KHTML, like Gecko) CriOS/48.0.2564.104 Mobile/13D15 Safari/601.1.46 |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 8_1 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B410 Safari/600.1.4 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; Touch; MAARJS; rv:11.0) like Gecko |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MASEJS; rv:11.0) like Gecko |
| Chromium | Safari | Mozilla/5.0 (Linux; Ubuntu 14.04 like Android 4.4) AppleWebKit/537.36 Chromium/35.0.1870.2 Mobile Safari/537.36 |
| Mobile Safari | Safari | Mozilla/5.0 (iPhone; CPU iPhone OS 7_1_1 like Mac OS X) AppleWebKit/537.51.2 (KHTML, like Gecko) Version/7.0 Mobile/11D201 Safari/9537.53 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; MASEJS; rv:11.0) like Gecko |
| IE | Internet Explorer | Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; MASMJS) |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10B329 Safari/8536.25 |
| SeaMonkey | Firefox | Mozilla/5.0 (Windows NT 5.1; rv:42.0) Gecko/20100101 Firefox/42.0 SeaMonkey/2.39 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 4.4.4; Mobile; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; Win64; x64; Trident/7.0; rv:11.0) like Gecko |
| Firefox iOS | Firefox | Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) FxiOS/1.4 Mobile/13D15 Safari/601.1.46 |
| Chrome Mobile | Chrome | Mozilla/5.0 (Linux; Android 5.0.2; SAMSUNG SM-A500FU-ORANGE Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.3 Chrome/38.0.2125.102 Mobile Safari/537.36 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 4.4.4; Tablet; rv:44.0) Gecko/44.0 Firefox/44.0 |
| IE Mobile | Internet Explorer | Mozilla/5.0 (Mobile; Windows Phone 8.1; Android 4.0; ARM; Trident/7.0; Touch; rv:11.0; IEMobile/11.0; NOKIA; Lumia 635) like iPhone OS 7_0_3 Mac OS X AppleWebKit/537 (KHTML, like Gecko) Mobile Safari/537 |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 8_1_2 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B440 Safari/600.1.4 |
| IE | Internet Explorer | Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; ASJB; rv:11.0) like Gecko |
| Iceweasel | Firefox | Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.3.0 |
| Iceweasel | Firefox | Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.5.0 |
| Mobile Safari | Safari | Mozilla/5.0 (iPad; CPU OS 9_0 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13A344 Safari/601.1 |
| Firefox Mobile | Firefox | Mozilla/5.0 (Android 4.4.2; Mobile; rv:41.0) Gecko/41.0 Firefox/41.0 |
| Iceweasel | Firefox | Mozilla/5.0 (X11; Linux x86_64; rv:45.0) Gecko/20100101 Firefox/45.0 Iceweasel/45.0 |
