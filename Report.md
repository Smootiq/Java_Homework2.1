# Отчёт о тестировании приложения "Tested"

## Краткое описание
Проведено тестирование на ПО IntelliJ IDEA Community, для выявления причины сбоя пополнения счёта VIP-клиента. 

## Описание тестов
На ПО IntelliJ IDEA Community, было создано базовое приложение, для анализа возможных вариантов произошедшей ситуации.
> <i> public class Main { <br>
    public static void main(String[] args) { <br>
        int bank = 2_000_000_000; <br>
        int payment = 500_000_000; <br>
        int total = bank + payment; <br>
        System.out.println(total);  <br>
    } <br>
} </i> <br>

Проводилось позитивное тестирование функционала зачисления денежных средств, с учётом переменной типа "int total".

## Результаты

1. 0% успешных тестов
2. По итогу операции баланс составляет: -1_794_967_296
3. Баланс должен составлять: 2_500_000_000
4. Issues: https://github.com/Smootiq/Java_Homework2.1/issues/1

## Общие рекомендации

Исправить команду вывода сообщений в консоль
> System.out.println(total);  <br>