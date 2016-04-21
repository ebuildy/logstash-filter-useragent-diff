# Basic

```sql
SELECT DISTINCT t1.os || t2.os, t1.os,t2.os
FROM dfs.tmp.`output1.json` t1
JOIN dfs.tmp.`output2.json` t2 ON t1.id = t2.id
WHERE t1.os <> t2.os;
```

| duplicate_key | os 1 | os 2 |
| ------------- | ---- | ---- |
| OtherUnknown                      | Other                 | Unknown                |
| Mac OS X 10.11Mac OS X            | Mac OS X 10.11        | Mac OS X               |
| Mac OS X 10.11.3Mac OS X          | Mac OS X 10.11.3      | Mac OS X               |
| Mac OS X 10.10Mac OS X            | Mac OS X 10.10        | Mac OS X               |
| Mac OS X 10.6Mac OS X             | Mac OS X 10.6         | Mac OS X               |
| iOS 9.2.1iOS 9 (iPad)             | iOS 9.2.1             | iOS 9 (iPad)           |
| Mac OS X 10.9Mac OS X             | Mac OS X 10.9         | Mac OS X               |
| Mac OS X 10.10.5Mac OS X          | Mac OS X 10.10.5      | Mac OS X               |
| Linux 3.16.0Linux                 | Linux 3.16.0          | Linux                  |
| Mac OS X 10.7Mac OS X             | Mac OS X 10.7         | Mac OS X               |
| Mac OS X 10.9.5Mac OS X           | Mac OS X 10.9.5       | Mac OS X               |
| Mac OS X 10.11.2Mac OS X          | Mac OS X 10.11.2      | Mac OS X               |
| Mac OS X 10.6.8Mac OS X           | Mac OS X 10.6.8       | Mac OS X               |
| Mac OS X 10.8Mac OS X             | Mac OS X 10.8         | Mac OS X               |
| iOS 9.2.1iOS 9 (iPhone)           | iOS 9.2.1             | iOS 9 (iPhone)         |
| FedoraLinux                       | Fedora                | Linux                  |
| Mac OS X 10.7.5Mac OS X           | Mac OS X 10.7.5       | Mac OS X               |
| Linux 3.14.32Linux                | Linux 3.14.32         | Linux                  |
| Android 5.1.1Android 5.x          | Android 5.1.1         | Android 5.x            |
| Android 4.4.2Android 4.x Tablet   | Android 4.4.2         | Android 4.x Tablet     |
| Mac OS X 10.8.5Mac OS X           | Mac OS X 10.8.5       | Mac OS X               |
| Mac OS X 10.11.1Mac OS X          | Mac OS X 10.11.1      | Mac OS X               |
| Android 5.0.2Android 5.x Tablet   | Android 5.0.2         | Android 5.x Tablet     |
| iOS 9.2iOS 9 (iPad)               | iOS 9.2               | iOS 9 (iPad)           |
| Windows RT 8.1Windows 8.1         | Windows RT 8.1        | Windows 8.1            |
| Chrome OS 3912.101.0Chrome OS     | Chrome OS 3912.101.0  | Chrome OS              |
| Chrome OS 4319.74.0Chrome OS      | Chrome OS 4319.74.0   | Chrome OS              |
| Android 5.0.2Android 5.x          | Android 5.0.2         | Android 5.x            |
| Mac OS X 10.10.4Mac OS X          | Mac OS X 10.10.4      | Mac OS X               |
| Android 5.0Android 5.x            | Android 5.0           | Android 5.x            |
| Android 4.4.2Android 4.x          | Android 4.4.2         | Android 4.x            |
| Mac OS X 10.5Mac OS X             | Mac OS X 10.5         | Mac OS X               |
| Mac OS X 10.5.8Mac OS X           | Mac OS X 10.5.8       | Mac OS X               |
| Android 5.1.1Android 5.x Tablet   | Android 5.1.1         | Android 5.x Tablet     |
| Android 4.4.4Android 4.x          | Android 4.4.4         | Android 4.x            |
| Chrome OS 7647.84.0Chrome OS      | Chrome OS 7647.84.0   | Chrome OS              |
| Android 4.1.2Android 4.x Tablet   | Android 4.1.2         | Android 4.x Tablet     |
| Android 5.1Android 5.x            | Android 5.1           | Android 5.x            |
| Android 4.2.2Android 4.x Tablet   | Android 4.2.2         | Android 4.x Tablet     |
| iOS 9.1iOS 9 (iPad)               | iOS 9.1               | iOS 9 (iPad)           |
| iOS 9.2iOS 9 (iPhone)             | iOS 9.2               | iOS 9 (iPhone)         |
| Mac OS X 10.10.2Mac OS X          | Mac OS X 10.10.2      | Mac OS X               |
| Linux 3.2.0Linux                  | Linux 3.2.0           | Linux                  |
| iOS 8.4.1iOS 8.4 (iPad)           | iOS 8.4.1             | iOS 8.4 (iPad)         |
| iOS 8.4iOS 8.4 (iPad)             | iOS 8.4               | iOS 8.4 (iPad)         |
| Mac OS X 10.10.3Mac OS X          | Mac OS X 10.10.3      | Mac OS X               |
| iOS 7.1.2iOS 7 (iPhone)           | iOS 7.1.2             | iOS 7 (iPhone)         |
| iOS 8.3iOS 8.3 (iPad)             | iOS 8.3               | iOS 8.3 (iPad)         |
| Android 4.3Android 4.x            | Android 4.3           | Android 4.x            |
| Mac OS X 10.11.0Mac OS X          | Mac OS X 10.11.0      | Mac OS X               |
| Android 6.0.1Android 6.x          | Android 6.0.1         | Android 6.x            |
| Mac OS X 10.11.4Mac OS X          | Mac OS X 10.11.4      | Mac OS X               |
| Android 5.0.1Android 5.x          | Android 5.0.1         | Android 5.x            |
| iOS 7.1.2iOS 7 (iPad)             | iOS 7.1.2             | iOS 7 (iPad)           |
| iOS 5.1.1Mac OS X (iPad)          | iOS 5.1.1             | Mac OS X (iPad)        |
| Mac OS X 10.10.1Mac OS X          | Mac OS X 10.10.1      | Mac OS X               |
| iOS 8.3iOS 8.3 (iPhone)           | iOS 8.3               | iOS 8.3 (iPhone)       |
| AndroidAndroid Mobile             | Android               | Android Mobile         |
| Android 5.0.1Android 5.x Tablet   | Android 5.0.1         | Android 5.x Tablet     |
| iOS 9.1iOS 9 (iPhone)             | iOS 9.1               | iOS 9 (iPhone)         |
| Android 4.0.4Android 4.x Tablet   | Android 4.0.4         | Android 4.x Tablet     |
| iOS 7.1.1iOS 7 (iPad)             | iOS 7.1.1             | iOS 7 (iPad)           |
| iOS 8.1.3iOS 8.1 (iPad)           | iOS 8.1.3             | iOS 8.1 (iPad)         |
| Android 6.0Android 6.x            | Android 6.0           | Android 6.x            |
| iOS 9.0.2iOS 9 (iPad)             | iOS 9.0.2             | iOS 9 (iPad)           |
| iOS 8.1iOS 8.1 (iPad)             | iOS 8.1               | iOS 8.1 (iPad)         |
| Android 4.4Ubuntu Touch (mobile)  | Android 4.4           | Ubuntu Touch (mobile)  |
| iOS 7.1.1iOS 7 (iPhone)           | iOS 7.1.1             | iOS 7 (iPhone)         |
| iOS 6.1.3iOS 6 (iPad)             | iOS 6.1.3             | iOS 6 (iPad)           |
| Android 4.4.4Android 4.x Tablet   | Android 4.4.4         | Android 4.x Tablet     |
| iOS 8.1.2iOS 8.1 (iPad)           | iOS 8.1.2             | iOS 8.1 (iPad)         |
| iOS 9.0iOS 9 (iPad)               | iOS 9.0               | iOS 9 (iPad)           |
