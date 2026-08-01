# Especificacion Funcional - Sistema de Gestion de Planificacion Estrategica

## 1. Proposito

Definir la estructura funcional del sistema requerido para administrar la planificacion estrategica del OTEC, asegurando integracion con el Sistema de Gestion de Calidad, trazabilidad documental, seguimiento de indicadores y evidencia para auditorias y revision por la direccion.

## 2. Objetivo del sistema

Disponer de una plataforma que permita:

- planificar estrategicamente cada periodo anual
- controlar objetivos, indicadores, metas y responsables
- consolidar resultados operativos y de calidad
- gestionar acciones correctivas y preventivas
- controlar documentos y registros
- preparar y evidenciar la revision por la direccion
- mantener trazabilidad auditables de decisiones, resultados y evidencias

## 3. Alcance funcional

El sistema cubrira los siguientes dominios:

- Planificacion estrategica anual
- Gestion de FODA
- Gestion de politica, mision y vision
- Gestion de objetivos e indicadores
- Seguimiento y tablero de control
- Revision por la direccion
- Acciones correctivas y preventivas
- Reclamos y no conformidades
- Control documental y de registros
- Gestion de evidencias
- Proyeccion financiera y flujo de caja
- Reportes de gestion y auditoria

## 4. Actores del negocio

### 4.1 Actores principales

- Representante Legal
- Representante de la Direccion
- Encargada Area Academica
- Encargado de area
- Administracion y Finanzas
- Auditor Interno
- Auditor Externo

### 4.2 Actores secundarios

- Relator o facilitador
- Cliente o empresa contratante
- Participante

## 5. Problemas actuales que el sistema debe resolver

- Informacion dispersa entre documentos, actas, encuestas, registros y planillas.
- Seguimiento manual de indicadores y metas.
- Trazabilidad limitada entre objetivo, resultado, evidencia y accion correctiva.
- Riesgo de uso de documentos obsoletos.
- Preparacion manual de revision por la direccion.
- Dificultad para consolidar evidencia ante auditorias y fiscalizaciones.
- Escasa visibilidad ejecutiva del cumplimiento del plan.

## 6. Procesos de negocio soportados

### 6.1 Macroproceso estrategico

1. Crear periodo anual.
2. Registrar FODA.
3. Definir politica, mision, vision y objetivos.
4. Asociar indicadores, metas, responsables y evidencias.
5. Aprobar plan.
6. Ejecutar seguimiento periodico.
7. Analizar desviaciones.
8. Abrir acciones correctivas o preventivas cuando corresponda.
9. Realizar revision por la direccion.
10. Cerrar periodo y dejar historial.

### 6.2 Macroproceso de control de calidad asociado

1. Registrar resultados de cursos, encuestas y reclamos.
2. Consolidar indicadores.
3. Registrar auditorias y hallazgos.
4. Gestionar no conformidades.
5. Dar seguimiento a acciones.
6. Generar reportes y evidencias.

### 6.3 Macroproceso documental

1. Crear documento controlado.
2. Revisar y aprobar.
3. Publicar version vigente.
4. Distribuir copia controlada.
5. Marcar version anterior como obsoleta.
6. Mantener listas maestras y retencion.

## 7. Modulos del sistema

### 7.1 Modulo de Planificacion Estrategica

Funciones:

- crear periodos
- configurar estados del plan
- registrar FODA
- administrar mision, vision y politica
- aprobar y cerrar plan

### 7.2 Modulo de Objetivos e Indicadores

Funciones:

- crear objetivos
- definir indicadores y formulas
- asignar metas y frecuencias
- vincular responsables
- asociar medios de verificacion

### 7.3 Modulo de Seguimiento

Funciones:

- cargar resultados
- adjuntar evidencias
- visualizar cumplimiento por semaforo
- emitir alertas por desviaciones
- mostrar tendencia historica

### 7.4 Modulo de Revision por la Direccion

Funciones:

- programar revision anual
- solicitar insumos a responsables
- consolidar entradas
- generar acta
- administrar acuerdos y seguimiento

### 7.5 Modulo de Acciones Correctivas y Preventivas

Funciones:

- registrar acciones AC/AP
- analizar causa
- asignar responsables y plazos
- verificar eficacia
- cerrar o reabrir acciones

### 7.6 Modulo de Reclamos y No Conformidades

