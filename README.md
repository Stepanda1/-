# Анализ доходности и волатильности криптовалют

Итоговый проект по дисциплине **«Анализ данных на Python»**

**Авторы:** Козлов Степан, Шембек Александр
**Источник данных:** CoinGecko API  
**Объекты анализа:** BTC, ETH, BNB, SOL, XRP, DOGE, ADA и TRX

[Открыть основной ноутбук](./crypto_analysis.ipynb)

## Цель проекта

Сравнить доходность и риск восьми популярных криптовалют за 365 дней, изучить взаимосвязи между их дневными доходностями.

## Запуск проекта

### 1. Клонирование

```bash
git clone https://github.com/Stepanda1/Analyze-profitability-and-volatility-crypto.git
cd Analyze-profitability-and-volatility-crypto
```

### 2. Виртуальное окружение

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

Linux/macOS:

```bash
source .venv/bin/activate
```

### 3. Установка зависимостей

```bash
pip install -r requirements.txt
```

### 4. Настройка CoinGecko API

Создайте файл `.env` по образцу `.env.example`:

```text
COINGECKO_API_KEY=your_api_key_here
```

### 5. Запуск ноутбука

```bash
jupyter notebook crypto_analysis.ipynb
```

Без API-ключа ноутбук может использовать локальный файл `raw_crypto_data.csv`, расположенный рядом с ним.

Обязательные столбцы локального файла:

```text
date,symbol,coin_id,price,market_cap,total_volume
```