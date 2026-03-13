# Задача Терминал (Сеть) --> Роман Салий

1. Добавил интерфейс в vb, проверил название интерфейсов.

   - Команда `ip link show`.(они уже измененные на скриншоте)

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/1.png?raw=true" />

2. Отредактировал файл `/etc/netplan/50-cloud-init.yaml`

   - Добавил статические адреса на оба интерфейса.
   
   - Через `match` добвил макадреса и привязал к интерфейсам нормальные имена.

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/2.png?raw=true" />

3. Проверил поднялись ли интерфейсы и проверил их работоспособность.

   - `netplan status -a.`
   
   - `ping.`

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/3.png?raw=true" />

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/3-1.png?raw=true" />

4. Отредактировал и проверил `dns.`

   - `/etc/systemd/resolved.conf.`
   
   - `/etc/resolv.conf.`
   
   - Применил `sudo systemctl restart systemd-resolved.service.`
   
   - Проверил `nslookup ya.ru.`

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/4.png?raw=true" />

5. `Ssh` был установлен заранее скриншот (Состояния и портов).

<img src="https://github.com/krukVandal/Tms-Terminal-3-Network/blob/main/ScreenShot/5.png?raw=true" />

