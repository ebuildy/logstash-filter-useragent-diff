```sql
SELECT  t1.ua,t1.os,t2.os,t1.name,t2.name,t1.os_name,t2.os_family 
FROM dfs.tmp.`output1.json` t1 
JOIN dfs.tmp.`output2.json` t2 ON t1.id = t2.id;
```

| ua | name 1 | name 2 | os 1 | os 2 |
| ---| ------ | ------ | ---- | ---- |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:46.0) Gecko/20100101 Firefox/46.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; Touch; ASU2JS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:29.0) Gecko/20100101 Firefox/29.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux x86_64; rv:40.0) Gecko/20100101 Firefox/40.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; MDDRJS; rv:11.0) like Gecko | Windows 7 | Windows 7 | IE | Internet Explorer | Windows 7 | Windows |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:28.0) Gecko/20100101 Firefox/28.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Android 5.0.1; Mobile; rv:44.0) Gecko/44.0 Firefox/44.0 | Android 5.0.1 | Android 5.x | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (iPad; CPU OS 5_1_1 like Mac OS X) AppleWebKit/534.46 (KHTML, like Gecko) Version/5.1 Mobile/9B206 Safari/7534.48.3 | iOS 5.1.1 | Mac OS X (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:30.0) Gecko/20100101 Firefox/30.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.109 Safari/537.36 OPR/35.0.2066.68 | Windows 7 | Windows 7 | Opera | Opera | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux x86_64; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.3.0 | Linux | Linux | Iceweasel | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MAPBJS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 OPR/35.0.2066.82 | Mac OS X 10.11.3 | Mac OS X | Opera | Opera | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux x86_64; rv:45.0) Gecko/20100101 Firefox/45.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Linux; Android 5.1.1; D6603 Build/23.4.A.1.264) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Mobile Safari/537.36 | Android 5.1.1 | Android 5.x | Chrome Mobile | Chrome | Android | Android |
| Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.64 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MASMJS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (X11; Fedora; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Fedora | Linux | Chrome | Chrome | Fedora | Linux |
| Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:44.0) Gecko/20100101 Firefox/44.0.3 Waterfox/44.0.3 | Windows 10 | Windows 10 | Firefox | Firefox | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.118 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/600.1.25 (KHTML, like Gecko) Version/8.0 Safari/600.1.25 | Mac OS X 10.10.1 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:37.0) Gecko/20100101 Firefox/37.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.10; rv:39.0) Gecko/20100101 Firefox/39.0 | Mac OS X 10.10 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:39.0) Gecko/20100101 Firefox/39.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_5) AppleWebKit/537.78.2 (KHTML, like Gecko) Version/7.0.6 Safari/537.78.2 | Mac OS X 10.9.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.9; rv:39.0) Gecko/20100101 Firefox/39.0 | Mac OS X 10.9 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.103 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; rv:41.0) Gecko/20100101 Firefox/41.0 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2490.86 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 5.1; rv:34.0) Gecko/20100101 Firefox/34.0 | Windows XP | Windows XP | Firefox | Firefox | Windows XP | Windows |
| Mozilla/5.0 (iPhone; CPU iPhone OS 8_3 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12F70 Safari/600.1.4 | iOS 8.3 | iOS 8.3 (iPhone) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Android; Mobile; rv:40.0) Gecko/40.0 Firefox/40.0 | Android | Android Mobile | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MALNJS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 6.1; rv:45.0) Gecko/20100101 Firefox/45.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13D20 Safari/601.1 | iOS 9.2.1 | iOS 9 (iPhone) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 OPR/35.0.2066.82 | Windows 8 | Windows 8 | Opera | Opera | Windows 8 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Maxthon/4.4.6.1000 Chrome/30.0.1599.101 Safari/537.36 | Windows 8.1 | Windows 8.1 | Maxthon | Chrome | Windows 8.1 | Windows |
| Mozilla/5.0 (Linux; Android 5.0.2; SAMSUNG SM-T550 Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.3 Chrome/38.0.2125.102 Safari/537.36 | Android 5.0.2 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (Windows NT 6.0; rv:42.0) Gecko/20100101 Firefox/42.0 | Windows Vista | Windows Vista | Firefox | Firefox | Windows Vista | Windows |
| Mozilla/5.0 (Linux; Android 4.4.2; GT-P5210 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 4.4.2 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (Linux; Android 5.0.2; SAMSUNG SM-T810 Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.5 Chrome/38.0.2125.102 Safari/537.36 | Android 5.0.2 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 | Other | Unknown | Other | Mozilla | Other | Unknown |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.268 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:45.0) Gecko/20100101 Firefox/45.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 OPR/35.0.2066.82 | Linux | Linux | Opera | Opera | Linux | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Mac OS X 10.10.4 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.2.1 | Linux | Linux | Iceweasel | Firefox | Linux | Linux |
| Mozilla/5.0 (X11; Linux x86_64; rv:42.0) Gecko/20100101 Firefox/42.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.9; rv:42.0) Gecko/20100101 Firefox/42.0 | Mac OS X 10.9 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/45.0.2454.85 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Linux; U; Android 4.1.2; fr-fr; GT-N8010 Build/JZO54K) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30 | Android 4.1.2 | Android 4.x Tablet | Android | Safari | Android | Android |
| Mozilla/5.0 (Linux; Android 5.0.2; SM-T800 Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 5.0.2 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; ASU2JS) | Windows 8 | Windows 8 | IE | Internet Explorer | Windows 8 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.7; rv:43.0) Gecko/20100101 Firefox/43.0 | Mac OS X 10.7 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Mac OS X 10.11.4 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (Android 5.0.1; Tablet; rv:44.0) Gecko/44.0 Firefox/44.0 | Android 5.0.1 | Android 5.x Tablet | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Linux; Android 5.0.2; SM-T530 Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 5.0.2 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/44.0.2403.89 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; rv:35.0) Gecko/20100101 Firefox/35.0 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.80 Safari/537.36 | Linux | Linux | Chrome | Chrome | Linux | Linux |
| Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; MAPBJS; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; managedpc; gdn/adcp) | Windows 7 | Windows 7 | IE | Internet Explorer | Windows 7 | Windows |
| Mozilla/5.0 (Linux; Android 5.1.1; D5803 Build/23.4.A.1.264) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Mobile Safari/537.36 | Android 5.1.1 | Android 5.x | Chrome Mobile | Chrome | Android | Android |
| Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1 | iOS 9.1 | iOS 9 (iPhone) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:16.0) Gecko/20100101 Firefox/16.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Windows 8 | Windows 8 | Chrome | Chrome | Windows 8 | Windows |
| Mozilla/5.0 (Linux; U; Android 4.0.4; fr-fr; GT-P7510 Build/IMM76D) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30 | Android 4.0.4 | Android 4.x Tablet | Android | Safari | Android | Android |
| Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:40.0) Gecko/20100101 Firefox/40.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:37.0) Gecko/20100101 Firefox/37.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Linux; Android 4.4.2; Lenovo A7600-F Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/30.0.0.0 Safari/537.36 | Android 4.4.2 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:43.0) Gecko/20100101 Firefox/43.0 | Fedora | Linux | Firefox | Firefox | Fedora | Linux |
| Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 OPR/35.0.2066.82 | Windows 10 | Windows 10 | Opera | Opera | Windows 10 | Windows |
| Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:38.0) Gecko/20100101 Firefox/38.0 | Fedora | Linux | Firefox | Firefox | Fedora | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.109 Safari/537.36 | Mac OS X 10.9.5 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.103 Safari/537.36 | Linux | Linux | Chrome | Chrome | Linux | Linux |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Dragon/46.9.15.425 Chrome/46.0.2490.86 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/40.0.2214.91 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.3; rv:36.0) Gecko/20100101 Firefox/36.04 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:30.0) Gecko/20100101 Firefox/30.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5) AppleWebKit/601.1.56 (KHTML, like Gecko) Version/9.0 Safari/601.1.56 | Mac OS X 10.10.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Linux; Android 5.1.1; SAMSUNG SM-G920F-ORANGE Build/LMY47X) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.2 Chrome/38.0.2125.102 Mobile Safari/537.36 | Android 5.1.1 | Android 5.x | Chrome Mobile | Chrome | Android | Android |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/43.0.2357.130 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/45.0.2454.101 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (iPad; CPU OS 7_1_1 like Mac OS X) AppleWebKit/537.51.2 (KHTML, like Gecko) Version/7.0 Mobile/11D201 Safari/9537.53 | iOS 7.1.1 | iOS 7 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; BOIE9;FRFR; rv:11.0) like Gecko | Windows 7 | Windows 7 | IE | Internet Explorer | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; rv:29.0) Gecko/20100101 Firefox/29.0 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 5.1; rv:30.0) Gecko/20100101 Firefox/30.0 | Windows XP | Windows XP | Firefox | Firefox | Windows XP | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux i686 on x86_64; rv:44.0) Gecko/20100101 Firefox/44.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:42.0) Gecko/20100101 Firefox/42.0 DT-Browser/DTB7.42.0.19_01 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.11 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.11 | Mac OS X 10.10.4 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:44.0) Gecko/20100101 Firefox/44.0 | Windows 8 | Windows 8 | Firefox | Firefox | Windows 8 | Windows |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2490.71 Safari/537.36 | Linux | Linux | Chrome | Chrome | Linux | Linux |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Mac OS X 10.10.3 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (iPad; CPU OS 8_1_3 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B466 Safari/600.1.4 | iOS 8.1.3 | iOS 8.1 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; Touch; ASU2JS; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (Linux; Android 4.4.2; fr-fr; SAMSUNG GT-I9195 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Version/1.5 Chrome/28.0.1500.94 Mobile Safari/537.36 | Android 4.4.2 | Android 4.x | Chrome Mobile | Chrome | Android | Android |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:29.0) Gecko/20100101 Firefox/29.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Maxthon/4.4.6.1000 Chrome/30.0.1599.101 Safari/537.36 | Windows 7 | Windows 7 | Maxthon | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2553.0 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/47.0.2526.73 Chrome/47.0.2526.73 Safari/537.36 | Ubuntu | Ubuntu | Chromium | Chrome | Ubuntu | Linux |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:42.0) Gecko/20100101 Firefox/42.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; rv:6.0) Gecko/20100101 Firefox/6.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Android 6.0; Mobile; rv:44.0) Gecko/44.0 Firefox/44.0 | Android 6.0 | Android 6.x | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; Touch; MASEJS) | Windows 8 | Windows 8 | IE | Internet Explorer | Windows 8 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.6; rv:45.0) Gecko/20100101 Firefox/45.0 | Mac OS X 10.6 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Iridium/47.0 Safari/537.36 Chrome/47.0.2526.106 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:33.0) Gecko/20100101 Firefox/33.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 5.1; rv:37.0) Gecko/20100101 Firefox/37.0 | Windows XP | Windows XP | Firefox | Firefox | Windows XP | Windows |
| Mozilla/5.0 (Android 4.4.2; Tablet; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 | Android 4.4.2 | Android 4.x Tablet | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Android 5.1.1; Mobile; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 | Android 5.1.1 | Android 5.x | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Windows NT 6.1; rv:6.0.1) Gecko/20100101 Firefox/6.0.1 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; LCJB; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Safari/537.36 Edge/14.14271 | Windows 10 | Windows 10 | Edge | Microsoft Edge | Windows 10 | Windows |
| Mozilla/5.0 (iPad; CPU OS 9_0_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13A452 Safari/601.1 | iOS 9.0.2 | iOS 9 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/44.0.2403.125 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; rv:24.0; [eburo v5.0]) Gecko/20100101 Firefox/24.0 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (X11; Linux i686; rv:24.0) Gecko/20100101 Firefox/24.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Dragon/45.9.12.392 Chrome/45.0.2454.93 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (iPad; CPU OS 9_2_1 like Mac OS X) AppleWebKit/601.1 (KHTML, like Gecko) CriOS/48.0.2564.104 Mobile/13D15 Safari/601.1.46 | iOS 9.2.1 | iOS 9 (iPad) | Chrome Mobile iOS | Chrome | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.64 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Dragon/46.9.15.425 Chrome/46.0.2490.86 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_5) AppleWebKit/600.8.9 (KHTML, like Gecko) Version/7.1.8 Safari/537.85.17 | Mac OS X 10.9.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux i686) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.116 Safari/537.36 | Linux | Linux | Chrome | Chrome | Linux | Linux |
| Mozilla/5.0 (iPad; CPU OS 8_1 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B410 Safari/600.1.4 | iOS 8.1 | iOS 8.1 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:28.0) Gecko/20100101 Firefox/28.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Windows NT 6.1; rv:36.0) Gecko/20100101 Firefox/36.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.64 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; Touch; MAARJS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64; rv:37.0) Gecko/20100101 Firefox/37.0 | Windows 10 | Windows 10 | Firefox | Firefox | Windows 10 | Windows |
| Mozilla/5.0 (X11; Linux i686 on x86_64; rv:38.0) Gecko/20100101 Firefox/38.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; MASEJS; rv:11.0) like Gecko | Windows 8.1 | Windows 8.1 | IE | Internet Explorer | Windows 8.1 | Windows |
| Mozilla/5.0 (Linux; Ubuntu 14.04 like Android 4.4) AppleWebKit/537.36 Chromium/35.0.1870.2 Mobile Safari/537.36 | Android 4.4 | Ubuntu Touch (mobile) | Chromium | Safari | Android | Linux |
| Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:42.0) Gecko/20100101 Firefox/42.0 | Fedora | Linux | Firefox | Firefox | Fedora | Linux |
| Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.109 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.103 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_5) AppleWebKit/600.6.3 (KHTML, like Gecko) Version/6.2.6 Safari/537.85.15 | Mac OS X 10.8.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.109 Safari/537.36 | Windows Vista | Windows Vista | Chrome | Chrome | Windows Vista | Windows |
| Mozilla/5.0 (iPhone; CPU iPhone OS 7_1_1 like Mac OS X) AppleWebKit/537.51.2 (KHTML, like Gecko) Version/7.0 Mobile/11D201 Safari/9537.53 | iOS 7.1.1 | iOS 7 (iPhone) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.106 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Iridium/46.0 Safari/537.36 Chrome/46.0.2490.80 | Ubuntu | Ubuntu | Chrome | Chrome | Ubuntu | Linux |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:44.0) Gecko/20100101 Firefox/44.0 Cyberfox/44.0.2 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.5; rv:12.0) Gecko/20100101 Firefox/12.0 | Mac OS X 10.5 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; MASEJS; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.73 Safari/537.36 OPR/34.0.2036.41 | Windows 10 | Windows 10 | Opera | Opera | Windows 10 | Windows |
| Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0; MASMJS) | Windows 8 | Windows 8 | IE | Internet Explorer | Windows 8 | Windows |
| Mozilla/5.0 (Windows NT 6.3; rv:43.0) Gecko/20100101 Firefox/43.0 | Windows 8.1 | Windows 8.1 | Firefox | Firefox | Windows 8.1 | Windows |
| Mozilla/5.0 (Linux; Android 5.0.2; P023 Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 5.0.2 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10B329 Safari/8536.25 | iOS 6.1.3 | iOS 6 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Windows NT 6.1; rv:32.0) Gecko/20100101 Firefox/32.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (X11; Linux i686; rv:41.0) Gecko/20100101 Firefox/41.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_5) AppleWebKit/600.2.5 (KHTML, like Gecko) Version/6.2.2 Safari/537.85.11 | Mac OS X 10.8.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux x86_64; rv:41.0) Gecko/20100101 Firefox/41.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Windows NT 5.1; rv:42.0) Gecko/20100101 Firefox/42.0 SeaMonkey/2.39 | Windows XP | Windows XP | SeaMonkey | Firefox | Windows XP | Windows |
| Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.118 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 6.1; WOW64; rv:26.0) Gecko/20100101 Firefox/26.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Android 4.4.4; Mobile; rv:44.0.2) Gecko/44.0.2 Firefox/44.0.2 | Android 4.4.4 | Android 4.x | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.73 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 10.0; Win64; x64; Trident/7.0; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.1; rv:38.0) Gecko/20100101 20000523 Firefox/38.0 | Windows 7 | Windows 7 | Firefox | Firefox | Windows 7 | Windows |
| Mozilla/5.0 (Linux; Android 5.1.1; SAMSUNG SM-P600 Build/LMY47X) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.3 Chrome/38.0.2125.102 Safari/537.36 | Android 5.1.1 | Android 5.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:35.0) Gecko/20100101 Firefox/35.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) FxiOS/1.4 Mobile/13D15 Safari/601.1.46 | iOS 9.2.1 | iOS 9 (iPhone) | Firefox iOS | Firefox | iOS | iOS |
| Mozilla/5.0 (Linux; Android 4.4.2; SM-T530 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 4.4.2 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (X11; Linux i686; rv:43.0) Gecko/20100101 Firefox/43.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Linux; Android 5.0.2; SAMSUNG SM-A500FU-ORANGE Build/LRX22G) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.3 Chrome/38.0.2125.102 Mobile Safari/537.36 | Android 5.0.2 | Android 5.x | Chrome Mobile | Chrome | Android | Android |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.99 Safari/537.36 OPR/35.0.2070.100283 | Linux | Linux | Opera | Opera | Linux | Linux |
| Mozilla/5.0 (X11; Linux x86_64; rv:34.0) Gecko/20100101 Firefox/34.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Mozilla/5.0 (Android 4.4.4; Tablet; rv:44.0) Gecko/44.0 Firefox/44.0 | Android 4.4.4 | Android 4.x Tablet | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (Windows NT 5.1; rv:24.0) Gecko/20100101 Firefox/24.0 | Windows XP | Windows XP | Firefox | Firefox | Windows XP | Windows |
| Mozilla/5.0 (Mobile; Windows Phone 8.1; Android 4.0; ARM; Trident/7.0; Touch; rv:11.0; IEMobile/11.0; NOKIA; Lumia 635) like iPhone OS 7_0_3 Mac OS X AppleWebKit/537 (KHTML, like Gecko) Mobile Safari/537 | Windows Phone 8.1 | Windows Phone 8.1 | IE Mobile | Internet Explorer | Windows Phone | Windows |
| Mozilla/5.0 (iPad; CPU OS 8_1_2 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/8.0 Mobile/12B440 Safari/600.1.4 | iOS 8.1.2 | iOS 8.1 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10) AppleWebKit/600.1.25 (KHTML, like Gecko) Version/8.0 Safari/600.1.25 | Mac OS X 10.10 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 5.1; rv:28.0) Gecko/20100101 Firefox/28.0 | Windows XP | Windows XP | Firefox | Firefox | Windows XP | Windows |
| Mozilla/5.0 (Linux; Android 4.4.2; QOOQ Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.141 Safari/537.36 | Android 4.4.2 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; ASJB; rv:11.0) like Gecko | Windows 10 | Windows 10 | IE | Internet Explorer | Windows 10 | Windows |
| Mozilla/5.0 (Windows NT 6.0; rv:35.0) Gecko/20100101 Firefox/35.0 | Windows Vista | Windows Vista | Firefox | Firefox | Windows Vista | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5) AppleWebKit/534.57.7 (KHTML, like Gecko) Version/5.1.7 Safari/534.57.7 | Mac OS X 10.7.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.73 Safari/537.36 | Linux | Linux | Chrome | Chrome | Linux | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_5) AppleWebKit/600.6.3 (KHTML, like Gecko) Version/7.1.6 Safari/537.85.15 | Mac OS X 10.9.5 | Mac OS X | Safari | Safari | Mac OS X | Mac OS X |
| Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.82 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10.6; rv:41.0) Gecko/20100101 Firefox/41.0 | Mac OS X 10.6 | Mac OS X | Firefox | Firefox | Mac OS X | Mac OS X |
| Mozilla/5.0 (Linux; Android 4.4.2; fr-fr; SAMSUNG SM-T230 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Version/1.5 Chrome/28.0.1500.94 Safari/537.36 | Android 4.4.2 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.106 Safari/537.36 | Mac OS X 10.11.3 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:33.0) Gecko/20100101 Firefox/33.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.3.0 | Linux | Linux | Iceweasel | Firefox | Linux | Linux |
| Mozilla/5.0 (X11; Linux i686; rv:38.0) Gecko/20100101 Firefox/38.0 Iceweasel/38.5.0 | Linux | Linux | Iceweasel | Firefox | Linux | Linux |
| Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.109 Safari/537.36 | Mac OS X 10.11.2 | Mac OS X | Chrome | Chrome | Mac OS X | Mac OS X |
| Mozilla/5.0 (iPad; CPU OS 9_0 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13A344 Safari/601.1 | iOS 9.0 | iOS 9 (iPad) | Mobile Safari | Safari | iOS | iOS |
| Mozilla/5.0 (Android 4.4.2; Mobile; rv:41.0) Gecko/41.0 Firefox/41.0 | Android 4.4.2 | Android 4.x | Firefox Mobile | Firefox | Android | Android |
| Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:36.0) Gecko/20100101 Firefox/36.0 | Ubuntu | Ubuntu | Firefox | Firefox | Ubuntu | Linux |
| Mozilla/5.0 (Linux; Android 4.4.4; SM-T560 Build/KTU84P) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/48.0.2564.95 Safari/537.36 | Android 4.4.4 | Android 4.x Tablet | Chrome | Chrome | Android | Android |
| Mozilla/5.0 (X11; Linux x86_64; rv:24.0) Gecko/20100101 Firefox/24.0 | Linux | Linux | Firefox | Firefox | Linux | Linux |
| Opera/9.80 (Windows NT 6.2; WOW64) Presto/2.12.388 Version/12.15 | Windows 8 | Windows 8 | Opera | Opera | Windows 8 | Windows |
| Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.131 Safari/537.36 | Windows 7 | Windows 7 | Chrome | Chrome | Windows 7 | Windows |
| Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/40.0.2214.111 Adventurer/2.2.0.3 Safari/537.36 | Windows 10 | Windows 10 | Chrome | Chrome | Windows 10 | Windows |
| Mozilla/5.0 (X11; Linux x86_64; rv:45.0) Gecko/20100101 Firefox/45.0 Iceweasel/45.0 | Linux | Linux | Iceweasel | Firefox | Linux | Linux |
| Mozilla/5.0 (X11; Linux) AppleWebKit/538.15 (KHTML, like Gecko) Chrome/18.0.1025.133 Safari/538.15 Midori/0.5 | Linux | Linux | Chrome | Chrome | Linux | Linux |