Funciones:

- registrar reclamos
- registrar no conformidades
- clasificar impacto y origen
- escalar a AC/AP
- mantener evidencia y cierre

### 7.7 Modulo de Control Documental

Funciones:

- registrar documentos y registros
- versionar revisiones
- controlar vigencia
- generar listas maestras
- administrar obsolescencia

### 7.8 Modulo Financiero de Planificacion

Funciones:

- registrar proyeccion a 3 anos
- registrar presupuesto anual
- registrar flujo de caja mensual
- comparar plan versus real

### 7.9 Modulo de Reportes y Auditoria

Funciones:

- emitir reportes ejecutivos
- emitir reportes de auditoria
- exportar PDF y Excel
- consultar bitacora y trazabilidad

## 8. Flujo funcional principal

### Flujo 1. Creacion y aprobacion del plan anual

1. El Representante de la Direccion crea el periodo anual.
2. Registra FODA y definiciones estrategicas.
3. El Representante Legal y el Representante de la Direccion definen objetivos.
4. Se asocian indicadores, metas, responsables y evidencias.
5. El sistema valida campos obligatorios.
6. El Representante Legal aprueba el plan.
7. El sistema publica el plan como vigente.

### Flujo 2. Seguimiento del plan

1. Los responsables cargan resultados segun frecuencia.
2. El sistema calcula cumplimiento.
3. Se adjuntan evidencias.
4. Si existe desviacion, se genera alerta.
5. El responsable registra observaciones o propone accion.

### Flujo 3. Gestion de incumplimientos

1. Un indicador incumplido, reclamo, auditoria o no conformidad genera un caso.
2. El Representante de la Direccion evalua si corresponde AC o AP.
3. Se asignan responsables y plazos.
4. Se ejecutan acciones.
5. Se verifica eficacia.
6. Se cierra o reabre el caso.

### Flujo 4. Revision por la direccion

1. Se programa la revision anual.
2. El sistema solicita insumos a los responsables.
3. Se consolidan entradas obligatorias.
4. La direccion revisa resultados y brechas.
5. Se generan acuerdos, recursos y decisiones.
6. Se realiza seguimiento posterior.

## 9. Matriz de roles y permisos

| Modulo / Accion | Rep. Legal | Rep. Direccion | Enc. Academica | Enc. Area | Adm. Finanzas | Auditor |
|---|---|---|---|---|---|---|
| Crear periodo estrategico | A | E | C | - | - | - |
| Aprobar periodo | A | C | - | - | - | - |
| Registrar FODA | E | E | C | C | - | - |
| Definir objetivos e indicadores | A | E | C | C | C | - |
| Cargar mediciones | C | C | E | E | E | - |
| Ver tablero ejecutivo | A | A | C | C | C | C |
| Programar revision por direccion | A | E | C | C | C | - |
| Emitir acta de revision | A | E | C | - | C | - |
| Registrar AC/AP | A | E | C | C | - | C |
| Cerrar AC/AP | A | E | C | - | - | C |
| Registrar reclamos | C | E | E | C | - | C |
| Registrar no conformidades | C | E | E | C | - | C |
| Crear documento controlado | A | E | C | - | - | - |
| Aprobar documento | A | C | - | - | - | - |
| Administrar lista maestra | C | E | - | - | - | C |
| Registrar proyeccion financiera | A | C | - | - | E | - |
| Registrar flujo de caja | C | C | - | - | E | - |
| Emitir reportes de auditoria | C | E | C | C | C | E |

Leyenda:

- A: Aprueba
- E: Ejecuta
- C: Consulta o colabora
- -: Sin acceso

## 10. Reglas funcionales

### 10.1 Planificacion

- Cada periodo debe ser unico por ano.
- No puede aprobarse un plan sin objetivos, indicadores, metas y responsables.
- Solo un plan por ano puede estar vigente.

### 10.2 Indicadores

- Todo indicador debe tener frecuencia de medicion.
- Todo indicador debe tener responsable y medio de verificacion.
- El sistema debe identificar automaticamente incumplimientos.

### 10.3 Revision por la direccion

- Debe existir al menos una revision cada 12 meses.
- No debe cerrarse la revision si faltan entradas obligatorias.
- Todo acuerdo debe quedar con responsable y plazo.

