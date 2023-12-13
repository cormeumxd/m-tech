# Тестовое задание М.Тех

Этот репозиторий содержит решение тестового задания на стажировку М.Тех по направлению «Младший исследователь данных (DS)»

## Предварительные требования

- Docker установлен на вашем компьютере.

## Как запустить

### Первый вариант
```
docker run -p 8501:8501 -p 8888:8888 ghcr.io/cormeumxd/m-tech-image:latest
```

### Если первый не сработал
1. Склонируйте репозиторий:

   ```bash
   git clone https://github.com/cormeumxd/m-tech.git
   
2. Перейдите в директорию проекта:

   ```bash
   cd m-tech

3. Создайте докер-образ:

   ```
   docker build -t your_image_name .
   ```

4. Запустите докер контейнер следующей командой:

   ```
   docker run -p 8501:8501 -p 8888:8888 your_iamge_name
   ```

В итоге запустится сервер streamlit, используя порт 8501 и jupyter-notebook, используя порт 8888. При необходимости порт можно изменить.
Так же дэшборд отдельно поднят на сервере: https://cormeumxd-m-tech-dashboard-gznhlr.streamlit.app/