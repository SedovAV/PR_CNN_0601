# PR_CNN_0601

### Пример 1. Ручное вычисление свёртки

#### Дано. Вход X (5×5), ядро K(3×3), stride = 1, padding = 0. 

<img width="414" height="134" alt="image" src="https://github.com/user-attachments/assets/63bfc58a-7681-4ca2-8066-bf40d767b9a1" />

Найти: карту признаков Y (размер и все значения).

<img width="678" height="609" alt="image" src="https://github.com/user-attachments/assets/808b7a2b-23de-4ddd-afed-56908fa76138" />

Вывод для обсуждения: ядро — детектор вертикальных границ (разность «левый столбец − правый столбец»). Отрицательные значения = переход «светлое→тёмное» слева направо. Именно поэтому после свёртки ставят ReLU/модуль.

### Пример 2. Размерности и число параметров

<img width="781" height="411" alt="image" src="https://github.com/user-attachments/assets/eb2c47bd-198a-4e23-a660-c06119a534e8" />

### Пример 3. Max-pooling

<img width="498" height="206" alt="image" src="https://github.com/user-attachments/assets/5c990133-5d51-440f-a04e-ab5aae1ea2a0" />

<img width="732" height="405" alt="image" src="https://github.com/user-attachments/assets/136d4f1a-6df6-49a0-b847-ed4db40c6880" />

### Задание 1. Реализация свёртки на NumPy

<img width="735" height="544" alt="image" src="https://github.com/user-attachments/assets/498d98f2-e4a2-4b69-b7d5-a58d1af449a5" />
<img width="738" height="336" alt="image" src="https://github.com/user-attachments/assets/6e646001-42c3-49a0-81ba-3b35bde65c4b" />

<img width="572" height="168" alt="image" src="https://github.com/user-attachments/assets/c6e7a7ca-59b9-4ec6-9d29-14ba8c31792e" />

Проверка через PyTorch (эталон):

<img width="735" height="87" alt="image" src="https://github.com/user-attachments/assets/af91ec2b-0146-4288-a3d4-33376e3ac92e" />

<img width="762" height="45" alt="image" src="https://github.com/user-attachments/assets/1a192b26-b8c8-41ad-bc8f-b783629b9707" />

### Задание 5. Обучение CNN в PyTorch

Задача: собрать CNN по архитектуре из задания 2 (но с FC-головой), обучить на MNIST, получить accuracy ≥ 98% за 3 эпохи.

Решение

<img width="744" height="449" alt="image" src="https://github.com/user-attachments/assets/6e86f037-62b5-43b8-9d4d-2efd8acb13c5" />
<img width="745" height="536" alt="image" src="https://github.com/user-attachments/assets/f1649e02-859b-4801-99fe-7fe4170f1b4b" />
<img width="750" height="295" alt="image" src="https://github.com/user-attachments/assets/b2b6a802-b349-4da2-bc73-ad64bad4947e" />

<img width="578" height="175" alt="image" src="https://github.com/user-attachments/assets/15531212-9e5d-4f24-9a9c-87a5d61ea93f" />

<img width="769" height="395" alt="image" src="https://github.com/user-attachments/assets/e0f623fd-ed3f-4c44-90e3-d17600afbc3a" />

