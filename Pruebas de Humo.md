# Pruebas de Humo (Smoke Test)

## 1. Información General
* **Nombre del Proyecto:** Plan de pruebas -- Toolshop
* **Versión / Build:** Versión 1.0
* **Fecha de Ejecución:** 14/09/2026
* **Responsable / QA:** Jenny Sofía Morales López
* **Entorno:** Entorno de QA

---

## 2. Casos de Prueba

| ID | Módulo / Componente | Acción | Resultado Esperado |
|----|---------------------|--------------------------|---------------------|
| SM-01 | Infraestructura | Revisar docker | Los servicios requeridos aparecen en estado Up. | 
| SM-02 | Catálogo | Abrir http://localhost:4200 | La página carga y muestra el catálogo de productos. | 
| SM-03 | Navegación | Abrir categorías y el detalle de un producto | Las páginas cargan sin errores 404 ni pantallas en blanco. |
| SM-04 | Autenticación | Iniciar sesión con una cuenta válida | El sistema autentica al usuario y muestra la sesión activa. |
| SM-05 | Carrito | Agregar un producto al carrito | El producto aparece en el carrito con cantidad y precio. |
| SM-06 | API | Abrir Swagger o consultar un endpoint | Swagger responde y la API devuelve una respuesta válida. |
---
### Evidencia SM-01

* **Código:** EV-SM-01
* **Caso relacionado:** SM-01
* **Descripción:** Estado de los contenedores obtenido .
* **Fecha:** 16/09/2026
* **Resultado observado:** Contenedores conrriendo correctamente
* **Archivo:** `EV-SM-01_contenedores_activos.png`

![EV-SM-01 - Contenedores Docker](evidencias/EV-SM-01_contenedores_activos.png)

### Evidencia SM-02

* **Código:** EV-SM-02
* **Caso relacionado:** SM-02
* **Descripción:** Carga de la página principal y catálogo.
* **Fecha:** 16/09/2026
* **Resultado observado:** [Describir lo que apareció]
* **Archivo:** `EV-SM-02-catalogo.png`

![EV-SM-02 - Catálogo de productos](evidencias/EV-SM-02-catalogo.png)

### Evidencia SM-03

* **Código:** EV-SM-03
* **Caso relacionado:** SM-03
* **Descripción:** Navegación hacia una categoría y detalle de producto.
* **Fecha:** 16/09/2026
* **Resultado observado:** [Describir lo que apareció]
* **Archivo:** `EV-SM-03-navegacion.png`

![EV-SM-03 - Navegación](evidencias/EV-SM-03-navegacion.png)

### Evidencia SM-04

* **Código:** EV-SM-04
* **Caso relacionado:** SM-04
* **Descripción:** Inicio de sesión con credenciales válidas.
* **Fecha:** 16/09/2026
* **Resultado observado:** [Describir lo que apareció]
* **Archivo:** `EV-SM-04-login.png`

![EV-SM-04 - Inicio de sesión](evidencias/EV-SM-04-login.png)

### Evidencia SM-05

* **Código:** EV-SM-05
* **Caso relacionado:** SM-05
* **Descripción:** Producto agregado al carrito.
* **Fecha:** 16/09/2026
* **Resultado observado:** [Describir lo que apareció]
* **Archivo:** `EV-SM-05-carrito.png`

![EV-SM-05 - Carrito](evidencias/EV-SM-05-carrito.png)

### Evidencia SM-06

* **Código:** EV-SM-06
* **Caso relacionado:** SM-06
* **Descripción:** Acceso a Swagger o respuesta de un endpoint.
* **Fecha:** 16/09/2026
* **Resultado observado:** [Describir lo que apareció]
* **Archivo:** `EV-SM-06-swagger.png`

![EV-SM-06 - API Swagger](evidencias/EV-SM-06-swagger.png)


## 3. Resumen y Criterios de Aprobación
* **Total de Pruebas:** 4
* **Aprobadas (Pass):** 2
* **Fallidas (Fail):** 1
* **Bloqueadas / Pendientes:** 1
* **Decisión Final:** **RECHAZADO** (La compilación no es estable para pasar a la fase de pruebas funcionales profundas debido a fallos críticos en la API).
