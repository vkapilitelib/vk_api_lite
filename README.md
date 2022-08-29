# vk_api_lite
Small library for VK API (via access_token)

```Python
from vk_api_lite import VkAPILite

vk_api_l = VkAPILite(TOKEN='vk1.a.Yout.Token')

# Get info from wall by id
wall_content = vk_api_l.wallGetById(1)

# Get info from wall by domain
wall_content = vk_api_l.wallGetByDomain('apiclub')

# wall.post
vk_api_l.wallPost(1, message="Hello, World!")

# photos.save
id_list = vk_api_l.photosSave(22822305, 126315661, ['1.png', '2.png'])
```

## Supported methods

```wall.get``` - https://dev.vk.com/method/wall.get

```wall.post``` - https://dev.vk.com/method/wall.post

```photos.save``` - https://dev.vk.com/method/photos.save

