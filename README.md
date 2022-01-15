# ML crash course

## План курса

* Лекция 1: Введение в Machine Learning



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