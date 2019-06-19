Zadanie 1
---------

![zadanie 1](zadanie-1.svg)

1. Zaprojektuj oraz przygotuj prototyp rozwiązania z wykorzystaniem oprogramowania ``VirtualBox`` lub podobnego. 
Zaproponuj rozwiązanie spełniające poniższe wymagania:
   * Usługodawca zapewnia domunikację z siecią internet poprzez interfejs ``eth0`` ``PC0``
   * Zapewnij komunikację z siecią internet na poziomie ``LAN1`` oraz ``LAN2``
   * Dokonaj takiego podziału sieci o adresie ``172.22.128.0/17`` aby w ``LAN1`` można było zaadresować ``500`` adresów natomiast w LAN2 ``5000`` adresów    
   * Przygotuj dokumentację powyższej architektury w formie graficznej w programie ``DIA``
   
   
2.Rozwiązanie zadania
---------------------
2.1
---
1. Dane jest, że komunikację z siecią internet zapewnia usługodawca (dla ``eth0`` i ``PC0``).
2. Należy dokonać podziału sieci o adresie ``172.22.128.0/17``
  * 500 adresów w ``LAN1``
  * 5000 adresów w ``LAN2``.
  
2.2
---
1. Podział sieci.
| ilość | netmaska | adres |
|:--------------|:----|:--------------|
| 500 urządzeń  | /23 | 255.255.254.0 |
| 5000 urządzeń | /19 | 255.255.224.0 |

| IP startowy | 172.22.128.0    | podany adres                                                                      |
|   ``LAN1``  | 172.22.128.0/23 | orzystając z obliczeń w kalkulatorze - kolejne adresy w /19 zaczynają się od 160
|   ``LAN2``  | 172.22.160.0/19 | Korzystając z obliczeń w kalkulatorze - kolejne adresy w /19 zaczynają się od 160 |


 
