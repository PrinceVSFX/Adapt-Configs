<div align="center">

<img src="Materials/png/information.png" alt="ADAPT-CONFIGS" width="1920">

</br>

<img src="https://img.shields.io/badge/VLESS-0066FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/REALITY-00AA55?style=for-the-badge" />
<img src="https://img.shields.io/badge/XTLS_VISION-7A3CFF?style=for-the-badge" />
<img src="https://img.shields.io/badge/XHTTP-FF8800?style=for-the-badge" />

</div>

</br>

### Принципы Конфигов

```txt
[✓] СТАБИЛЬНОСТЬ
[✓] МИНИМАЛИЗМ
[✓] МАСКИРОВКА
[✓] СОВМЕСТИМОСТЬ

[✓] REALITY
[✓] XTLS VISION
[✓] XHTTP
[✓] DPI BYPASS

[✗] ЛИШНИЕ НАСТРОЙКИ
[✗] УСТАРЕВШИЕ РЕШЕНИЯ
[✗] ПЕРЕГРУЖЕННЫЕ КОНФИГИ
[✗] МАРКЕТИНГОВЫЙ ШУМ
```

### Характеристики

**BLACK / KEPLER**

```yaml
ПРОФИЛЬ: Агрессивный

ОСНОВА:
  - xHTTP
  - Reality

ПРЕДНАЗНАЧЕНИЕ:
  - Жёсткий DPI
  - Фильтрация провайдера
  - Ограниченные сети
  - Сложные условия подключения

ЗАДЕРЖКА: СРЕДНЯЯ
НАГРУЗКА: СРЕДНЯЯ
МАСКИРОВКА: УСИЛЕННАЯ

XMUX: ВКЛЮЧЁН
PACKET MASKING: ВКЛЮЧЁН

СТАБИЛЬНОСТЬ: ВЫСОКАЯ
``` 

</br>

**WHITE / ALBEDO**

```yaml
ПРОФИЛЬ: Стабильный

ОСНОВА:
  - Reality
  - XTLS Vision

ПРЕДНАЗНАЧЕНИЕ:
  - Браузер
  - YouTube
  - Telegram
  - Discord
  - Игры

ЗАДЕРЖКА: НИЗКАЯ
НАГРУЗКА: НИЗКАЯ
МАСКИРОВКА: СТАНДАРТНАЯ

СТАБИЛЬНОСТЬ: ВЫСОКАЯ
```

### Стек технологий

```yaml

**Безопасность**

`VLESS`
`REALITY`
`XTLS Vision`
`TLS Camouflage`

**Транспорт**

`TCP`
`xHTTP`
`gRPC`
`WebSocket`

**Оптимизация**

`DPI Bypass`
`Packet-Up`
`XMUX`
`Padding`
```

### Транспорты

```yaml
TCP:
  Для: Стабильности
  Особенность: Классический транспорт

xHTTP:
  Для: Продвинутого обхода DPI
  Особенность: Современный и агрессивный

gRPC:
  Для: Длительных соединений
  Особенность: Multiplexing и стабильный throughput

WebSocket:
  Для: CDN-совместимости
  Особенность: Универсальный транспорт
```

### Маскировка Трафика

```txt
Yandex
├─ Поисковая система

mwscdn
├─ CDN инфраструктура

RBC
├─ Медиа-платформа

Beget
├─ Хостинг-провайдер

storage.yandex
├─ Облачное хранилище

CDN Endpoints
├─ Сеть доставки контента
```

**Результат**

*Трафик выглядит как обычный HTTPS/CDN.*

### Архитектура Reality

**Цепочка Подключения**

```txt
КЛИЕНТ
   │
   ▼
VLESS + REALITY
   │
   ▼
TLS МАСКИРОВКА
   │
   ▼
ЦЕЛЕВОЙ САЙТ
```

**Защитные Механизмы**

```txt
✓ Browser Fingerprinting

✓ Реальный SNI

✓ TLS Camouflage

✓ DPI Resistance
```

**Результат**

*DPI не видит отличий от обычного HTTPS-трафика.*

### Выбор Профиля

```txt
НУЖНА СТАБИЛЬНОСТЬ: WHITE
│
├─ Reality + Vision
│
└─ WHITE / ALBEDO
   ├─ YouTube
   ├─ Discord
   ├─ Telegram
   └─ Игры
```

---

```txt
ПРОВАЙДЕР ФИЛЬТРУЕТ ТРАФИК: BLACK
│
├─ xHTTP + Reality
│
└─ BLACK / KEPLER
   ├─ Жёсткий DPI
   ├─ Ограниченные сети
   ├─ Фильтрация
   └─ Сложные условия
``` 

### Теги репозитория

<div align="center">

<img src="https://img.shields.io/badge/XRAY-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/REALITY-16A34A?style=flat-square" />
<img src="https://img.shields.io/badge/VLESS-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/XHTTP-DC2626?style=flat-square" />
<img src="https://img.shields.io/badge/DPI_BYPASS-F97316?style=flat-square" />
<img src="https://img.shields.io/badge/CAMOUFLAGE-7C3AED?style=flat-square" />
<img src="https://img.shields.io/badge/SING_BOX-0891B2?style=flat-square" />
<img src="https://img.shields.io/badge/FREE_INTERNET-16A34A?style=flat-square" />

</div> 
