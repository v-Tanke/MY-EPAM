# LAB-3. Introduction to Testing
+++++++++++

### Test cases for [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785)

| Number |                             Task                             |                          Condition                           |                           Actions                            |                       Expected result                        |
| :----: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|   1    |                     Поиск котировки BMW                      | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785) | Развернуть окно котировок, ввести в поиск BMW(bmw), выбрать нужный вариант | В окно подгрузится нужный график, название котировки над графиком поменяется на BMW |
|   2    |         Осуществить сделку SELL для котировки EURUSD         | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку EURUSD, выбрать объем, дальше выбрать функцию SELL | В поле открытые ордера подгрузится информация по текущему ордеру, в столбце доходность должно динамически указываться прибыль или убыль в данный момент |
|   3    |                   Закончить открытый ордер                   | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь открытый ордер | Из списка открытых ордеров выбрать ток которы нужно закончить, нажать на крестик в столбце Close | Закрытый ордер должен удалиться из списка Открытые ордера, должен правильно сформироваться Баланс счета, данный ордер должен появится в таблице Закрытые ордера |
|   4    |               Использовать функцию Take Profit               | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать объем, дальше выбрать функцию Sell/Buy, поставить галочку T/P, выбрать коэффициент | Когда прибыль достигнет значения состовляющего коэффициент от лота, ордер автоматически закроется |
|   5    |                Использовать функцию Stop Loss                | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать объем, дальше выбрать функцию Sell/Buy, поставить галочку S/L, выбрать коэффициент | Когда убыль достигнет значения состовляющего коэффициент от лота, ордер автоматически закроется |
|   6    |          Открыть ордер на сумму превышающую баланс           | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать объем так чтоб желаемый ордер превысил баланс, дальше выбрать функцию Sell/Buy | При попытке осуществить данный ордер должна появится ошибка уведомляющая о недостаточности баланса для данного ордера |
|   7    |               Открыть ордер с нулевым объемом                | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать нулевой объем, дальше выбрать функцию Sell/Buy | При попытке осуществить данный ордер должна появится ошибка уведомляющая о том что нельзя открыть ордер с таким объемом |
|   8    |    Сделать Take Profit при Sell больше чем стоимость лота    | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать T/P так чтобы оно было больше стоимости лота, дальше выбрать функцию Sell | При попытке осуществить данный ордер должна появится ошибка уведомляющая о том что Take Profit не можеть быть больше стоимости лота |
|   9    |          Сделать Stop Loss больше чем объем ордера           | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать S/L так чтобы оно было больше объема лота,  дальше выбрать функцию Sell/Buy | При попытке осуществить данный ордер должна появится ошибка уведомляющая о том что Stop Loss не можеть быть больше объема лота |
|   10   | Попробовать сделать ордер с отрицательным значением Take Profit | Авторизоваться на сайте [Grand Capital](https://ru.grandcapital.net/my/webtrader_classic/109431785), иметь минимальный баланс | Выбрать котировку, выбрать объем, дальше выбрать функцию Sell/Buy, поставить галочку T/P, выбрать отрицательный коэффициент | При попытке осуществить данный ордер должна появится ошибка уведомляющая о том что что значение T/P должно быть больше 0 |

