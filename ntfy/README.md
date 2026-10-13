![ntfy](web/public/static/images/ntfy.png)

# SINA

**SINA** es un sistema de notificaciones basado en [ntfy](https://github.com/binwiederhier/ntfy), 
un servicio de notificaciones HTTP [pub-sub](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) 
que permite enviar notificaciones a tu teléfono o computadora mediante scripts, sin necesidad de registrarse 
ni pagar tarifas.

Este módulo (`ntfy/`) es el **motor base** del proyecto SINA, desarrollado como parte del proyecto de 
residencias profesionales.

## Documentación

- [Getting started](docs/index.md)
- [Android/iOS](docs/subscribe/phone.md)
- [API](docs/publish.md)
- [Install / Self-hosting](docs/install.md)
- [Building](docs/develop.md)

## Créditos

SINA está basado en el proyecto open source **ntfy**, creado por 
[Philipp C. Heckel](https://heckel.io) y publicado bajo doble licencia 
[Apache 2.0](LICENSE) / [GPLv2](LICENSE.GPLv2).

El código original de ntfy se conserva íntegro en este directorio. 
Las adaptaciones específicas de SINA se encuentran fuera de esta carpeta (en la raíz del proyecto).
