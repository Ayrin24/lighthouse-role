# lighthouse-role

Устанавливает Nginx и деплоит статику LightHouse.

## Переменные (defaults)

| Переменная | Значение по умолчанию |
|---|---|
| `lighthouse_version` | `0.1.0` |
| `lighthouse_download_url` | `.../master.tar.gz` |
| `lighthouse_install_dir` | `/var/www/lighthouse` |
| `nginx_listen_port` | `80` |
| `nginx_server_name` | `_` |

## Зависимости

- Nginx (устанавливается внутри роли)

## Использование

```yaml
- hosts: lighthouse
  become: true
  roles:
    - lighthouse-role
