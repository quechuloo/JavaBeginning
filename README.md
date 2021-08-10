# Отчёт о тестировании **IntelliJ IDEA**

## Проверить работу программы с разными тестовыми данными

09/08/2021 - 10/08/2021 было проведено 11 тестирований в приложении *Intellij IDEA*.

На тестирование затрачено: 10 часов

В результате тестирования выявлены следующие дефекты:
* [Карты вида American Express (AMEX), не проходят валидацию](https://github.com/quechuloo/JavaBeginning/issues/1)




## В процессе тестирования использовались следующие артефакты:
* Test Plan
1. Тестируем функциональность валидации номера банковской карты.
2. Тестируем в IntelliJ IDEA
3. Тестирование будем проводить с 09/08/2021 - 10/08/2021
4. Для тестирования будем использовать код оставшийся от нашего программиста
5. Проверим самые популярные виды банковских карт на корректную валидацию



## В качестве тестовых данных использовались данные с сайта freeformatter.com:
* VISA: 4662477486320345 - Result is OK Process finished with exit code 0
* VISA: 4485570925564831 - Result is OK Process finished with exit code 0
* MasterCard: 2221003788932963 - Result is OK Process finished with exit code 0
* MasterCard: 2720995656779184 - Result is OK Process finished with exit code 0
* MasterCard: 5329558034616995 - Result is OK Process finished with exit code 0
* American Express (AMEX): 370772351271487 - *ОР* Result is OK Process finished with exit code 0 / *ФР* Result is FAIL Process finished with exit code 0
* American Express (AMEX): 372705148769569 - *ОР* Result is OK Process finished with exit code 0 / *ФР* Result is FAIL Process finished with exit code 0
* American Express (AMEX): 372208725885403 - *ОР* Result is OK Process finished with exit code 0 / *ФР* Result is FAIL Process finished with exit code 0
* Maestro: 6759236479813974 - Result is OK Process finished with exit code 0
* Maestro: 6304372174799919 - Result is OK Process finished with exit code 0
* Maestro: 6763816857798170 - Result is OK Process finished with exit code 0

## Тестирование производилось в следующем окружении:
* Windows 10 Home 64 bits
* openjdk version "11.0.11" 2021-04-20
OpenJDK Runtime Environment AdoptOpenJDK-11.0.11+9 (build 11.0.11+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK-11.0.11+9 (build 11.0.11+9, mixed mode)
