# Лабы за 7 семестр ПМИ МАИ по Методам, средствам и технологииям мультимедиа

(по факту это искусственный интеллект и анализ данных)

### **Выполнил Лохматов Никита Игоревич, М8О-406Б-21**

### Структура

- В директории `datasets` лежат два датасета: `shelter_animal_outcomes.csv` для задачи классификации и `kc_house_data.csv` для задачи регрессии

- В директориях `lab1`, `lab2`, `lab3`, `lab4` и `lab5` лежат соответственные ЛР по отдельности

- В файле `labs1-5.ipynb` лежит сборник всех ЛР, итоговая таблица с результатами и выводы

### Таблица с результатами

| Алгоритм              | Задача          | Бейзлайн                                                                 | Улучшенный бейзлайн                                                   | Самостоятельная имплементация                                       | Улучшенная самостоятельная имплементация                            |
|------------------------|-----------------|-------------------------------------------------------------------------|----------------------------------------------------------------------|----------------------------------------------------------------------|----------------------------------------------------------------------|
| **KNN**               | Классификация  | accuracy: 0.7180 <br> f1: 0.6582 <br> recall: 0.6622 <br> precision: 0.6542 | accuracy: 0.6770 <br> f1: 0.5193 <br> recall: 0.4256 <br> precision: 0.6660 | accuracy: 0.7320 <br> f1: 0.6736 <br> recall: 0.6744 <br> precision: 0.6727 | accuracy: 0.6795 <br> f1: 0.6016 <br> recall: 0.5902 <br> precision: 0.6134 |
|                        | Регрессия      | mae: 165296.01 <br> rmse: 273167.61 <br> r²: 0.4968                     | mae: 145297.89 <br> rmse: 230201.78 <br> r²: 0.6427                   | mae: 143717.60 <br> rmse: 228580.44 <br> r²: 0.6477                   | mae: 145279.43 <br> rmse: 230197.34 <br> r²: 0.6427                   |
| **Линейные модели**    | Классификация  | accuracy: 0.7625 <br> f1: 0.6953 <br> recall: 0.6610 <br> precision: 0.7334 | accuracy: 0.7338 <br> f1: 0.6635 <br> recall: 0.6422 <br> precision: 0.6863 | accuracy: 0.7060 <br> f1: 0.4674 <br> recall: 0.3146 <br> precision: 0.9085 | accuracy: 0.7570 <br> f1: 0.6920 <br> recall: 0.6659 <br> precision: 0.7203 |
|                        | Регрессия      | mae: 142010.83 <br> rmse: 226649.05 <br> r²: 0.6536                     | mae: 141519.59 <br> rmse: 226630.27 <br> r²: 0.6537                   | mae: 141883.26 <br> rmse: 226499.03 <br> r²: 0.6541                   | mae: 141884.33 <br> rmse: 226502.94 <br> r²: 0.6540                   |
| **Решающее дерево**    | Классификация  | accuracy: 0.7305 <br> f1: 0.6707 <br> recall: 0.6695 <br> precision: 0.6720 | accuracy: 0.7500 <br> f1: 0.6484 <br> recall: 0.5622 <br> precision: 0.7658 | accuracy: 0.7100 <br> f1: 0.4775 <br> recall: 0.3232 <br> precision: 0.9138 | accuracy: 0.7500 <br> f1: 0.6474 <br> recall: 0.5598 <br> precision: 0.7676 |
|                        | Регрессия      | mae: 165621.36 <br> rmse: 270434.98 <br> r²: 0.5068                     | mae: 144253.57 <br> rmse: 224019.85 <br> r²: 0.6616                   | mae: 221864.00 <br> rmse: 362256.06 <br> r²: 0.1151                   | mae: 221864.00 <br> rmse: 362256.06 <br> r²: 0.1151                   |
| **Случайный лес**      | Классификация  | accuracy: 0.7525 <br> f1: 0.6904 <br> recall: 0.6732 <br> precision: 0.7086 | accuracy: 0.7630 <br> f1: 0.6989 <br> recall: 0.6707 <br> precision: 0.7294 | accuracy: 0.7240 <br> f1: 0.6546 <br> recall: 0.6378 <br> precision: 0.6722 | accuracy: 0.7235 <br> f1: 0.6576 <br> recall: 0.6476 <br> precision: 0.6679 |
|                        | Регрессия      | mae: 125980.82 <br> rmse: 197415.05 <br> r²: 0.7372                     | mae: 125162.05 <br> rmse: 193739.07 <br> r²: 0.7469                   | mae: 171256.58 <br> rmse: 280589.84 <br> r²: 0.4691                   | mae: 146040.42 <br> rmse: 250307.33 <br> r²: 0.5775                   |
| **Градиентный бустинг**| Классификация  | accuracy: 0.7590 <br> f1: 0.6596 <br> recall: 0.5695 <br> precision: 0.7836 | accuracy: 0.7685 <br> f1: 0.7068 <br> recall: 0.6805 <br> precision: 0.7352 | accuracy: 0.7550 <br> f1: 0.6418 <br> recall: 0.5354 <br> precision: 0.8011 | accuracy: 0.7715 <br> f1: 0.7102 <br> recall: 0.6829 <br> precision: 0.7398 |
|                        | Регрессия      | mae: 125246.45 <br> rmse: 195061.07 <br> r²: 0.7434                     | mae: 125143.45 <br> rmse: 197023.59 <br> r²: 0.7382                   | mae: 125250.42 <br> rmse: 194972.52 <br> r²: 0.7437                   | mae: 125040.79 <br> rmse: 195862.95 <br> r²: 0.7413                   |
