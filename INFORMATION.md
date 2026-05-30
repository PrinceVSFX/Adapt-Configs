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

```txt
Безопасность 
├─ VLESS
├─ REALITY
├─ XTLS Vision
└─ TLS Camouflage

Транспорт
├─ TCP
├─ xHTTP
├─ gRPC
└─ WebSocket

Оптимизация
├─ DPI Bypass
├─ Packet-Up
├─ XMUX
└─ Padding
```

### Сравнение транспортов

| Транспорт | Лучше всего для | Особенность |
|-----------|----------------|-------------|
| **TCP** | Стабильность | Классика |
| **xHTTP** | Advanced bypass | Современный, агрессивный |
| **gRPC** | Long sessions, multiplexing | Стабильный throughput |
| **WS** | CDN-совместимость | WebSocket |

</br>

### Маскировка (Camouflage)

Используемые домены для имитации обычного HTTPS/CDN-трафика:

| Домен | Тип |
|-------|-----|
| Yandex | Поисковик |
| mwscdn | CDN |
| RBC | СМИ |
| Beget | Хостинг |
| storage.yandex | Облако |
| CDN endpoints | Сеть доставки |

**Результат:** трафик выглядит как обычный HTTPS/CDN.

### Архитектура REALITY

**Цепочка проксирования**

`Клиент` → `VLESS + REALITY` → `Фейковый TLS` → `Целевой сайт`

**Защитные механизмы**

- Browser fingerprinting (браузерное окружение)
- Реальный SNI (yandex.ru, RBC, CDN endpoints)
- Полная неотличимость от HTTPS

**Результат**

DPI не видит разницы ✅

### Диаграмма выбора профиля

| Ваша ситуация | → | Профиль | → | Идеально для |
|:---|:---:|:---|:---:|:---|
| Нужна стабильность и низкий ping | → | **WHITE**<br>`Reality + Vision` | → | YouTube, Discord, Telegram, игры |
| Провайдер жестко блокирует | → | **BLACK**<br>`xHTTP + REALITY` | → | Нестабильные сети, агрессивный DPI | 

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
