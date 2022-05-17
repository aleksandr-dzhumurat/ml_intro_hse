# ML crash course

## План курса

* Лекция 1: Введение в Machine Learning
    * [slides](https://docs.google.com/presentation/d/17lCrDPFqPzrxco9NOdgBCx_1ewLJ7iQ9/edit#slide=id.p1)
    * [видео](https://youtu.be/_BSlnZzlng4)
    * [lecture notes](./lecture_notes/ml_intro.md)
    * [notebook](./jupyter_notebooks/Part_01_ML_intro.ipynb)
    
* Лекция 2. Градиентное обучение
    * [slides]()
    * [видео]()
    * [lecture notes](./lecture_notes/gradient_descent.md)
    * [notebook](./jupyter_notebooks/Part_02_gradient_descent.ipynb)
    
* Лекция 3. Классификация, линейные модели
    * [slides](https://docs.google.com/presentation/d/1P6BGXL1RF4ehTRXCs7zU2jLkIOLfagRk/edit?usp=sharing&ouid=116356322827696809637&rtpof=true&sd=true)
    * [видео](https://youtu.be/-FDok30act0)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_03_validation_generalization_ability_overfitting.ipynb)
    
* Лекция 4. Классификация, линейные модели
    * [slides](https://docs.google.com/presentation/d/1jiV8xDS-26Vit6eMbzAXmvgd2tSeyh3P/edit?usp=sharing&ouid=116356322827696809637&rtpof=true&sd=true)
    * [видео](https://youtu.be/-FDok30act0)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_04_classification.ipynb)
    
* Лекция 5. Деревянные модели: случайный лес и градиентный бустинг
    * [slides](https://docs.google.com/presentation/d/11uOvlnIs4PhTnXRq7MWs-zFRoGLqW9bB/edit#slide=id.g111d491c0c7_0_11)
    * [видео](https://youtu.be/Q2h7CkvZXIo)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_05_Trees_Boosting.ipynb)
    
* Лекция 6. Пример ML проекта: классификация кликбейта
    * [slides]()
    * [видео](https://youtu.be/EaQQ83YNH24)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_06_ML_project_example.ipynb)
    
* Лекция 7. Обучение без учителя: кластеризация, снижение размерности
    * [slides]()
    * [видео](https://youtu.be/Q8zOYacXLXI)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_07_feature_engineering.ipynb)
    
* Лекция 8. Neural Networks
    * [slides]()
    * [видео](https://youtu.be/tOSAjblsCtc)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_08_neural_networks.ipynb)
    
* Лекция 9. Feature Engineering
    * [slides]()
    * [видео](https://youtu.be/kYibLwNYYU0)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_9_feature_engineering.ipynb)
    
* Лекция 10. Приложения ML: рекомендательные системы
    * [slides]()
    * [видео](https://youtu.be/n2Dx0-1Xw_M)
    * [lecture notes](./lecture_notes/)
    * [notebook](./jupyter_notebooks/Part_10_recommeder_systems.ipynb)


## Подготовка к работе

Предпочтительный способ - работа в [Google Colab](https://colab.research.google.com/)

Либо можно  запустить Jupyter на локальной машине - [тут, например, инструкция для windows](https://medium.com/@neuralnets/beginners-quick-guide-for-handling-issues-launching-jupyter-notebook-for-python-using-anaconda-8be3d57a209b)

### Mac

Для локального запуска нужно добавить системные пакеты (иначе некорректно соберётся python-окружение)
```shell
brew install openssl xz gdbm
```

Затем создаём виртуальное окружение

```shell
pyenv install 3.8.10 && \
pyenv virtualenv 3.8.10 hse-env
```

Далее активируем окружение
```shell
source ~/.pyenv/versions/hse-env/bin/activate
```

После активации устанавлеваем зависимости
```shell
pip install -r requirements.txt
```

И заускаем jupyter - в командной строке появится ссылка вида `http://127.0.0.1:8888/?token=123` - её нужно открыть в браузере
```shell
jupyter notebook jupyter_notebooks --ip 0.0.0.0 --port 8888 --allow-root --no-browser
```