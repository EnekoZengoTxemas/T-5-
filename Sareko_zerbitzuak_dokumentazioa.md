# Sareko zerbitzuak eta Internet – Dokumentazioa

## 1. DNS

DNS zerbitzaria `WindowsZerbitzaria` makinan dago (192.168.5.1) eta `eklipse.eus` domeinuaren izenak ebazten ditu.

| Zona / elementua | Edukia |
|---|---|
| Zona zuzena | `eklipse.eus` |
| Zona alderantzizkoa | `5.168.192.in-addr.arpa` |
| Birbidaltzaile baldintzatua | `google` → 8.8.8.8 |

Zona zuzenean ostalarien erregistroak (A) daude:

| Izena | Mota | Datua |
|---|---|---|
| windowszerbitzaria | Host (A) | 192.168.5.1 |
| eklipse.eus (zona bera) | Host (A) | 192.168.5.1 |
| jitsi | Host (A) | 192.168.5.8 |

Zona alderantzizkoan `jitsi` ostalariaren erregistroa dago:

| IP | Mota | Datua |
|---|---|---|
| 192.168.5.8 | Puntero (PTR) | jitsi.eklipse.eus |

**Zona zuzena:**

![Zona zuzena](img/21_dns_zona_zuzena.png)

**Zona alderantzizkoa:**

![Zona alderantzizkoa](img/22_dns_zona_alderantzizkoa.png)

**Birbidaltzaile baldintzatua:**

![Birbidaltzaile baldintzatua](img/23_dns_birbidaltzaile_baldintzatua.png)

**Probak:** domeinuko bezero batetik `nslookup` bidez bi zonak ondo erantzuten dute. `jitsi.eklipse.eus` izenak 192.168.5.8 helbidea ematen du, eta 192.168.5.8 helbideak `jitsi.eklipse.eus` izena. Erantzuten duen zerbitzaria 192.168.5.1 da.

![nslookup probak](img/31_dns_nslookup.png)

---

## 2. DHCP

DHCP zerbitzaria `WindowsZerbitzaria` makinan dago (192.168.5.1). `eklipse` izeneko ámbitoa sortu da 192.168.5.0 azpisarerako.

| Parametroa | Balioa |
|---|---|
| Ámbitoa | 192.168.5.0 (`eklipse`) |
| Banatzeko IP tartea | 192.168.5.100 – 192.168.5.150 |
| 003 Enrutadorea (irteera-atea) | 192.168.5.254 |
| 006 DNS zerbitzaria | 192.168.5.1 |
| 015 Domeinu-izena | eklipse.eus |

**Helbide-multzoa:**

![Helbide-multzoa](img/27_dhcp_helbide_multzoa.png)

**Ámbitoaren aukerak** (irteera-atea, DNS eta domeinu-izena):

![Ámbitoaren aukerak](img/30_dhcp_ambito_aukerak.png)

**Alokairuak:** bi bezerok jaso dute helbidea.

| IP | Bezeroa | Mota |
|---|---|---|
| 192.168.5.101 | Ubuntu-zerbitzaria | DHCP |
| 192.168.5.105 | WB-Eneko.eklipse.eus | Erreserba (aktiboa) |

![Alokairuak](img/28_dhcp_alokairuak.png)

**Erreserba:** 192.168.5.105 helbidea `WB-Eneko.eklipse.eus` ekipoarentzat erreserbatuta dago.

![Erreserba](img/29_dhcp_erreserba.png)

**Bezeroa:** domeinuko bezeroak 192.168.5.105 helbidea, 255.255.255.0 maskara, 192.168.5.254 irteera-atea eta 192.168.5.1 DNS zerbitzaria jasotzen ditu (DNS atzizkia: `eklipse.eus`).

![Bezeroaren sare-konfigurazioa](img/20_dhcp_bezeroa_ipconfig.png)

---

## 3. Jitsi (audio- eta bideo-zerbitzaria)

Jitsi Meet Linux zerbitzari batean dago instalatuta (`jitsi`, 192.168.5.8) eta `jitsi.eklipse.eus` izenarekin ebazten da, DNS zerbitzariaren A eta PTR erregistroei esker. Zerbitzu berak audioa eta bideoa kudeatzen ditu bileretan.

`jitsi-videobridge2` zerbitzua gaituta dago eta martxan (`active (running)`):

![Jitsi Videobridge zerbitzua](img/24_jitsi_videobridge_egoera.png)

Bezeroak zerbitzura izenaren bidez sartzen dira (`https://jitsi.eklipse.eus`):

![Jitsi DNS bidez](img/25_jitsi_dns_bidez.png)

Proba gisa `Prueba1` bilera sortu da, bi partaiderekin (Jokin eta Joan) eta txata erabiliz:

![Bilera proba](img/26_jitsi_bilera_proba.png)
