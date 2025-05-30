# Análisis de la Hoja de Cálculo DSI desde la Perspectiva de un Director de Sistemas de Información

## 1. PLANIFICACIÓN - Análisis de la Estructura del Sistema

### 1.1 Arquitectura de Datos Implementada

**Fortalezas identificadas:**
• Diseño modular: La estructura de 5 hojas especializadas (Alumnos, EC Individual, Grupos, ComponentesSI, NumerosDelParcial) demuestra una correcta separación de concerns y normalización de datos
• Integridad referencial: Sistema de nombres definidos para validación cruzada entre hojas
• Escalabilidad: Capacidad para manejar 82 estudiantes distribuidos en 4 grados universitarios

**Métricas del sistema:**
• Cobertura de datos: 100% de estudiantes registrados con seguimiento individual
• Granularidad temporal: Seguimiento sesión por sesión de asistencia
• Diversidad de métricas: Evaluación continua, parciales y análisis demográfico integrados

### 1.2 Alineación con Objetivos Estratégicos

El sistema responde a los cuatro pilares fundamentales de la dirección de SI:
• Planificación: Estructura predefinida para seguimiento académico
• Organización: Clasificación por grados, grupos y componentes evaluativos
• Dirección: Métricas de rendimiento y asistencia para toma de decisiones
• Control: Validaciones automáticas y alertas de cumplimiento

## 2. ORGANIZACIÓN - Estructura y Gobernanza de Datos

### 2.1 Distribución Demográfica y Organizacional

**Composición estudiantil por grado:**

| Grado | Estudiantes | Porcentaje | Representación |
|-------|-------------|------------|----------------|
| Ingeniería Informática (II) | 36 | 43.9% | Mayor representación |
| Administración y Dirección de Empresas (ADE) | 25 | 30.5% | Significativa |
| Ingeniería de Organización Industrial (IOI) | 14 | 17.1% | Moderada |
| Grado en Proceso de Ingeniería (GPI) | 5 | 6.1% | Grupo minoritario |
| **TOTAL** | **82** | **100%** | - |

**Análisis de diversidad internacional:**

| Criterio | Cantidad | Porcentaje | Observaciones |
|----------|----------|------------|---------------|
| Estudiantes Españoles | 50 | 62.5% | Mayoría nacional |
| Estudiantes Extranjeros | 30 | 37.5% | Excelente internacionalización |
| **TOTAL** | **80** | **100%** | Estrategia exitosa de atracción internacional |

### 2.2 Framework de Gestión de Grupos

El sistema implementa un **algoritmo de validación automática** para composición de grupos que evalúa:

• Porcentajes mínimos y máximos por grado
• Distribución de género
• Balance entre estudiantes nacionales e internacionales

**Valor estratégico:** Esta automatización reduce errores manuales y garantiza equidad en la formación de equipos de trabajo.

## 3. DIRECCIÓN - Indicadores de Rendimiento y Calidad

### 3.1 KPIs Académicos Principales

**Rendimiento global de la asignatura:**

| Métrica | Cantidad | Porcentaje | Benchmark |
|---------|----------|------------|-----------|
| Aprobados | 76 | 92.7% | 🟢 Excelente (+17.7% vs media nacional) |
| Suspensos | 5 | 6.1% | 🟢 Muy bajo (-18.9% vs media nacional) |
| No evaluados | 1 | 1.2% | 🟢 Mínimo |
| **TOTAL** | **82** | **100%** | Superior a media nacional (≈75%) |

**Calidad académica:**

| Indicador | Valor | Clasificación | Observaciones |
|-----------|-------|---------------|---------------|
| Media de calificaciones | 7.60/10 | 🟢 Notable | Supera expectativas |
| Desviación estándar | - | Pendiente cálculo | Requerido para análisis completo |
| Mediana | - | Pendiente cálculo | Análisis de distribución |

### 3.2 Análisis de Asistencia por Segmentos

**Comparativa de asistencia por grado:**

| Grado | Tasa de Asistencia | Estado | Acción Requerida |
|-------|-------------------|--------|------------------|
| IOI | 78.8% | 🟢 Excelente | Mantener buenas prácticas |
| II | ~75.0% | 🟡 Aceptable | Monitoreo continuo |
| ADE | 69.2% | 🔴 Requiere intervención | Plan de mejora inmediato |

