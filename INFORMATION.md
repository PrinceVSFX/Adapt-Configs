# ADAPT CONFIGS — INFORMATION

**Curated Xray subscription repository**  
Обход блокировок · DPI bypass · Transport camouflage · Xray инфраструктура

</br>

## Основные принципы

| Принцип | Описание |
|--------|----------|
| **Стабильность** | Работа без сбоев |
| **Bypass** | Обход любых ограничений |
| **Минимализм** | Только нужное |
| **Clean routing** | Предсказуемые маршруты |

---

## 📊 Сравнение профилей

| Характеристика | ⚪ WHITE / ALBEDO | ⚫ BLACK / KEPLER |
|---------------|------------------|-------------------|
| **Назначение** | Браузер, YouTube, Telegram, Discord, игры | Жёсткий DPI, provider filtering, нестабильные сети |
| **База** | Reality + Vision | xHTTP + REALITY |
| **Стабильность** | 5/5 | 4/5 |
| **Latency** | Низкий | Средний |
| **Overhead** | Низкий | Выше |
| **Camouflage** | Обычная | Усиленная (packet masking) |
| **Multiplex** | ❌ | ✅ XMUX |

## Стек технологий

**Security Layer**
`VLESS` · `REALITY` · `XTLS Vision` · `TLS Camouflage`

**Transport Layer**
`TCP` · `xHTTP` · `gRPC` · `WebSocket`

**Enhancement Layer**
`DPI Bypass` · `Packet-Up` · `XMUX` · `Padding`

## Сравнение транспортов

| Транспорт | Лучше всего для | Особенность |
|-----------|----------------|-------------|
| **TCP** | Стабильность | Классика |
| **xHTTP** | Advanced bypass | Современный, агрессивный |
| **gRPC** | Long sessions, multiplexing | Стабильный throughput |
| **WS** | CDN-совместимость | WebSocket |

</br>

## Маскировка (Camouflage)

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

## Архитектура REALITY

**Цепочка проксирования**

`Клиент` → `VLESS + REALITY` → `Фейковый TLS` → `Целевой сайт`

**Защитные механизмы**

- Browser fingerprinting (браузерное окружение)
- Реальный SNI (yandex.ru, RBC, CDN endpoints)
- Полная неотличимость от HTTPS

**Результат**

DPI не видит разницы ✅

</br>

## Требования совместимости

| Компонент | Необходимость |
|-----------|--------------|
| latest sing-box | ✅ Обязательно |
| latest xray-core | ✅ Обязательно |
| Reality support | ✅ Обязательно |
| xHTTP support | ✅ (для BLACK) |
| modern transports | ✅ |

### ⚠️ Предупреждение
> Старые клиенты могут не поддерживать Reality, xHTTP, XTLS Vision.

## 📈 Диаграмма выбора профиля
                НУЖЕН ЛИ ВАМ?
                      │
        ┌─────────────┴─────────────┐
        ↓                           ↓
  Стабильность                Жёсткий обход
  и низкий ping               (провайдер блокирует)
        │                           │
        ↓                           ↓
  ⚪ WHITE                      ⚫ BLACK
(Reality+Vision)            (xHTTP+REALITY)
        │                           │
        ↓                           ↓
YouTube, Discord,           Нестабильные сети,
Telegram, игры               агрессивный DPI

---

## 🏷️ Теги репозитория

`#Xray` `#Reality` `#VLESS` `#xHTTP` `#DPIBypass` `#Camouflage` `#SingBox` `#FreeInternet`

---

> 👑 **PRINCEVSFX / FREE WEB RING**
