Point-to-Point протокол, часть систем типа "Точка-точка". 

PPP - протокол канального уровня, который позволяет установить соединение между двумя сетевыми узлами.

настройка интерфейса в cisco:
```
interface dialer
ip address negotiated
encapsulation ppp - Включение PPP
ppp authentication chap callin (Метод аутентификации)
ppp chap hostname <имя_пользователя>
ppp chap password <пароль>
```

![[IMG_Протокол PPP_Защита.png]]

Настройка PPPoE (Over Ethernet)
```
`interface GigabitEthernet0/0
no ip address
pppoe enable
pppoe-client
dial-pool-number 1`
```

![[Принцип работы протокола PPP.]]