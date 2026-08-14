<div align="center">

<img src="Materials/png/information.png" alt="ADAPT-CONFIGS" width="1920">

</div>

<div align="center">

</br>

<img src="https://img.shields.io/badge/VLESS-0066FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/REALITY-00AA55?style=for-the-badge" />
<img src="https://img.shields.io/badge/SOCKS5-2F2F2F?style=for-the-badge" />
<img src="https://img.shields.io/badge/HYSTERIA2-00B4D8?style=for-the-badge" />
<img src="https://img.shields.io/badge/TROJAN-E63946?style=for-the-badge" />  
<img src="https://img.shields.io/badge/XTLS_VISION-7A3CFF?style=for-the-badge" />
<img src="https://img.shields.io/badge/XHTTP-FF8800?style=for-the-badge" />

</div>

</br>

### Принципы Конфигов

```txt
[✓] СТАБИЛЬНОСТЬ
    Каждый ключ проверен на реальную доступность.
    Никаких «мёртвых душ» — только рабочие серверы.
    Дубли исключены, нумерация сквозная и актуальная.

[✓] МИНИМАЛИЗМ
    Убираем всё лишнее: рекламные хвосты, громоздкие комментарии,
    дублирующиеся параметры. Только необходимая информация.

[✓] МАСКИРОВКА
    Конфиги заточены под обход DPI с помощью:
    Reality (подмена SNI на легитимный), xHTTP/gRPC поверх TLS,
    XMUX (фрагментация и перемешивание пакетов).
    Fingerprint браузера (Chrome/Firefox/Safari) подобран под SNI.

[✓] СОВМЕСТИМОСТЬ
    Поддерживаются все популярные клиенты:
    v2rayN, v2rayNG, Nekobox, Sing-box, FoxRay, Streisand.
    Никаких экзотических параметров, ломающих импорт.

[✓] REALITY
    Основной метод защиты канала.
    Используется связка XTLS-Vision для маскировки под обычный HTTPS-трафик.
    Полностью исключает обнаружение по сертификату.

[✓] XTLS VISION
    Включён там, где уместен (TCP-поток).
    Обеспечивает нулевую длину и обфускацию handshake.
    Не применяется с XMUX/gRPC/xHTTP — там работает транспортный уровень.

[✓] XHTTP
    Основной транспорт для агрессивной маскировки.
    Используется stream-one и packet-up режимы.
    Совместим с CDN (Cloudflare, Fastly и др.) для дополнительной скрытности.

[✓] DPI BYPASS
    Каждый конфиг спроектирован для обхода глубокой инспекции:
    - пакетная маскировка
    - рандомизация размера и таймингов
    - правдоподобный SNI и Fingerprint
    - обход блокировок по протоколам

[✗] ЛИШНИЕ НАСТРОЙКИ
    Без "мусора": неиспользуемых transport, пустых headerType,
    бессмысленных дублей параметров. Всё строго по делу.

[✗] УСТАРЕВШИЕ РЕШЕНИЯ
    Никакого KCP, TCP без obfuscation, старых версий VLESS.
    Только актуальные транспортные протоколы и методы обфускации.

[✗] ПЕРЕГРУЖЕННЫЕ КОНФИГИ
    Каждый URI оптимизирован по длине.
    Убраны избыточные query-параметры, длинные host-строки,
    неработающие опции. Баланс между информативностью и размером.

[✗] МАРКЕТИНГОВЫЙ ШУМ
    Вместо рекламных слоганов — чёткие флаги стран, номер и SNI.
    Списки очищены от мусорных эмодзи и бессмысленных тегов.
    Только сухие факты для быстрой оценки конфига. 
```

### Характеристики

<div align="center"> 

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:1a1a2e&height=180&section=header&text=Adapt%20%2F%20VPN&fontSize=40&fontColor=ffffff&fontAlignY=35&animation=fadeIn"/>

</div>

```yaml
ПРОТОКОЛЫ:
  Основные: VLESS, Trojan, Shadowsocks, Hysteria2
  Транспорт: TCP(Reality), xHTTP, gRPC, WebSocket(TLS)
  Безопасность: Reality(TLS 1.3), TLS
  Шифрование: None (XMUX обфускация), SS-методы

НАЗНАЧЕНИЕ:
  - Все ресурсы (RU + глобальные)
  - Обход DPI, корпоративные/домашние/мобильные сети
  - Адаптивная маршрутизация

ЗАДЕРЖКА/НАГРУЗКА: Низкая-Высокая (автоадаптация)
МАСКИРОВКА: Усиленная (XMUX + рандомизация Fingerprint + подмена CDN)

XMUX: Включён
PACKET MASKING: Включён

СТАБИЛЬНОСТЬ: Максимальная (диверсификация SNI + портов)

SNI-ПУЛ (все):
  id.vk.ru, smartcaptcha.yandexcloud.net, cdn.tracker.yandex.net
  *.minzt.su, *.sellflow.org
  *.yandex.ru, *.yandex.net, api-maps.yandex.ru, cloud.mail.ru
  *.vk.com, *.vk.ru, userapi.com, yastatic.net
  ads.x5.ru, web.max.ru, dzen.ru, rutube.ru
  gosuslugi.ru, api.ok.ru, avito.ru, kinopoisk.ru
  www.apple.com, www.tesla.com, www.cloudflare.com, wikipedia.org
  global.fastly.com, fastly.net, amazon.com, azure.com
  deepl.com, telegraph.co.uk, parisjetaime.com, iamsterdam.com
  www.sony.com, www.nvidia.com, login.ns.nl, jp1.cyphervpn.pro
  www.paypal.com, www.intel.com, www.samsung.com
  *.oncloudnineservicestreang.com, pro-de.emrata.top

ПОРТЫ (все):
  TCP: 443, 8443, 9445, 3443, 6443, 55861, 9823
  gRPC: 444, 16923, 47884, 56625, 52727
  xHTTP: 80, 443, 5443, 2083, 43264
  WebSocket: 80, 443, 8090

ПРИМЕЧАНИЕ: Для RU-сегмента использовать только подтверждённые российские SNI из списка выше
```

