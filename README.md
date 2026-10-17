# 📡 Sistema de Gestión Empresa Tigo (.NET WinForms)

Un sistema de escritorio desarrollado en **C# y .NET Framework** enfocado en la administración de clientes, contratos, planes de telecomunicaciones y suscripciones a servicios adicionales (TV Cable, Internet, plataformas de streaming, etc.).

---

## 🚀 Características Principales

* 🔐 **Autenticación Multirrol:** Inicios de sesión diferenciados para **Administradores** y **Clientes**.
* 📋 **Gestión de Clientes y Usuarios:** Registro, modificación y consulta de perfiles.
* 📦 **Administración de Paquetes y Planes:** Visualización y gestión de paquetes de telecomunicaciones.
* ➕ **Servicios Adicionales:** Contratación e integración de plataformas adicionales (Disney+, HBO Max, Paramount+, TV Cable, WiFi).
* 📝 **Gestión de Contratos y Pagos:** Registro de contratos activos, procesamiento y seguimiento de pagos.
* 🗄️ **Persistencia en Base de Datos:** Scripts SQL para la creación del esquema relacional y almacenamiento estructurado.
* 🎨 **Interfaz Moderna:** Integración de **FontAwesome.Sharp** para iconos vectoriales y una navegación fluida.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** C#
* **Framework:** .NET Framework 4.7.2 (Windows Forms)
* **Librerías GUI:** FontAwesome.Sharp (v6.6.0)
* **Base de Datos:** SQL Server / T-SQL (`crear_tablas.sql`)
* **Testing:** MSTest / Microsoft Visual Studio Test Platform

---

## 📂 Estructura del Proyecto

```text
Empresa_Tigo/
├── Clases/                      # Lógica de negocio y entidades
│   ├── BaseDatos.cs             # Conexión y operaciones de base de datos
│   ├── Cliente.cs               # Entidad Cliente
│   ├── Usuario.cs / IUsuario.cs # Gestión e interfaces de usuarios
│   ├── Paquete.cs               # Planes y paquetes de servicios
│   ├── Contrato.cs              # Gestión de contratos
│   ├── Pago.cs                  # Procesamiento de pagos
│   └── ServisioAdicional.cs     # Servicios extra y plataformas
├── form/                        # Formularios e interfaz de usuario (WinForms)
│   ├── FormLoginAdmi.cs         # Login para administradores
│   ├── FormLoginCliente.cs      # Login para clientes
│   ├── FormAdmi.cs              # Panel principal de administración
│   ├── FormCliente.cs           # Panel principal de cliente
│   └── FormPaquetes.cs          # Catálogo y configuración de paquetes
├── Resources/                   # Recursos visuales (logotipos e iconos)
└── crear_tablas.sql             # Script SQL de creación de la base de datos
