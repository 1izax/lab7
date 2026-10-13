# lab7
```
#include <stdio.h>
#include <locale.h>

int goodhour()
{
    setlocale(LC_CTYPE, "RUS");
    int hour;

    printf("===== ПРИВЕТСТВИЕ ПО ВРЕМЕНИ СУТОК =====\n");
    printf("Введите час (число от 0 до 23): ");
    scanf("%d", &hour);
    printf("----------------------------------------\n");
    printf("Ваше время: %d ч.\n", hour);

    switch (hour)
    {
    case 0:
    case 1:
    case 2:
    case 3:
    case 4:
    case 5:
        printf("Спокойной ночи!\n");
        break;
    case 6:
    case 7:
    case 8:
    case 9:
    case 10:
    case 11:
        printf("Доброго утра!\n");
        break;
    case 12:
    case 13:
    case 14:
    case 15:
    case 16:
    case 17:
        printf("Доброго дня!\n");
        break;
    case 18:
    case 19:
    case 20:
    case 21:
    case 22:
    case 23:
        printf("Доброго вечера!\n");
        break;
    default:
        printf("Ошибка! Час должен быть от 0 до 23.\n");
        break;
    }
    printf("----------------------------------------\n");
}

int main()
{
    goodhour();
    getchar();
    return 0;
}
```