### 10.4 Acciones correctivas y preventivas

- Toda accion debe indicar origen, causa, responsable y fecha compromiso.
- No puede cerrarse una accion sin verificacion de eficacia.
- Una accion puede derivar de indicador, auditoria, reclamo o revision.

### 10.5 Control documental

- Todo documento controlado debe tener codigo, revision, estado y aprobador.
- La nueva revision debe dejar obsoleta la version anterior.
- Debe conservarse historial de cambios.

### 10.6 Registros

- Los registros deben almacenarse al menos 3 anos.
- Debe existir lista maestra de registros.
- Toda evidencia debe indicar origen, fecha y responsable.

## 11. Datos maestros y transaccionales

### 11.1 Datos maestros

- usuarios
- roles
- areas
- tipos de objetivo
- tipos de indicador
- tipos de evidencia
- tipos de documento
- tipos de no conformidad
- tipos de accion AC/AP
- clientes
- cursos

### 11.2 Datos transaccionales

- periodos estrategicos
- items FODA
- objetivos
- indicadores
- mediciones
- evidencias
- revisiones por la direccion
- acuerdos
- reclamos
- no conformidades
- acciones correctivas/preventivas
- documentos y revisiones
- listas maestras
- proyecciones financieras
- movimientos de flujo de caja

## 12. Reportes requeridos

### 12.1 Reportes gerenciales

- cumplimiento general del plan
- cumplimiento por objetivo
- cumplimiento por responsable
- indicadores en alerta
- estado de acciones abiertas
- resumen anual de revision por la direccion

### 12.2 Reportes operativos

- mediciones pendientes
- documentos por vencer
- acciones por vencer
- reclamos abiertos
- no conformidades por tipo

### 12.3 Reportes de auditoria

- trazabilidad objetivo a evidencia
- historial de cambios documentales
- listado de registros con retencion
- acciones correctivas y eficacia
- insumos y acta de revision por la direccion

## 13. Requisitos no funcionales

- autenticacion por usuario y contrasena o integracion corporativa
- control de acceso por roles
- bitacora de auditoria inalterable
- respaldo de adjuntos y evidencias
- exportacion a PDF y Excel
- interfaz web responsiva
- buscador global por codigo, objetivo, curso, cliente o documento
- disponibilidad de historico por multiples anos
- resguardo de documentos obsoletos sin borrado logico indebido

## 14. Integraciones recomendadas

### Minimas

- carga manual de encuestas
- carga manual de resultados de cursos
- adjunto de actas, libros de clases y evidencias

### Deseables

- integracion con correo para alertas
- importacion masiva desde Excel
- repositorio documental centralizado
- futura integracion con plataformas SENCE o sistemas internos si existieran

## 15. Criterios de exito del proyecto

- 100% de los objetivos del periodo registrados en el sistema
- 100% de indicadores con responsable y evidencia definida
- reduccion del tiempo de preparacion de revision por la direccion
- disponibilidad inmediata de evidencia para auditorias
- control de vigencia documental sin duplicidades
- seguimiento oportuno de acciones correctivas y preventivas

## 16. Propuesta de implementacion por etapas

### Etapa 1. Base de cumplimiento

- periodos
- FODA
- objetivos
- indicadores
- mediciones
- tablero
- revision por la direccion
- AC/AP

### Etapa 2. Control y trazabilidad

- reclamos
- no conformidades
- control documental
- listas maestras
- reportes de auditoria

### Etapa 3. Gestion ampliada

- proyeccion financiera
- flujo de caja
- automatizaciones
- importaciones masivas

## 17. Riesgos de implementacion

- confundir el sistema con una planilla de KPI sin soporte documental.
- no definir responsables reales por indicador.
- no establecer una gobernanza clara para aprobaciones.
- cargar evidencia sin estandar minimo de calidad.
- no capacitar a los usuarios clave del SGC.

## 18. Recomendacion final de analisis

Antes de iniciar desarrollo, conviene levantar los siguientes artefactos:

- matriz RACI formal
- diccionario de datos
- mockups de pantalla
- reglas de negocio validadas por direccion
- calendario de medicion por indicador
- inventario de documentos y registros actuales

Con esto el proyecto queda en condiciones de pasar a diseno funcional detallado, seleccion de tecnologia o solicitud de propuesta a un proveedor.