**Análisis de brecha de asistencia:**

| Métrica | Valor | Implicaciones |
|---------|-------|---------------|
| Mejor desempeño (IOI) | 78.8% | Benchmark interno |
| Peor desempeño (ADE) | 69.2% | Requiere intervención |
| Gap de rendimiento | 9.6% | Significativo - Acción inmediata |
| Correlación tamaño-asistencia | Inversa (hipótesis) | Validar con análisis estadístico |

### 3.3 Evaluación Continua - Componentes SI

**Análisis de participación en evaluaciones:**

| Estado | Cantidad | Porcentaje | Semáforo | Observaciones |
|--------|----------|------------|----------|---------------|
| Presentados | 67 | 81.7% | 🟡 Mejorable | Por debajo del objetivo 85% |
| No presentados | 15 | 18.3% | 🔴 Riesgo | Requiere seguimiento individual |
| **TOTAL** | **82** | **100%** | - | Gap identificado |

**Comparativa con otros indicadores:**

| Métrica | ComponentesSI | Rendimiento General | Diferencial |
|---------|---------------|-------------------|-------------|
| Participación | 81.7% | 98.8% (evaluados) | -17.1% |
| No participación | 18.3% | 1.2% (no evaluados) | +17.1% |

**Análisis de riesgo:** El 18% de no presentación representa un riesgo significativo para el cumplimiento de objetivos académicos y requiere intervención inmediata.

## 4. CONTROL - Sistemas de Monitoreo y Mejora Continua

### 4.1 Métricas de Control Implementadas

**Dashboard de seguimiento académico:**

| Componente | Estado Actual | Funcionalidad | Efectividad |
|------------|---------------|---------------|-------------|
| Indicadores cromáticos | 🟢 Activo | Alertas visuales automáticas | Alta |
| Validaciones tiempo real | 🟢 Activo | Control de integridad | Alta |
| Seguimiento por sesión | 🟢 Activo | Granularidad detallada | Alta |
| Alertas proactivas | 🔴 Ausente | Notificaciones automáticas | Pendiente |

**Análisis del sistema de examen parcial:**

| Funcionalidad | Implementación | Utilidad | Prioridad de Mejora |
|---------------|----------------|----------|-------------------|
| Tracking de respuestas por pregunta | ✓ Implementado | Alta | Baja |
| Monitoreo de procedimientos | ✓ Implementado | Media | Media |
| Análisis estadístico de patrones | ✓ Implementado | Alta | Baja |
| Análisis predictivo | ✗ No implementado | Muy Alta | **Alta** |

### 4.2 Infraestructura Tecnológica

**Stack tecnológico actual:**

| Componente | Herramienta | Versión/Tipo | Evaluación | Limitaciones |
|------------|-------------|--------------|------------|--------------|
| Plataforma base | Microsoft Excel | Desktop | 🟡 Funcional | Escalabilidad limitada |
| Lógica de negocio | Fórmulas complejas | Avanzadas | 🟢 Efectivo | Mantenibilidad compleja |
| Integridad de datos | Referencias nombradas | Nativo | 🟢 Robusto | Sin versionado |
| Control de calidad | Validación de datos | Automático | 🟡 Básico | Sin auditoría |

**Evaluación de madurez tecnológica:**

| Nivel | Descripción | Estado Actual | Siguiente Nivel |
|-------|-------------|---------------|-----------------|
| 1 - Inicial | Procesos ad-hoc | ✗ Superado | - |
| 2 - Repetible | Procesos básicos | ✗ Superado | - |
| 3 - Definido | Documentado y estandarizado | ✅ Actual | Optimización |
| 4 - Gestionado | Medición y control | 🔄 En progreso | Automatización completa |
| 5 - Optimizado | Mejora continua | ⏸ Objetivo | Transformación digital |

## 5. FRAMEWORK DE TRABAJO IDENTIFICADO

### 5.1 Arquitectura de Capas

**Evaluación por componente arquitectónico:**

