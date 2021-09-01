# module_8
 Проект 7. Ford vs Ferrari: определяем модель авто по фото 
 
В данном проекте осуществлялось написание нейросети с целью предсказания модели автомобиля по фотографии. Были использованы следующие приемы:
 - Аугментация данных с использованием библиотек Albumentations и ImageDataAugmentor, для предпросмотра которых был использован ресурс https://albumentations-demo.herokuapp.com/;
 - transfer learning использованием различных архитектур (Xception, EfficientNetB3);
 - произведен fine-tuning обучаемых моделей;
 - использован инструмент контроля LR в виде ExponentialDecay;
 - в качестве функции потерь была использована стандартная для классификации с множеством классов CategoricalCrossentropy;
 - использован прием Test Time Augmentation;

Лучшая оценка accuracy, полученная для первой версии, построенной на Xception - 0.9494

Для второй, построенной на EfficientNetB3 - 0.9587

Личные впечатления:
К сожалению, выделил на написание этого проекта крайне мало времени - лишь последнюю неделю, выделенную в расписании. С учетом того, что часть этой недели я использовать не смог, написание проекта получилось очень поспешным. Поскольку впервые работал с написанием нейросети, сильно недооценил время, которое требуется на ее обучение (счел, что раз мы только учимся, то сети у нас просты и быстро учатся. Как я был неправ...). 
Было очень непривычно проверять гипотезы, поскольку по одному лишь первому слою и его результатам сложно однозначно сказать, насколько будет удачна вся сеть целиком, а полное обучение весьма длительно. 
Первым делом принялся за аугментацию данных (счел, что входные данные нужно улучшать в первую очередь), что было не так уж и бесполезно, но все же fine-tuning, как показалось, принес куда более значительные результаты. 
Поначалу сильно распылился, вознамерившись реализовать несколько видов архитектур (ResNet, EfficientNet, Xception), что заняло немало времени, которое можно было потратить на улучшение работы какой-то одной. В перспективе это кажется более мудрым решением. 
В процессе работы подвел Colab - не дал включить GPU, поскольку закончилось время использования, пришлось тратить время и переносить все в Kaggle ноутбук. 
Не смог провести дообучение на изображениях более высокого разрешения, поскольку до дедлайна мне бы не хватило времени (хотя времени использования GPU , выделенного на эту неделю, мне бы хватило).

В целом, работать над написанием своей первой нейросети мне понравилось и работу эту я выполнял с удовольствием, но следовало подойти к вопросу более обстоятельно и выделить больше времени. Думаю, если бы смог хотя бы всю неделю (не говоря уже о большем), а не 4 дня, то добился бы куда лучших результатов. Но энтузиазм, к сожалению, не заменит приложенные время и усилия.

Спасибо за проверку, с уважением - Кобелев Алексей
