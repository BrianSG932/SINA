# SINA — Sistema Integral de Notificaciones y Alertas

![Logo ITMH](https://www.matehuala.tecnm.mx/images/logo-itmh.png)

**SINA** es un sistema integral de notificaciones y alertas diseñado para informar de manera inmediata, segura y segmentada a estudiantes, docentes y personal del **Instituto Tecnológico de Matehuala (TecNM)** sobre situaciones de emergencia, contingencias y avisos institucionales.

El sistema permite enviar notificaciones segmentadas por **edificio, departamento, carrera, área administrativa, grupo o tipo de usuario**, fortaleciendo la prevención, mejorando la capacidad de respuesta y optimizando la comunicación institucional.

> ⚠️ **Nota:** SINA funciona como **complemento tecnológico** de los mecanismos tradicionales de alarma y de los protocolos oficiales de Protección Civil. **No los sustituye.**

---

## 📋 Tabla de contenidos

- [Objetivo general](#-objetivo-general)
- [Objetivos específicos](#-objetivos-específicos)
- [Características principales](#-características-principales)
- [Arquitectura y tecnologías](#-arquitectura-y-tecnologías)
- [Estructura del repositorio](#-estructura-del-repositorio)
- [Instalación](#-instalación)
- [Uso](#-uso)
- [Equipo de desarrollo](#-equipo-de-desarrollo)
- [Asesores](#-asesores)
- [Créditos y licencias](#-créditos-y-licencias)

---

## 🎯 Objetivo general

Desarrollar e implementar **SINA**, un sistema integral de notificaciones y alertas que permita informar de manera inmediata, segura y segmentada a estudiantes, docentes y personal del Tecnológico Nacional de México sobre situaciones de emergencia, contingencias y avisos institucionales, de acuerdo con su ubicación, área, carrera o grupo de pertenencia, con el propósito de fortalecer la prevención, mejorar la capacidad de respuesta y optimizar la comunicación institucional.

---

## ✅ Objetivos específicos

1. Analizar los mecanismos actuales utilizados para comunicar emergencias, contingencias y avisos institucionales, identificando sus principales necesidades y limitaciones.
2. Diseñar una plataforma centralizada para generar, administrar y distribuir alertas y notificaciones institucionales.
3. Implementar mecanismos de segmentación de destinatarios por edificio, departamento, carrera, área administrativa, grupo o tipo de usuario.
4. Establecer diferentes niveles de prioridad para distinguir alertas críticas, preventivas, operativas y notificaciones informativas.
5. Desarrollar un módulo para la emisión inmediata de alertas relacionadas con incendios, situaciones de violencia, inundaciones, fallas eléctricas, fenómenos naturales, evacuaciones, simulacros y otras contingencias.
6. Implementar un módulo de notificaciones académico-administrativas (servicio social, residencias profesionales, trámites, convocatorias y fechas importantes).
7. Establecer roles y permisos que determinen qué usuarios están autorizados para emitir cada tipo de alerta o notificación.
8. Mantener un registro histórico con la información de emisor, fecha, destinatarios y clasificación de cada notificación.
9. Realizar pruebas funcionales y un ejercicio piloto que evalúe el funcionamiento, alcance y tiempos de entrega.
10. Documentar el funcionamiento técnico y operativo del sistema para facilitar su mantenimiento y futura ampliación.

---

## 🚀 Características principales

### Tipos de notificaciones
- 🚨 **Alertas críticas:** incendios, violencia, inundaciones, evacuaciones
- ⚠️ **Alertas preventivas:** fenómenos naturales, fallas eléctricas, simulacros
- 📢 **Avisos operativos:** comunicados institucionales
- 📚 **Notificaciones académico-administrativas:** servicio social, residencias, trámites y convocatorias

### Segmentación de destinatarios
- Por **edificio**
- Por **departamento**
- Por **carrera**
- Por **área administrativa**
- Por **grupo**
- Por **tipo de usuario** (estudiante, docente, administrativo)

### Seguridad y trazabilidad
- Autenticación y autorización por roles
- Control de privilegios para emisión de alertas críticas
- Registro histórico completo: emisor, fecha, hora, destinatarios y estado del envío

---

## 🏗️ Arquitectura y tecnologías

SINA está construido sobre el motor de **[ntfy](https://github.com/binwiederhier/ntfy)**, un servicio de notificaciones HTTP pub-sub de código abierto, al cual se le han añadido capas de segmentación, roles institucionales y módulos específicos para el contexto del TecNM.

| Componente | Tecnología |
|------------|------------|
| **Backend** | Go (basado en ntfy) |
| **Frontend** | React + Material UI |
| **Base de datos** | SQLite / PostgreSQL |
| **Protocolo** | HTTP pub-sub |
| **Notificaciones push** | Firebase Cloud Messaging (FCM) / Web Push |
| **Autenticación** | Basada en tokens con roles y permisos |

---

## 📁 Estructura del repositorio