| Capa | Función | Implementación Actual | Madurez | Próximos Pasos |
|------|---------|----------------------|---------|----------------|
| Presentación | Dashboards y vistas | Excel sheets especializadas | 🟡 Básica | UI/UX interactiva |
| Lógica de Negocio | Validaciones y cálculos | Fórmulas y macros avanzadas | 🟢 Sólida | APIs y microservicios |
| Datos | Estructura normalizada | Hojas relacionadas | 🟢 Buena | Base de datos relacional |
| Persistencia | Almacenamiento | Archivo Excel local | 🔴 Limitada | Cloud + versionado |

## 6. PROPUESTAS DE MEJORA ESTRATÉGICA

### 6.1 Mejoras de Corto Plazo (0-6 meses)

| Mejora | Descripción | Impacto Esperado | Recursos Necesarios | Timeline |
|--------|-------------|------------------|-------------------|----------|
| Dashboard Ejecutivo Interactivo | Filtros dinámicos, gráficos tiempo real, KPIs con semáforos | 🟢 Alto | 1 Analista BI × 2 meses | Q1 |
| Sistema de Alertas Proactivas | Notificaciones automáticas asistencia <75%, riesgo académico <5.0 | 🟢 Alto | 1 Desarrollador × 1 mes | Q1 |
| Métricas Avanzadas de Calidad | NPS académico, tiempo resolución ejercicios, correlaciones | 🟡 Medio | 1 Data Scientist × 1 mes | Q2 |

### 6.2 Mejoras de Medio Plazo (6-18 meses)

| Mejora | Descripción | Impacto Esperado |
|--------|-------------|------------------|
| Integración Sistemas | API gestión académica, campus virtual, videoconferencia | 🟢 Muy Alto |
| Análisis Predictivo & ML | Modelo riesgo abandono, recomendaciones grupos, predicción rendimiento | 🟢 Muy Alto |
| Gamificación & Engagement | Badges asistencia, ranking grupos, challenges semanales | 🟡 Medio |

### 6.3 Mejoras de Largo Plazo (18+ meses)

| Iniciativa Estratégica | Objetivo |
|------------------------|----------|
| Plataforma BI Enterprise | Migración Power BI/Tableau con drill-down y benchmarking |
| Certificación ISO 21001 | Gestión calidad educativa con auditorías automáticas |
| Centro de Excelencia Académica | Hub de mejores prácticas y análisis comparativo |

## 7. EVALUACIÓN DE RIESGOS Y MITIGACIÓN

### 7.1 Matriz de Riesgos Identificados

| Riesgo | Probabilidad | Impacto | Nivel | Descripción | Estrategia de Mitigación |
|--------|--------------|---------|-------|-------------|-------------------------|
| Dependencia Excel | Alta | Alto | 🔴 CRÍTICO | Plataforma única, pérdida datos, escalabilidad limitada | Plan migración gradual + backup cloud |
| Gap asistencia ADE | Media | Medio | 🟡 MEDIO | 69.2% vs 78.8% IOI, impacto en resultados | Programa mentorización específico |
| 18% no presentación | Baja | Bajo | 🟢 BAJO | Sesgo en métricas de rendimiento | Sistema recordatorios automáticos |
| Falta de integración | Alta | Medio | 🟡 MEDIO | Trabajo manual, errores humanos | Desarrollo APIs institucionales |
| Ausencia análisis predictivo | Media | Alto | 🟡 MEDIO | Decisiones reactivas vs proactivas | Implementación ML y BI |

### 7.2 Plan de Continuidad de Negocio

| Componente | Solución Actual | Nivel Protección | Mejora Requerida | Timeline |
|------------|-----------------|------------------|------------------|----------|
| Backup de datos | Manual, local | 🔴 Insuficiente | Automatización cloud | Q1 2025 |
| Documentación | Limitada | 🟡 Básica | Procedimientos completos | Q1 2025 |
| Recuperación | Sin procedimientos aparentes | 🔴 Crítico | RTO: 1h, RPO: 1h | Q2 2025 |

**Métricas objetivo de continuidad:**
• RTO (Recovery Time Objective): 1 hora máximo
• RPO (Recovery Point Objective): 1 hora máximo de pérdida de datos
• Disponibilidad del sistema: 99.9% (8.77 horas downtime/año)

## 8. CONCLUSIONES Y RECOMENDACIONES EJECUTIVAS

### 8.1 Fortalezas del Sistema Actual

