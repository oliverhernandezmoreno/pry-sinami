# Plan de Proyecto - Sistema de Gestion de Planificacion Estrategica

## 1. Objetivo del plan

Proponer una hoja de ruta de implementacion para construir e implantar el sistema de gestion de planificacion estrategica del OTEC, desde la definicion funcional hasta la puesta en marcha.

## 2. Enfoque general

Se recomienda ejecutar el proyecto por etapas, priorizando primero el cumplimiento del SGC y la trazabilidad minima exigible, antes de automatizaciones avanzadas o integraciones.

## 3. Supuestos base

- Existe patrocinio de la direccion.
- El OTEC designara usuarios clave para validacion funcional.
- La informacion documental actual sera insumo para parametrizacion y migracion.
- El desarrollo puede ser propio o tercerizado.

## 4. Fases del proyecto

### Fase 0. Inicio y preparacion

Objetivo:

Formalizar el proyecto, su alcance y responsables.

Actividades:

- nombrar sponsor y contraparte funcional
- designar usuarios clave
- validar alcance inicial
- definir objetivos del proyecto
- aprobar plan de trabajo

Entregables:

- acta de inicio
- alcance validado
- equipo de proyecto definido

### Fase 1. Levantamiento y validacion funcional

Objetivo:

Confirmar requerimientos y reglas de negocio antes del diseno tecnico.

Actividades:

- revisar documentos base del SGC
- validar historias de usuario
- validar requerimientos funcionales
- validar matriz RACI
- confirmar roles y permisos
- definir criterios de exito

Entregables:

- documento funcional aprobado
- backlog priorizado
- matriz de roles validada

### Fase 2. Diseno funcional y tecnico

Objetivo:

Preparar la solucion para construccion.

Actividades:

- elaborar mockups definitivos
- definir modelo de datos fisico
- definir arquitectura de la solucion
- definir estrategia de seguridad
- definir reportes del MVP
- definir estrategia de migracion documental

Entregables:

- mockups aprobados
- arquitectura tecnica
- modelo de datos
- especificacion de integraciones

### Fase 3. Desarrollo MVP

Objetivo:

Construir la primera version operativa del sistema.

Modulos sugeridos del MVP:

- autenticacion y roles
- planificacion estrategica
- objetivos e indicadores
- seguimiento y tablero
- revision por la direccion
- acciones correctivas/preventivas
- reportes base

Actividades:

- configuracion de ambientes
- desarrollo backend
- desarrollo frontend
- pruebas unitarias
- pruebas de integracion

Entregables:

- MVP desplegable
- base de datos inicial
- documentacion tecnica base

### Fase 4. Desarrollo complementario

Objetivo:

Incorporar modulos de control y cumplimiento ampliado.

Modulos sugeridos:

- reclamos y no conformidades
- control documental
- listas maestras
- bitacora de auditoria
- reportes de auditoria
- modulo financiero

Entregables:

- version ampliada del sistema
- funciones de trazabilidad completa

### Fase 5. Pruebas funcionales y aceptacion

Objetivo:

Validar que el sistema responde a los procesos reales del OTEC.

Actividades:

- pruebas funcionales por modulo
- pruebas integrales por proceso
- pruebas de perfiles y permisos
- pruebas de reportes
- correccion de incidencias
- aceptacion por usuario clave

Entregables:

- plan de pruebas
- evidencias de prueba
- acta de aceptacion

### Fase 6. Capacitacion y puesta en marcha

Objetivo:

Dejar el sistema operando con usuarios entrenados.

Actividades:

- capacitacion a direccion
- capacitacion a responsables operativos
- carga inicial de catalogos y parametros
- migracion inicial de documentos y datos base
- salida a produccion
- soporte de estabilizacion

Entregables:

- manual de usuario
- manual administrador
- sistema en produccion
- plan de soporte inicial

## 5. Cronograma referencial

Estimacion orientativa para un proyecto mediano:

- Fase 0: 1 semana
- Fase 1: 2 a 3 semanas
- Fase 2: 2 a 4 semanas
- Fase 3: 6 a 10 semanas
- Fase 4: 4 a 8 semanas
- Fase 5: 2 a 3 semanas
- Fase 6: 1 a 2 semanas

Duracion total estimada:

- entre 18 y 31 semanas, segun alcance, equipo e integraciones

## 6. Dependencias criticas

- aprobacion temprana de alcance funcional
- disponibilidad de usuarios clave para validaciones
- definicion de roles reales del OTEC
- definicion de infraestructura tecnologica
- disponibilidad de repositorio documental y datos historicos

## 7. Riesgos principales

### Riesgos funcionales

- cambios de alcance durante el desarrollo
- diferencias entre procedimiento documentado y operacion real
- falta de validacion oportuna por usuarios clave

### Riesgos tecnicos

- subestimar complejidad del control documental
- baja calidad de datos historicos
- falta de estandar en evidencias y archivos adjuntos

### Riesgos de adopcion

- resistencia al cambio
- uso parcial del sistema
- mantencion de controles paralelos en planillas

## 8. Medidas de mitigacion

- aprobar backlog y requerimientos antes del desarrollo
- realizar demos funcionales por sprint o fase
- designar un duenio funcional del sistema
- definir politica de carga de evidencias y calidad de datos
- ejecutar capacitacion por perfil de usuario

## 9. Roles sugeridos del proyecto

### Cliente / negocio

- Sponsor: Representante Legal
- Dueno funcional: Representante de la Direccion
- Referente operativo: Encargada Area Academica
- Referente financiero: Administracion y Finanzas

### Equipo de implementacion

- jefe de proyecto
- analista funcional
- arquitecto o lider tecnico
- desarrollador backend
- desarrollador frontend
- QA o responsable de pruebas
- especialista de datos o DBA

## 10. Entregables minimos exigibles a un proveedor

- plan de proyecto detallado
- analisis funcional validado
- diseno UX/UI
- arquitectura tecnica
- desarrollo del sistema
- pruebas documentadas
- manuales
- capacitacion
- garantia y soporte post salida

## 11. Indicadores de exito del proyecto

- porcentaje de modulos implementados segun alcance
- porcentaje de casos de prueba aprobados
- porcentaje de objetivos migrados al sistema
- porcentaje de usuarios clave capacitados
- tiempo de preparacion de revision por la direccion antes y despues
- tiempo de busqueda de evidencia para auditoria antes y despues

## 12. Recomendacion de estrategia de contratacion

Si el desarrollo sera tercerizado, conviene solicitar propuesta en dos etapas:

1. etapa de analisis y diseno detallado
2. etapa de construccion e implementacion

Esto reduce riesgo, mejora la estimacion real y permite ajustar el alcance del MVP antes de comprometer el desarrollo completo.
