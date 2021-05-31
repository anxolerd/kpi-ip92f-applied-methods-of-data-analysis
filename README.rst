==============================
Прикладні методи аналізу даних
==============================

Виконав
=======

Аспірант групи ІП-92ф Ковальчук Олександр Миронович

Запуск
======

1. Створити та активувати віртуальне оточення Python

   .. code:: console

      $ python3 -m venv .venv
      $ . ./.venv/bin/activate

2. Встановити залежності

   .. code:: console

      (.venv) $ pip install -r requirements.txt --no-deps
      ...
      Installing collected packages: wordcloud, widgetsnbextension, webencodings, wcwidth, traitlets, tornado, testpath, terminado, six, send2trash, qtpy, qtconsole, pyzmq, pytz, python-dateutil, pyrsistent, pyparsing, pygments, pycparser, ptyprocess, prompt-toolkit, prometheus-client, pillow, pickleshare, pexpect, parso, pandocfilters, pandas, packaging, numpy, notebook, nest-asyncio, nbformat, nbconvert, nbclient, mistune, matplotlib-inline, matplotlib, markupsafe, kiwisolver, jupyterlab-widgets, jupyterlab-pygments, jupyter-core, jupyter-console, jupyter-client, jupyter, jsonschema, jinja2, jedi, ipywidgets, ipython-genutils, ipython, ipykernel, entrypoints, defusedxml, decorator, cycler, cffi, bleach, backcall, attrs, async-generator, argon2-cffi
      Successfully installed argon2-cffi-20.1.0 async-generator-1.10 attrs-21.2.0 backcall-0.2.0 bleach-3.3.0 cffi-1.14.5 cycler-0.10.0 decorator-5.0.9 defusedxml-0.7.1 entrypoints-0.3 ipykernel-5.5.5 ipython-7.24.0 ipython-genutils-0.2.0 ipywidgets-7.6.3 jedi-0.18.0 jinja2-3.0.1 jsonschema-3.2.0 jupyter-1.0.0 jupyter-client-6.1.12 jupyter-console-6.4.0 jupyter-core-4.7.1 jupyterlab-pygments-0.1.2 jupyterlab-widgets-1.0.0 kiwisolver-1.3.1 markupsafe-2.0.1 matplotlib-3.4.2 matplotlib-inline-0.1.2 mistune-0.8.4 nbclient-0.5.3 nbconvert-6.0.7 nbformat-5.1.3 nest-asyncio-1.5.1 notebook-6.4.0 numpy-1.20.3 packaging-20.9 pandas-1.2.4 pandocfilters-1.4.3 parso-0.8.2 pexpect-4.8.0 pickleshare-0.7.5 pillow-8.2.0 prometheus-client-0.10.1 prompt-toolkit-3.0.18 ptyprocess-0.7.0 pycparser-2.20 pygments-2.9.0 pyparsing-2.4.7 pyrsistent-0.17.3 python-dateutil-2.8.1 pytz-2021.1 pyzmq-22.1.0 qtconsole-5.1.0 qtpy-1.9.0 send2trash-1.5.0 six-1.16.0 terminado-0.10.0 testpath-0.5.0 tornado-6.1 traitlets-5.0.5 wcwidth-0.2.5 webencodings-0.5.1 widgetsnbextension-3.5.1 wordcloud-1.8.1

3. Запустити ``jupyter notebook``

   .. code:: console

      (.venv) jupyter notebook
      [I 18:28:39.354 NotebookApp] Serving notebooks from local directory: /home/oleksandr/workspace/github.com/anxolerd/kpi-ip92f-applied-methods-of-data-analysis
      [I 18:28:39.354 NotebookApp] Jupyter Notebook 6.4.0 is running at:
      [I 18:28:39.354 NotebookApp] http://localhost:8888/?token=<TOKEN HERE>
      [I 18:28:39.354 NotebookApp]  or http://127.0.0.1:8888/?token=<TOKEN HERE>
      [I 18:28:39.354 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
      [C 18:28:39.480 NotebookApp]

    To access the notebook, open this file in a browser:
        file:///home/oleksandr/.local/share/jupyter/runtime/nbserver-603351-open.html
    Or copy and paste one of these URLs:
        http://localhost:8888/?token=<TOKEN HERE>
     or http://127.0.0.1:8888/?token=<TOKEN HERE>
[I 18:29:38.294 NotebookApp] 302 GET /tree (127.0.0.1) 0.610000ms

4. Відкрити http://localhost:8888/tree у браузері, якщо це не відбулося автоматично, та за потреби введіит токен із виводу попередньої команди


Примітки
========

Згідно з угодою користування датасетом YELP, який використовується в лабораторних роботах 4 --- 6, публікувати його публічно заборонено. Тому папка з датасетом (``JSON``) в даному репозиторії порожня. Для роботи необхідно розпакувати датасет у директорію ``JSON``.

З тих же причин, більшість сформованих результатів відсутні у директорії ``out``. Утім, результати, отримані на основі датасету, але які не розкривають сам датасет (такі як зображення wordcloud) таки розміщені у директорії ``out``.
