
# CryptoFolio

Этот проект позволяет отслеживать ваши криптовалютные активы в реальном времени. Вы можете добавлять монеты, указывать их количество и видеть:

 - Текущую цену (через WebSocket Binance)
 - Общую стоимость (количество × цена)
 - Изменение цены за 24 часа (+/- в $ и %)
 - Долю в портфеле (% от общей стоимости)

# Основные функции

1. Добавление и удаление токенов

- В модальном окне (ModalWindow) можно указать количество для каждой монеты.

- Данные сохраняются в localStorage и не пропадают после перезагрузки.

- Чтобы удалить токен, кликните на строку в таблице.

2. Отслеживание цен в реальном времени

- Подключение к Binance WebSocket API (wss://stream.binance.com).

- Отображение:

        - Текущей цены (trade)

        - Изменения за 24ч (ticker)

3. Расчет доли в портфеле

Функция calculatePortfolioPercentage() вычисляет, какой процент от общего портфеля занимает каждый токен.

# Технологии

- React (хуки useState, useEffect)

- WebSocket (реал-тайм данные с Binance)

- LocalStorage (сохранение токенов)

- CSS-модули (стилизация таблицы и модалки)

# Как запустить?

1. Установите зависимости:
```bash
npm install
```
2. Запустите проект:
```bash
npm run dev
```

# Скриншоты
![Vite-React-TS](https://github.com/user-attachments/assets/71201f3a-39c4-4a80-86c2-7069fd48d3be)
![Vite-React-TS2](https://github.com/user-attachments/assets/4fe71180-ef47-439c-a756-70a531ffa94c)
![Vite-React-TS3](https://github.com/user-attachments/assets/bf6b339a-4ad6-4922-bd22-abb6d96bd90e)
![Vite-React-TS4](https://github.com/user-attachments/assets/25a1ddbb-8882-477e-a515-909306994390)
