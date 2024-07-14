Для запуска программы запустите через консоль файл `main.py`

Все необходимые пакеты программа установит самостоятельно при необходимости.
Если вы получили ошибку при попытке импортирования пакета, добавьте указанный ниже блок кода, указанный в сообщении об ошибке, в файл `init_pkg.py` в тело функции `init_packages`.

__Пример блока кода установки пакета `numpy`, если он не установлен__
```python
try:
    import numpy
except ImportError:
    subprocess.check_call([sys.executable, "-m", "pip", "install", "numpy"])
```

После работы программы вам нужно будет перейти в консоль по подсказке и посмотреть в ней результаты вычислений

Пример работы программы:
![](https://github.com/user-attachments/assets/6228d297-ec19-4092-8ae2-b002650fc134) <br />
![](https://github.com/user-attachments/assets/513fa117-20af-4c99-8f93-c77833229e8f)
