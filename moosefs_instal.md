### Установку MooseFs можно найти в документации: 
[PDF с официальног сайта](http://www.moosefs.org/tl_files/manpageszip/moosefs-step-by-step-tutorial-v.1.1.pdf)

### Старт MooseFS:

Запускаем master: 
```
/usr/sbin/mfsmaster start
```
Запускаем GGI monitor, который отображает текущий статус системе в браузере:
```
/usr/sbin/mfscgiserv
```
Запускаем metalogger: 
```
/usr/sbin/mfsmetalogger start
```
Запускаем chunkservers:
```
/usr/sbin/mfschunkserver start
```
Создаем папку, к которой будет примонтирована сетевая файловая система:
```
mkdir -p /mnt/mfs
```
Монтируем MooseFS:
```
/usr/bin/mfsmount /mnt/mfs -H mfsmaster
```