<div align="center"> 

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:000000&height=100&section=footer"/> 

</div>

</br>

### Отличия

| Протокол | Суть |
|---|---|
| **VLESS + REALITY** | Имитация HTTPS без своего TLS-сертификата. Максимальная маскировка, высокий обход DPI |
| **SOCKS5** | Универсальный прокси для TCP/UDP. Без шифрования, не для обхода DPI |
| **Hysteria2** | QUIC (UDP), высокая скорость, устойчив к потерям пакетов. Маскируется под HTTP/3 |
| **Trojan** | TLS-маскировка под обычный HTTPS. Нужен свой домен и сертификат |

---

### VLESS + REALITY

Лёгкий протокол из экосистемы Xray, использующий TLS вместо собственного шифрования — меньше сигнатур, сложнее обнаружить.
**REALITY** имитирует TLS-соединение к реальному популярному сайту, не требуя своего сертификата — трафик выглядит как обычный HTTPS.

**Плюсы:** высокая устойчивость к DPI · минимум уникальных сигнатур · без TLS-сертификата · высокая производительность · простая настройка

```
Client ➔ VLESS ➔ REALITY ➔ TCP ➔ Internet
```

---

### SOCKS5

Прокси-протокол уровня приложений для пересылки TCP/UDP-трафика. Не создаёт туннель и не шифрует данные сам по себе.

**Плюсы:** высокая скорость · низкие накладные расходы · TCP + UDP · простая настройка · широкая совместимость
**Минусы:** нет собственного шифрования · не скрывает факт использования прокси · нужна поддержка на стороне приложения

```
Application ➔ SOCKS5 Proxy ➔ Destination Server
```

**Применение:** браузеры, торренты, игры, тестирование, точечное перенаправление трафика.
**Безопасность:** сам по себе не шифрует — используйте вместе с TLS/Shadowsocks.

---

### Hysteria2

Протокол на базе QUIC (UDP) для сетей с активной фильтрацией и потерями пакетов. Маскируется под HTTP/3.

**Плюсы:** высокая скорость · низкая задержка · быстрое восстановление соединения · устойчивость к сетевым помехам

```
Client ➔ Hysteria2 ➔ QUIC (UDP) ➔ Internet
```

**Применение:** нестабильные сети, стриминг, игры, активный DPI.
**Ограничение:** некоторые провайдеры блокируют нестандартный QUIC-трафик.

---

### Trojan

Маскирует трафик под обычный HTTPS, используя стандартный TLS без собственного handshake.

**Плюсы:** высокая совместимость · простое развёртывание · устойчивость к DPI · стандартные HTTPS-механизмы

```
Client ➔ Trojan ➔ TLS ➔ TCP ➔ Internet
```

**Применение:** обход ограничений, маскировка под HTTPS, серверы с собственным доменом и сертификатом.
**Безопасность:** уровень защиты = уровень TLS. Держите TLS и сервер обновлёнными.

---

### Что выбрать?

- **VLESS + REALITY** — универсальный выбор по умолчанию: скорость + маскировка + устойчивость к DPI.
- **Hysteria2** — если важнее всего скорость и стабильность в плохих сетях (стриминг, игры).
- **Trojan** — если нужен трафик, неотличимый от HTTPS, и есть свой домен/сертификат.
- **SOCKS5** — точечное проксирование приложений, не замена полноценному обходу DPI.

> **По умолчанию:** VLESS + REALITY. Для максимальной скорости при неограниченном UDP — Hysteria2.

</br>

#### Теги репозитория

<div align="center">

<img src="https://img.shields.io/badge/XRAY-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/REALITY-16A34A?style=flat-square" />
<img src="https://img.shields.io/badge/VLESS-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/XHTTP-DC2626?style=flat-square" />
<img src="https://img.shields.io/badge/SOCKS5-525252?style=flat-square" />
<img src="https://img.shields.io/badge/TROJAN-B91C1C?style=flat-square" />
<img src="https://img.shields.io/badge/HYSTERIA2-0284C7?style=flat-square" />
<img src="https://img.shields.io/badge/DPI_BYPASS-F97316?style=flat-square" />
<img src="https://img.shields.io/badge/CAMOUFLAGE-7C3AED?style=flat-square" />
<img src="https://img.shields.io/badge/SING_BOX-0891B2?style=flat-square" />
<img src="https://img.shields.io/badge/FREE_INTERNET-16A34A?style=flat-square" />

</div>

</br>

<div align="center">

<a href="https://github.com/PrinceVSFX/Adapt-Configs/blob/main/LICENSE">
  <img src="https://img.shields.io/badge/LICENSE-MIT-green?style=for-the-badge" />
</a>

<a href="https://github.com/PrinceVSFX/Adapt-Configs/blob/main/DISCLAIMER">
  <img src="https://img.shields.io/badge/DISCLAIMER-READ-orange?style=for-the-badge" />
</a>

</div>
