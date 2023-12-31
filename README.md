# Учебный проект по компьютерному зрению
Представлено в проекте обучение модели глубокого обучения на датасете CIFAR-10, который содержит изображения различных объектов, разделенных на 10 классов. Здесь представлена модель нейронной сети ResidualNet, которая реализует сверточную нейронную сеть с использованием блоков ResNet. В проекте также представлен класс Trainer, который отвечает за обучение и тестирование модели.

Для быстрой проверки можно запускать в Jupyter notebook либо в Google Collabs.
Перед запуском изменить путь к папке датасетов на свой при необходимости '..datasets'. 
Данные загрузятся автоматически при запуске.

Что понадобится:

1. Установка PyTorch
 
!pip install torch torchvision

2. Установка Numpy

!pip install numpy
 
3. Установка Matplotlib

!pip install matplotlib

Последний блок кода с аугментацией(изменение тестовых данных) выполняем его и изменённые данные, после чего можем потворить обучение для повышения точности.
По всем вопросам https://t.me/Apexi8

Краткое описание основных компонент проекта:

  1.  Загрузка данных: В проекте используется датасет CIFAR-10, который загружается с использованием библиотеки torchvision. Датасет содержит обучающую и тестовую выборки с изображениями и соответствующими метками классов (10 классов).

   2. Модель нейронной сети: Вы определили модель ResidualNet, которая представляет собой сверточную нейронную сеть с использованием блоков ResNet. Эта модель используется для классификации изображений на 10 классов.

   3. Обучение модели: Для обучения модели используется класс Trainer, который содержит методы для обучения и тестирования модели. Во время обучения используется оптимизатор SGD и функция потерь CrossEntropyLoss.

   4. Тестирование модели: После обучения модели, она тестируется на тестовой выборке для оценки ее точности.

   5. Визуализация процесса обучения: В конце проекта представлена функция plot_train_log, которая отображает графики обучения модели.

   6. Аугментация данных: Проект также включает преобразование данных с помощью transforms.Compose, чтобы добавить аугментацию данных (RandomVerticalFlip) к обучающей выборке.

   7. Вывод точности: В проекте также представлен код для вычисления и вывода точности модели для каждого класса из CIFAR-10.