| Aspecto | Evaluación | Detalles | Valor Estratégico |
|---------|------------|----------|-------------------|
| Arquitectura de datos | 🟢 Excelente | Separación clara responsabilidades, normalización | Alto |
| Cobertura de métricas | 🟢 Integral | Asistencia, rendimiento, demografía, grupos | Muy Alto |
| Automatización parcial | 🟡 Aceptable | Validaciones, cálculos, alertas básicas | Medio |
| Resultados académicos | 🟢 Excepcionales | 92.7% aprobados (+17.7% vs nacional) | Muy Alto |
| Usabilidad | 🟡 Funcional | Familiar para usuarios, curva aprendizaje baja | Medio |

### 8.2 Roadmap Estratégico con Hitos

| Fase | Período | Objetivos Clave |
|------|---------|-----------------|
| Fase 1 | Q1-Q2 2025 | Dashboard + Alertas + Métricas avanzadas |
| Fase 2 | Q3-Q4 2025 | Integración + Predictivo + Gamificación |
| Fase 3 | 2026 | BI Platform + ISO 21001 + Centro Excelencia |
| **TOTAL** | **24 meses** | **Transformación digital completa** |

## 9. INVERSIÓN Y ANÁLISIS FINANCIERO

### 9.1 Desglose de Inversión por Categoría

| Categoría | Descripción | % del Total | Prioridad |
|-----------|-------------|-------------|-----------|
| Desarrollo BI & Dashboard | Interface interactiva, reportes ejecutivos | 15.8% | 🔴 Alta |
| Integración de Sistemas | APIs, sincronización, conectores | 26.3% | 🔴 Alta |
| Análisis Predictivo & ML | Modelos IA, algoritmos, data science | 36.8% | 🟡 Media |
| Certificación & Calidad | ISO 21001, auditorías, compliance | 21.1% | 🟢 Baja |
| **TOTAL PROGRAMA** | - | **100%** | - |

## 10. MÉTRICAS DE ÉXITO Y SEGUIMIENTO

### 10.1 KPIs de Implementación del Proyecto

| Métrica | Línea Base Actual | Objetivo 6 meses | Objetivo 12 meses | Objetivo 24 meses |
|---------|-------------------|------------------|-------------------|-------------------|
| Tasa de asistencia promedio | 72.7% | 75% | 80% | 85% |
| Detección temprana riesgo | 0% | 70% | 85% | 95% |
| Satisfacción usuario sistema | N/A | 7.5/10 | 8.5/10 | 9.0/10 |
| Precisión predicciones | N/A | N/A | 80% | 90% |

### 10.2 Dashboard de Control Ejecutivo

| Área de Control | Indicador Clave | Frecuencia | Responsable |
|-----------------|-----------------|------------|-------------|
| Rendimiento Académico | Tasa aprobados por grado | Semanal | Director Académico |
| Asistencia | % asistencia por sesión | Diaria | Coordinador DSI |
| Riesgo Estudiantil | Alertas tempranas activadas | Tiempo real | Tutor Académico |
| Calidad del Sistema | Disponibilidad y errores | Continua | CTO |

### 10.3 Plan de Comunicación de Resultados

| Audiencia | Formato | Contenido | Frecuencia |
|-----------|---------|-----------|------------|
| Rectorado | Executive Summary | KPIs, ROI, decisiones estratégicas | Trimestral |
| Decanos | Dashboard interactivo | Rendimiento por facultad | Mensual |
| Profesores | Reportes operativos | Asistencia, participación estudiantes | Semanal |
| Estudiantes | Portal autoservicio | Progreso personal, ranking | Tiempo real |

## 11. ANÁLISIS DE RIESGOS DEL PROYECTO

### 11.1 Matriz de Riesgos de Implementación

| Riesgo | Probabilidad | Impacto | Puntuación | Mitigación | Responsable |
|--------|--------------|---------|------------|------------|-------------|
| Sobrecostes desarrollo | Media | Alto | 🟡 6 | Contratos precio fijo | PMO |
| Problemas integración | Media | Alto | 🟡 6 | Pruebas piloto | CTO |
| Pérdida datos migración | Baja | Muy Alto | 🟡 5 | Backup múltiple | Director SI |
| Falta adopción usuarios | Media | Medio | 🟢 4 | Formación intensiva | Director Académico |
