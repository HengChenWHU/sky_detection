# sky_detection
Raw sky region detection algorithm

Основные черты небесной области на изображении:
1) Голубой или около того цвет
2) Расположение в верхней части изображения
3) Однородность (smoooooooooth)

Решено использовать вероятностный подход - чем лучше пиксель удовлетворяет вышеуказанным трем признакам, тем больше вероятность что он принадлежит небу. Таким образом строятся вероятностные карты каждого из этих признаков, которые затем совмещаются и по определеному порогу разделяются на небо и не небо.
Построение карты однородности сильно нуждается в доработке.
Прилагается пример хорошей работы алгоритма.
