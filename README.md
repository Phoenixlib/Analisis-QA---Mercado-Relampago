# ⚡ Proyecto QA: Mercado Relámpago

Este repositorio contiene la documentación y el análisis de calidad de software (QA) realizado sobre la plataforma de comercio electrónico simulada **"Mercado Relámpago"**.

El proyecto se enfoca en demostrar la capacidad de realizar pruebas exhaustivas, documentar fallos críticos y establecer una estrategia de priorización en un entorno de alto tráfico (Cyberday), utilizando estándares de la industria.

**QA Lead/Analista:** Pablo Puentes

## 1. Documentación Generada

La documentación QA se organizó en los siguientes artefactos clave, disponibles en este repositorio:

| **Archivo** | **Contenido** | 
 | ----- | ----- | 
| `plan_de_pruebas.md` | Estrategia, Alcance y Casos de Prueba Clave. | 
| `reporte_de_errores.md` | Documentación detallada de 6 fallos críticos. | 
| `Analisis_Priorizacion_QA.md` | Matriz de Priorización (Severidad vs. Impacto) y Propuestas de Solución Técnica. | 

## 2. Resumen de Fallos Críticos (Prioridad P1)

Se identificaron dos fallos de máxima prioridad que impactan directamente la rentabilidad y el cumplimiento de pedidos.

| **ID Bug** | **Fallo Detectado** | **Impacto en el Negocio** | **Recomendación Técnica Clave** | 
 | ----- | ----- | ----- | ----- | 
| **BUG-BL-002** | Doble Descuento | Pérdida financiera grave (30% en lugar de 15%). | Corregir lógica de cálculo en el Carrito (`useMemo`). | 
| **BUG-BL-001** | Sobreventa de Stock | Incumplimiento de pedidos y clientes insatisfechos. | Validar stock estrictamente en Frontend y Backend. | 

## 3. Cobertura de Pruebas Adicional

El análisis se extendió a áreas de calidad que van más allá de la funcionalidad:

* **Rendimiento Web (Web Performance):** Identificación de *Cumulative Layout Shift* (CLS) por carga tardía de elementos (BUG-WP-002).

* **Usabilidad Móvil (UX):** Reporte de fallos en el tamaño del objetivo táctil (*Touch Target Size*) en la aplicación de logística (BUG-UX-001).

* **Seguridad y Datos:** Fallo en la validación de longitud de contraseñas y formato de email (BUG-FV-001).

* **Accesibilidad (A11y):** Fallo de Contraste de Color WCAG AA en etiquetas de producto (BUG-A11Y-001).
