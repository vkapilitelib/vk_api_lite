# vk_api_lite
Небольшая библиотека для работы с VK API через access_token (wall.post, wall.get, photos.save)

```Python
from vk_api_lite import VkAPILite

vk_api_l = VkAPILite(TOKEN='vk1.a.OVgI7F9psMHdS4954SQ_6ksmDM0cFsZ6rCGYxbXJyR00A3Hqa76H6VI0anrkYLBTuxVtrXXT7fAK-YzSC78OhT2V_3FoqMQCwFHCi6utgVytIinZWNrxUlwKx_jPF7P0kgGbUq9QViyHvR0TUN35oobk7dBo8-QsiGT1afvS3KkKf0cbbgZ8UeAEiobq3Ctr')

# Получить информацию со стены сообщества по id
wall_content = vk_api_l.wallGetById(1)

# Получить информацию со стены сообщества по domain
wall_content = vk_api_l.wallGetByDomain('apiclub')

# Обубликовать пост на стене сообщества
vk_api_l.wallPost(1, message="Hello, World!")

# Загрузть фото на сервер и получить id
id_list = vk_api_l.photosSave(22822305, 126315661, ['1.png', '2.png'])
```

## Поддерживаваемые методы

```wall.get``` - https://dev.vk.com/method/wall.get

```wall.post``` - https://dev.vk.com/method/wall.post

```photos.save``` - https://dev.vk.com/method/photos.save

