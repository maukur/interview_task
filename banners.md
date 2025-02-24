## Задача: Рандомизация баннеров с учетом веса

У нас есть список баннеров, где каждый баннер имеет уникальный идентификатор и вес. Вес баннера указывает на его вероятность выпадения — чем выше вес, тем чаще баннер должен показываться. Требуется реализовать функцию, которая будет случайно возвращать баннеры с учетом их весов.

### Формат данных
```swift
struct Banner {
    let id: Int
    let weight: Double
}


let banners = [
    Banner(id: 1, weight: 5.0),
    Banner(id: 2, weight: 1.0),
    Banner(id: 3, weight: 4.0)
]
```

### Требования
1. Реализовать функцию func getRandomBanner(from banners: [Banner]) -> Banner?, которая возвращает случайный баннер с учетом его веса.
2. Функция должна корректно работать при любом количестве баннеров и любых весях.
3. Если список баннеров пустой, функция должна возвращать nil.

### Пример работы
При запуске функции getRandomBanner с указанным выше массивом, баннер с id = 1 должен выпадать примерно в 50% случаев, баннер с id = 2 — в 10%, и баннер с id = 3 — в 40%.

### Уточнения
- Ожидается, что функция использует эффективный алгоритм, который работает с минимальными затратами по времени и памяти.
- Желательно, чтобы функция была хорошо протестирована на различных наборах данных.
