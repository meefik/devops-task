# TO DO

Доработайте сценарий `docker-compose.yml` следующим образом:

1. Контейнер `proxy` на базе образа `bitnami/nginx` должен выпонять функцию обратного прокси-сервера (reverse proxy) с равномерным распределением запросов по двум бэкендам.

2. Контейнер `backend1` на базе образа `bitnami/nginx` должен возвращать страницу `index.html` из каталога `backend1`.

3. Контейнер `backend2` на базе образа `bitnami/nginx` должен возвращать страницу `index.html` из каталога `backend2`.

4. Обращение к контейнерам должно осуществляться по внутренней сети Docker без доступа извне.

5. При запросе страницы веб-сервер должен поочередно отвечать страницей `backend1` и `backend2`.
