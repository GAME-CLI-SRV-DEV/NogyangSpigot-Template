# NogyangSpigot-Template
NogyangSpigot Plugin Template, utilizes [Foundation](https://github.com/kangarko/foundation) v6 in NogyangSpigot-API 1.21.4

# To Make your Plugin Work only on NogyangSpigot, Follow these steps:

Choose either `Spigot-API` or `Paper-API`, or `NogyangSpigot-API`(You need to build the dependency and publish it to `mavenlocal()`.).\
Replace `plugin.yml` with `paper-plugin.yml`. Spigot will not detect paper-plugin.yml so it wont load on it by saying plugin.yml is missing. but it will instead load on paper and it's fork.\
Replace `extends JavaPlugin` with `extends SimplePlugin`. this is foundation usage. since the foundation was compileOnly dependency, it wont work on Paper at all since NogyangSpigot only embeds Foundation. it also means that you also need to rebuild the fork on NogyangSpigot by applying fork patches yourself.

# Using NMS

## Internals
> [!CAUTION]
> it is not recommended to use NMS Internal. Instead you should depend on ProtocolLib/packetevents!

use `paperweight-userdev`. 
