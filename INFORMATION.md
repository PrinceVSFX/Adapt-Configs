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

### Vless + Reality

**Что такое VLESS**

***VLESS*** *— современный прокси-протокол из экосистемы Xray, разработанный как более лёгкая и производительная альтернатива VMess. В отличие от VMess, VLESS не использует собственное шифрование трафика и полагается на TLS, что уменьшает количество распознаваемых сигнатур и делает соединение менее заметным для систем анализа трафика.*

**Что такое REALITY**

***REALITY*** *— технология маскировки в Xray, позволяющая устанавливать TLS-соединения без собственного сертификата и домена. Вместо этого соединение имитирует обращение к реальному популярному HTTPS-сайту.*

*Для стороннего наблюдателя трафик выглядит как обычное HTTPS-соединение, что значительно усложняет его обнаружение и фильтрацию.*

### Преимущества Vless + Reality 

- Высокая устойчивость к DPI (Deep Packet Inspection).
- Минимальное количество уникальных сигнатур.
- Отсутствие необходимости выпускать TLS-сертификаты.
- Маскировка под обычный HTTPS-трафик.
- Высокая производительность и низкие накладные расходы.
- Простая настройка по сравнению с классическими TLS-конфигурациями.

### Как это работает

```text
Client ➔ VLESS ➔ REALITY ➔ TCP ➔ Internet
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
