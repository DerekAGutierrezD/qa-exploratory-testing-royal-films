# 🎬 QA Exploratory Testing – Royal Films

## 📋 ¿Qué es esto?
Proyecto de pruebas exploratorias manuales ejecutadas sobre el sitio web 
royalfilms.com.co, enfocado en identificar defectos funcionales en flujos 
críticos de usuario como registro, compra de entradas y membresías.

---

## 🎯 Objetivo
Identificar vulnerabilidades y fallos funcionales que impactan directamente 
la experiencia del usuario y generan fricción en el proceso de compra.

---

## 🔍 Alcance
**Incluido:**
- Formulario de registro de usuario
- Flujo de compra de entradas (selección → pago → cancelación)
- Sección de membresías

**Excluido:**
- Pruebas de carga o rendimiento
- Pruebas de seguridad
- Flujo de pago real (no se completaron transacciones)

---

## 🛠️ Herramientas utilizadas
- **Jira** – Reporte y gestión de defectos
- **Google Chrome** – Navegador de prueba (Desktop y Mobile)
- **Captura de pantalla** – Evidencia visual de cada bug

---

## 🐛 Bugs encontrados

| ID | Título | Severidad |
|----|--------|-----------|
| BUG-001 | Campo "Nombre y Apellido" acepta caracteres numéricos sin validación | Media |
| BUG-002 | Error 502 y página vacía al cancelar el proceso de pago | Alta |
| BUG-003 | Modal de planes de membresía no muestra opciones al hacer clic en "Comprar ya" | Alta |

---

## 🔑 Decisiones clave
- Se priorizaron flujos de compra y registro por su impacto directo en la 
  conversión de usuarios.
- Se ejecutaron pruebas tanto en desktop como en mobile para cubrir 
  comportamiento responsive.
- Se documentaron únicamente defectos reproducibles con evidencia visual.

---

## 📊 Resultados
- 3 bugs documentados: 2 de severidad Alta, 1 de severidad Media
- Los bugs de severidad Alta bloquean flujos completos de compra y membresía
- Evidencia registrada en Jira con pasos de reproducción, resultado esperado 
  vs actual y capturas de pantalla

---

## 🔄 ¿Qué mejoraría después?
- Ampliar la cobertura con validación de API usando Postman en los endpoints 
  de compra
- Agregar casos de prueba formales complementarios a las sesiones exploratorias

---

## 📁 Archivos en este repositorio
| Archivo | Descripción |
|---------|-------------|
| `README.md` | Documentación del proyecto |
| `bug-reports/BUG-001.png` | Captura campo nombre acepta números |
| `bug-reports/BUG-003.png` | Captura modal membresía sin opciones |
