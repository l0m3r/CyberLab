
# 📄 Cheatsheet: [curl]
> популярная утилита командной строки для передачи данных на сервер и с сервера по множеству протоколов (включая HTTP, HTTPS, FTP).


## 📋 Основные команды
| Команда   | Описание   | Пример                 |
|-----------|------------|------------------------|
| `команда` | что делает | `пример с параметрами` |
| `команда` | что делает | `пример`               |
| ...       | ...        | ...                    |

---

## 🔬 Расширенные параметры / Продвинутое использование

### Пример 1: [Название]
Описание конкретного сценария использования.

---

## 📚 Полезные ресурсы
- https://curl.se/


 1429  curl http://kslweb1.spb.ctf.su/first/level3/ -d 'want-flag=YES' 'code=1337'
 1430  curl http://kslweb1.spb.ctf.su/first/level3/ -d 'fun=Kaspersky & Summer & Lab'
 1431  curl http://kslweb1.spb.ctf.su/first/level3/ -d 'want-flag=YES' 'code=1337'
 1432  curl http://kslweb1.spb.ctf.su/first/level3/ -d '{"want-flag":"YES", "code":"1337"}'
 1433  curl http://kslweb1.spb.ctf.su/first/level3/ -d '{"want_flag":"YES", "code":"1337"}'
 1434  curl http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag":"YES", "code":"1337"}'
 1435  curl -X GET http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag":"YES", "code":"1337"}'
 1436  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag":"YES", "code":"1337"}'
 1437  curl http://kslweb1.spb.ctf.su/first/level4/
 1438  curl http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag":"YES", "code":"1337"}'
 1439  curl -h
 1440  curl http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag":"YES", "code":"1337"}' -v
 1441  curl http://kslweb1.spb.ctf.su/first/level4/ -d '{"want_flag=YES", "code=1337"}' -v
 1442  curl http://kslweb1.spb.ctf.su/first/level4/
 1443  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "want_flag=YES" "code=1337"
 1444  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "want_flag=YES"\ -d "code=1337"
 1445  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "want_flag=YES", "code=1337"
 1446  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "want_flag=YES" -d "code=1337"
 1447  curl -X POST http://kslweb1.spb.ctf.su/first/level5/
 1448  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky & Summer & Lab"
 1449  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky/& Summer & Lab"
 1450  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=KasperskySummer & Lab"
 1451  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky Summer & Lab"
 1452  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky Summer Lab"
 1453  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky & Summer Lab"
 1454  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky \& Summer Lab"
 1455  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky \\& Summer Lab"
 1456  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky //& Summer Lab"
 1457  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky /& Summer Lab"
 1458  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky+& Summer Lab"
 1459  curl -X POST http://kslweb1.spb.ctf.su/first/level4/ -d "fun=Kaspersky+&+Summer+Lab"
 1460  curl -X POST http://kslweb1.spb.ctf.su/first/level5/ -d "fun=Kaspersky+&+Summer+Lab"
 1461  curl -X POST http://kslweb1.spb.ctf.su/first/level5/ -d "fun=Kaspersky & Summer & Lab"
 1462  curl -X POST http://kslweb1.spb.ctf.su/first/level5/ -d "fun=Kaspersky+& Summer & Lab"
 1463  curl -X POST http://kslweb1.spb.ctf.su/first/level5/ ---data-urlencode "fun=Kaspersky & Summer & Lab"
 1464  curl -X POST http://kslweb1.spb.ctf.su/first/level5/ --data-urlencode "fun=Kaspersky & Summer & Lab"
 1465  curl -h
 1466  curl http://kslweb1.spb.ctf.su/first/level6/
 1467  curl http://kslweb1.spb.ctf.su/first/level6/ -h
 1468  curl http://kslweb1.spb.ctf.su/first/level6/ --header
 1469  curl http://kslweb1.spb.ctf.su/first/level6/ --header "SPbCTF=Pretty cool"
 1470  curl http://kslweb1.spb.ctf.su/first/level6/ --header "SPbCTF:Pretty cool"
 1471  curl http://kslweb1.spb.ctf.su/first/level7/
 1472  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1"
 1473  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:2"
 1474  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" --header "Cookie:2"
 1475  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" --header "Cookie1:2"
 1476  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" --header "Cookie1:"
 1477  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" --header "Cookie1:2"
 1478  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" --header "Cookie:2"
 1479  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" && url http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:2"
 1480  curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:1" && curl http://kslweb1.spb.ctf.su/first/level7/ --header  "Cookie:2"
 1481  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1"
 1482  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1, Cookie:2"
 1483  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1" "Cookie:2"
 1484  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1" -H "Cookie:2"
 1485  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1" -H "Cookie1:2"
 1486  curl http://kslweb1.spb.ctf.su/first/level7/ --header "Cookie:1,2"
 1487  curl -h
 1488  curl --help
 1489  curl --help all
 1490  curl http://kslweb1.spb.ctf.su/first/level7/ -b "Cookie:1,2"
 1491  curl http://kslweb1.spb.ctf.su/first/level7/ -b "Cookie:1"
 1492  curl http://kslweb1.spb.ctf.su/first/level7/ -c "Cookie:1"
 1493  curl http://kslweb1.spb.ctf.su/first/level7/ -c
 1494  curl --help all
 1495  ls -lah
 1496  mkdir spbctf
 1497  cd spbctf
 1498  nano cookie.txt
 1499  curl http://kslweb1.spb.ctf.su/first/level7/
 1500  curl http://kslweb1.spb.ctf.su/first/level7/ -c cookie.txt
 1501  nano cookie.txt
 1502  curl http://kslweb1.spb.ctf.su/first/level7/ -b
 1503  curl http://kslweb1.spb.ctf.su/first/level7/ -b "Cookie:1"
 1504  curl http://kslweb1.spb.ctf.su/first/level7/ -d "Cookie:1"
 1505  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie:1"
 1506  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie:1" -H "Cookie:100"
 1507  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie:1" -H "Cookie1:100"
 1508  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(echo c{1..100}={1..100} | sed 's/ /; /g')"
 1509  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(echo c{1..2}={1..2} | sed 's/ /; /g')"
 1510  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(echo c{1}={1..3} | sed 's/ /; /g')"
 1511  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(echo c1={1..3} | sed 's/ /; /g')"
 1512  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(echo c{1..3}={1..3} | sed 's/ /; /g')"
 1513  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(printf "c%d=%d; " {1..3})"
 1514  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(printf "c%d=%d; " {1..101})"
 1515  curl http://kslweb1.spb.ctf.su/first/level7/ -H "Cookie: $(printf "c%d=%d; " {1..201})"
 1516  curl http://kslweb1.spb.ctf.su/first/level8/
 1517  curl http://kslweb1.spb.ctf.su/first/level8/ -v
 1518  curl http://kslweb1.spb.ctf.su/first/level9/
 1519  curl http://kslweb1.spb.ctf.su/first/level9/ -v
 1520  curl http://kslweb1.spb.ctf.su/first/level9/ -H "Cookie:do_i_really_want_flag_for_level_nine=no; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011"
 1521  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Cookie:do_i_really_want_flag_for_level_nine=no; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011"
 1522  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=no; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011" -v
 1523  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=no; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011"
 1524  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=yes; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011"
 1525  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=yes; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011" -v\
 1526  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=yes; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011" -v
 1527  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Set-Cookie:do_i_really_want_flag_for_level_nine=yes; expires=No, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011" -v
 1528  curl http://kslweb1.spb.ctf.su/first/level9/ -v
 1529  curl -X POST http://kslweb1.spb.ctf.su/first/level9/ -H "Cookie:do_i_really_want_flag_for_level_nine=yes; expires=Tue, 19-Jan-2038 03:14:07 GMT; Max-Age=360846011" -v
 1530  curl http://kslweb1.spb.ctf.su/first/level10/ -v
 1531  curl http://kslweb1.spb.ctf.su/first/level10/
 1532  curl http://kslweb1.spb.ctf.su/first/level10/robot.txt
 1533  curl http://kslweb1.spb.ctf.su/first/level10/robots.txt
 1534  curl http://kslweb1.spb.ctf.su/first/level10/hidden_admin_panel_WOW.php
 1535  curl -h
