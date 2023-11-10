# Декодирование BMP изображений

Программа представляет собой текстовое (консольное) графическое приложение, реализованное на python 3.12

## Задание

- Реализовать ручное и автоматическое декодирование заголовков BMP изображений.
- Реализовать ручное и автоматическое разбиение BMP изображений на цветовые компоненты.
- Реализовать ручное и автоматическое разбиение на битовые срезы BMP изображений.

Для реализаций разбиений на цветовые компоненты и на битовые срезы 
использовать только изображения с 24 битовой палитрой (RGB).

Примечание: При ручном разбиении допускается использование битовых карт (bitmap)

## Разбиение на цветовые компоненты (Алгоритмы)

### Ручное разбиение

Ручное разбиение занимает достаточно много кода, он немного избыточен.

https://github.com/JKearnsl/BMPDecoding/blob/4a80955e825d245b03adbd5140e708d4d8e3015b/src/core/bmp.py#L152-L227

### Автоматическое разбиение (Pillow)

https://github.com/JKearnsl/BMPDecoding/blob/4a80955e825d245b03adbd5140e708d4d8e3015b/src/core/bmp.py#L229-L261

## Разбиение на битовые срезы

Битовые срезы представляют собой 8 частей одного изображения, лучший эффект виден на ч/б изображении. 
Для экспериментов рекомендую использовать [данное изображение](https://raw.githubusercontent.com/JKearnsl/BMPDecoding/master/examples/bmp-24-gray.bmp)

### Ручное разбиение

https://github.com/JKearnsl/BMPDecoding/blob/4a80955e825d245b03adbd5140e708d4d8e3015b/src/core/bmp.py#L263-L295

### Автоматическое разбиение (Pillow)

https://github.com/JKearnsl/BMPDecoding/blob/4a80955e825d245b03adbd5140e708d4d8e3015b/src/core/bmp.py#L298-L321

## Скриншоты работы программы


## Экземпляры изображений для теста

- Цветное 24 битное изображение [скачать](https://raw.githubusercontent.com/JKearnsl/BMPDecoding/master/examples/bmp_24.bmp)
- Ч/Б 24 битное изображение [скачать](https://raw.githubusercontent.com/JKearnsl/BMPDecoding/master/examples/bmp-24-gray.bmp)
