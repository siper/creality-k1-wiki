---
comments: true
---
# Настройка камеры

В стандартном интерфейсе, камера доступна без дополнительных манипуляций. Для кастомных интерфейсов требуется дополнительная настройка.
Для Fluidd и Mainsail есть настройка камеры прямо из web интерфейса. Однако удобнее добавить камеру через файл конфигурации Moonraker,
т.к. его потом можно скопировать и сохранить, а так же камера будет доступна и Fluidd и в Mainsail без дополнительных настроек.

Чтобы добавить камеру, откройте файл `moonraker.conf` и добавьте туда следующий блок кода, подставив IP адрес своего принтера:

```yaml
[webcam CHAMBER]
location: printer
enabled: True
service: mjpegstreamer
target_fps: 15
icon: mdiPrinter3d
stream_url: http://<ip адрес принтера>:8080/?action=stream
snapshot_url: http://<ip адрес принтера>:8080/?action=snapshot
flip_horizontal: False
flip_vertical: False
rotation: 0
aspect_ratio: 4:3
```