<div align="center">

<img src="Materials/png/information.png" alt="ADAPT-CONFIGS" width="1920">

</div>

<table width="1920" style="background: #0d1117; border: 1px solid #30363d; border-radius: 16px;">
  <tr>
    <td align="center" style="padding: 32px 20px;">
      <strong style="font-size: 24px; color: #ffffff;">Curated Xray subscription repository</strong><br>
      <span style="font-size: 16px; color: #8b949e;">Обход блокировок · DPI bypass · Transport camouflage · Xray инфраструктура</span>
    </td>
  </tr>
</table> 

</br>

### Основные принципы

|	|	|
|---|---|
| **Стабильность**<br>Работа без сбоев | **Bypass**<br>Обход любых ограничений |
| **Минимализм**<br>Только нужное | **Clean routing**<br>Предсказуемые маршруты |

### Сравнение профилей

| Характеристика | WHITE / ALBEDO | BLACK / KEPLER |
|---------------|------------------|-------------------|
| **Назначение** | Браузер, YouTube, Telegram, Discord, игры | Жёсткий DPI, provider filtering, нестабильные сети |
| **База** | `Reality + Vision` | `xHTTP + REALITY` |
| **Стабильность** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Latency** | Низкий | Средний |
| **Overhead** | Низкий | Выше |
| **Camouflage** | Обычная | Усиленная (packet masking) |
| **Multiplex** | ❌ | XMUX |

### Стек технологий

**Security Layer**
`VLESS` · `REALITY` · `XTLS Vision` · `TLS Camouflage`

**Transport Layer**
`TCP` · `xHTTP` · `gRPC` · `WebSocket`

**Enhancement Layer**
`DPI Bypass` · `Packet-Up` · `XMUX` · `Padding`

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

### Требования совместимости

| Компонент | Необходимость |
|-----------|--------------|
| latest sing-box | ✅ Обязательно |
| latest xray-core | ✅ Обязательно |
| Reality support | ✅ Обязательно |
| xHTTP support | ✅ (для BLACK) |
| modern transports | ✅ |

### Диаграмма выбора профиля

| Ваша ситуация | → | Профиль | → | Идеально для |
|:---|:---:|:---|:---:|:---|
| 🟢 Нужна стабильность и низкий ping | → | ⚪ **WHITE**<br>`Reality + Vision` | → | YouTube, Discord, Telegram, игры |
| 🔴 Провайдер жестко блокирует | → | ⚫ **BLACK**<br>`xHTTP + REALITY` | → | Нестабильные сети, агрессивный DPI | 

### Теги репозитория

`#Xray` `#Reality` `#VLESS` `#xHTTP` `#DPIBypass` `#Camouflage` `#SingBox` `#FreeInternet`

---

> **PRINCEVSFX / FREE WEB RING**
