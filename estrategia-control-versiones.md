# Estrategia de control de versiones y seguridad

## 1. Contexto del proyecto

El proyecto corresponde al Sistema de Biblioteca y el archivo trabajado es `Login.java`. Este archivo contiene el proceso de autenticación del usuario, por lo que requiere control de versiones y validaciones de seguridad antes de ser publicado en producción.

## 2. Historial de versiones tomado de la plantilla

| Versión | Fecha | Autor | Descripción del cambio | Tipo de cambio | Aprobó |
|---|---|---|---|---|---|
| v1.0 | 10/7/2026 | Juan Pérez | Creación inicial del archivo | Creación | Docente |
| v1.1 | 10/7/2026 | María López | Se agregó validación del usuario | Mejora | Juan Pérez |
| v1.2 | 11/7/2026 | Carlos Díaz | Corrección de errores en el login | Corrección | Docente |
| v1.3 | 11/7/2026 | Ana Ruiz | Se agregó recuperación de contraseña | Nueva funcionalidad | María López |
| v1.4 | 12/7/2026 | Pedro Silva | Optimización del proceso de autenticación | Optimización | Docente |

## 3. Ambientes de trabajo

| Ambiente | Uso dentro del proyecto |
|---|---|
| Desarrollo | Se realizan cambios iniciales en `Login.java`. |
| Certificación | Se validan cambios, se revisan errores y se ejecutan pruebas de seguridad. |
| Producción | Se publica únicamente la versión estable y aprobada. |

## 4. Estrategia en GitHub

Para organizar el trabajo se propone usar las siguientes ramas:

| Rama | Propósito |
|---|---|
| main | Versión estable del proyecto. |
| desarrollo | Cambios iniciales y mejoras del login. |
| certificacion | Revisión de errores y pruebas de seguridad. |
| seguridad-login | Validaciones de contraseña y autenticación. |

## 5. Pruebas de seguridad antes del lanzamiento

Antes de pasar a producción, el archivo `Login.java` debe ser revisado con pruebas básicas de seguridad:

- Validar que el usuario exista.
- Verificar que la contraseña no sea débil.
- Evitar contraseñas comunes como `123456`, `admin` o `password`.
- Controlar intentos fallidos de acceso.
- Validar el código enviado al teléfono móvil.
- No mostrar mensajes que revelen información sensible.

## 6. Recuperación de versión anterior

Según la plantilla, la versión recuperada fue la `v1.2`, debido a que la versión `v1.4` presentó errores. Esta recuperación demuestra que el control de versiones permite regresar a una versión estable cuando una modificación afecta el funcionamiento del sistema.

## 7. Conclusión de la estrategia

La estrategia permite controlar los cambios del archivo `Login.java`, organizar el trabajo por ambientes y aplicar pruebas de seguridad antes del lanzamiento. GitHub sirve como evidencia del historial del proyecto y permite documentar los cambios realizados.
