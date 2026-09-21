# Pruebas de Humo (Smoke Test)

## 1. Información General
* **Nombre del Proyecto:** Plan de pruebas -- Toolshop
* **Versión / Build:** Versión 1.0
* **Fecha de Ejecución:** 14/09/2026
* **Responsable / QA:** Jenny Sofía Morales López
* **Entorno:** Entorno de QA

---

## 2. Casos de Prueba

| ID | Módulo / Componente | Descripción de la Acción | Resultado Esperado | Estado (Pass/Fail) | Observaciones |
|----|---------------------|--------------------------|---------------------|--------------------|---------------|
| SM-01 | Autenticación | Ingresar con credenciales válidas en el login. | El usuario accede al panel principal correctamente. | `[Pass]` | Carga en menos de 2s. |
| SM-02 | Navegabilidad | Hacer clic en el menú principal de navegación. | Los módulos cargan sin errores 404 ni pantallas en blanco. | `[Pass]` | - |
| SM-03 | Base de Datos | Realizar una consulta o lectura de datos clave. | Los datos se muestran en la interfaz sin interrupciones. | `[Fail]` | Error de conexión con API. |
| SM-04 | Funcionalidad Crítica | Crear o enviar un registro básico (ej. guardar perfil). | El sistema confirma el almacenamiento exitoso del registro. | `[Pendiente]` | Bloqueado por SM-03. |

---

## 3. Resumen y Criterios de Aprobación
* **Total de Pruebas:** 4
* **Aprobadas (Pass):** 2
* **Fallidas (Fail):** 1
* **Bloqueadas / Pendientes:** 1
* **Decisión Final:** **RECHAZADO** (La compilación no es estable para pasar a la fase de pruebas funcionales profundas debido a fallos críticos en la API).
