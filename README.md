Установка

1. Установить Node.js LTS https://nodejs.org/en/
2. Установить и синхронизировать parity https://www.parity.io/. Чтобы смотреть прогресс синхронизации поставить это https://github.com/parity-js/shell/releases/tag/v0.1.4/
3. Разархивировать архив и открыть терминал в этой папке
4. Ввести в терминал
```npm i```

5. Через текстовый редактор изменить input.json подставив туда актуальные данные времени, адресов, приватного ключа и стоимости газа. Газ вводится в единицах измерения gwei, как в метамаске.

6. Ввести в терминале
```npm start```

```privateKey``` - приватный ключ.<br />
```addressFrom``` - адрес с которого отправляются средства.<br />
```addressTo``` - адрес куда отправляются средства.<br />
```startGasPrice``` - цена газа с которой отправится первая транзакция когда сработает таймер.<br />
```maxGasPrice``` - максимальная цена газа.<br />
```gasLimit``` - газ лимит.<br />
```Increment``` - на сколько будет повышаться цена газа если в пул попадет транзакция с бОльшей ценой газа.<br />
```Value``` - объем средств в эфире.<br />
```startDate``` - время срабатывания таймера, не надо писать ноль перед другой цифрой, то есть если надо отправить в 9:05 то писать надо hour: 9, minute:5.<br />

Можно тестить отправляя транзакции на один адрес с разных нод(с другого клиента parity, metamask, mew).