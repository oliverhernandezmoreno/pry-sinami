# Documento de Requerimientos Funcionales

## 1. Identificacion

- Nombre del proyecto: Sistema de Gestion de Planificacion Estrategica
- Organizacion: OTEC
- Tipo de documento: Requerimientos funcionales
- Proposito: Base para analisis detallado, cotizacion, licitacion o desarrollo

## 2. Objetivo general

Construir un sistema web que permita administrar la planificacion estrategica anual del OTEC, integrada con los procesos del Sistema de Gestion de Calidad, para asegurar control, seguimiento, evidencia, trazabilidad y soporte a auditorias y revision por la direccion.

## 3. Objetivos especificos

- Centralizar la informacion estrategica del periodo.
- Gestionar objetivos, indicadores, metas y responsables.
- Consolidar evidencias operativas, documentales y de calidad.
- Gestionar acciones correctivas, preventivas, reclamos y no conformidades.
- Administrar documentos controlados y registros del sistema.
- Facilitar la revision por la direccion y la toma de decisiones.
- Proveer reportes ejecutivos y auditables.

## 4. Alcance funcional del producto

El sistema debera considerar como minimo los siguientes modulos:

- Planificacion estrategica
- FODA
- Politica, mision y vision
- Objetivos, indicadores y metas
- Seguimiento y tablero
- Revision por la direccion
- Acciones correctivas y preventivas
- Reclamos y no conformidades
- Control documental y listas maestras
- Evidencias y adjuntos
- Proyeccion financiera y flujo de caja
- Reportes y bitacora de auditoria

## 5. Alcance no incluido inicialmente

- Integracion directa con sistemas externos de SENCE
- Portal autoservicio para clientes externos
- Aplicacion movil nativa
- Analitica avanzada con inteligencia artificial

## 6. Perfiles de usuario

- Administrador del sistema
- Representante Legal
- Representante de la Direccion
- Encargada Area Academica
- Encargados de area
- Administracion y Finanzas
- Auditor interno
- Auditor externo en modo consulta

## 7. Requerimientos funcionales por modulo

### 7.1 Modulo de autenticacion y seguridad

**RF-001** El sistema debe permitir autenticacion de usuarios mediante credenciales.

**RF-002** El sistema debe permitir administrar perfiles y permisos por rol.

**RF-003** El sistema debe registrar en bitacora las acciones criticas de creacion, actualizacion, aprobacion, cierre y eliminacion logica.

**RF-004** El sistema debe impedir el acceso a funciones no autorizadas segun el rol del usuario.

### 7.2 Modulo de planificacion estrategica

**RF-005** El sistema debe permitir crear un periodo anual de planificacion.

**RF-006** El sistema debe manejar estados del periodo: borrador, en revision, aprobado y cerrado.

**RF-007** El sistema debe permitir registrar descripcion general del periodo, responsable, fechas y observaciones.

**RF-008** El sistema debe validar que solo exista un plan vigente por ano.

**RF-009** El sistema debe permitir aprobar formalmente el plan por usuarios autorizados.

### 7.3 Modulo FODA

**RF-010** El sistema debe permitir registrar fortalezas, oportunidades, debilidades y amenazas.

**RF-011** Cada item FODA debe permitir registrar responsable, fecha, comentarios y evidencia.

**RF-012** El sistema debe mantener historial de modificaciones de cada item FODA.

### 7.4 Modulo de politica, mision y vision

**RF-013** El sistema debe permitir mantener la politica de calidad vigente.

**RF-014** El sistema debe permitir mantener mision y vision institucional.

**RF-015** Cada definicion debe mantener version, fecha de vigencia, aprobador y estado.

**RF-016** El sistema debe conservar versiones obsoletas para trazabilidad.

### 7.5 Modulo de objetivos, indicadores y metas

**RF-017** El sistema debe permitir crear objetivos estrategicos y de calidad asociados a un periodo.

**RF-018** Cada objetivo debe registrar descripcion, tipo, responsable, frecuencia de seguimiento y estado.

**RF-019** El sistema debe permitir asociar uno o mas indicadores a cada objetivo.

**RF-020** Cada indicador debe registrar nombre, formula, unidad, meta, estandar, frecuencia y medio de verificacion.

**RF-021** El sistema debe permitir asignar responsable primario y secundario por indicador.

**RF-022** El sistema debe impedir aprobar el plan si un objetivo no tiene al menos un indicador.

**RF-023** El sistema debe permitir registrar umbrales de alerta por indicador.

### 7.6 Modulo de seguimiento y mediciones

**RF-024** El sistema debe permitir registrar mediciones periodicas por indicador.

**RF-025** Cada medicion debe registrar valor, fecha, comentario, responsable y evidencia asociada.

**RF-026** El sistema debe distinguir mediciones preliminares y validadas.

**RF-027** El sistema debe calcular automaticamente el nivel de cumplimiento respecto de la meta.

**RF-028** El sistema debe mostrar semaforizacion de cumplimiento.

**RF-029** El sistema debe generar alertas cuando un indicador este fuera de rango o sin actualizar.

**RF-030** El sistema debe mantener historial de mediciones por periodo.

### 7.7 Modulo de cursos, encuestas y fuentes operativas

**RF-031** El sistema debe permitir registrar cursos ejecutados asociados al periodo.

**RF-032** El sistema debe permitir clasificar cursos con codigo SENCE o costo empresa.

**RF-033** El sistema debe permitir registrar cantidad de participantes, aprobados, reprobados y datos relevantes del curso.

**RF-034** El sistema debe permitir registrar resultados de encuestas de participantes.

**RF-035** El sistema debe permitir registrar resultados de encuestas de clientes.

**RF-036** El sistema debe permitir asociar esta informacion a indicadores del plan.

### 7.8 Modulo de revision por la direccion

**RF-037** El sistema debe permitir programar la revision por la direccion al menos una vez cada 12 meses.

**RF-038** El sistema debe permitir definir agenda, fecha, responsables de insumos y estado de la revision.

**RF-039** El sistema debe consolidar entradas para la revision, incluyendo objetivos, satisfaccion, auditorias, proveedores, AC/AP, cambios, recursos y finanzas.

**RF-040** El sistema debe alertar cuando existan entradas obligatorias pendientes.

**RF-041** El sistema debe permitir generar acta de revision por la direccion.

**RF-042** El sistema debe permitir registrar acuerdos, responsables, plazos y estado de cumplimiento.

### 7.9 Modulo de acciones correctivas y preventivas

**RF-043** El sistema debe permitir registrar acciones correctivas y preventivas.

**RF-044** Cada accion debe registrar origen, descripcion de la situacion, analisis de causa, accion inmediata, accion definitiva, responsable y plazo.

**RF-045** El sistema debe permitir vincular una accion a objetivo, indicador, reclamo, auditoria, no conformidad o revision de direccion.

**RF-046** El sistema debe manejar estados de la accion: abierta, en ejecucion, verificada y cerrada.

**RF-047** El sistema debe permitir registrar verificacion de eficacia.

**RF-048** El sistema debe permitir reabrir una accion si la eficacia no fue satisfactoria.

### 7.10 Modulo de reclamos y no conformidades

**RF-049** El sistema debe permitir registrar reclamos de clientes o participantes.

**RF-050** El sistema debe permitir clasificar el reclamo por tipo, gravedad, curso asociado y estado.

**RF-051** El sistema debe permitir registrar no conformidades del servicio o del SGC.

**RF-052** El sistema debe permitir registrar medidas de contencion, decisiones y evidencias.

**RF-053** El sistema debe permitir escalar reclamos y no conformidades a AC/AP.

### 7.11 Modulo de control documental

**RF-054** El sistema debe permitir registrar documentos controlados del SGC.

**RF-055** Cada documento debe registrar codigo, nombre, tipo, revision, aprobador, fecha de vigencia y estado.

**RF-056** El sistema debe permitir gestionar nuevas revisiones documentales.

**RF-057** El sistema debe marcar la revision anterior como obsoleta al publicar una nueva version.

**RF-058** El sistema debe permitir registrar distribucion de copias controladas.

**RF-059** El sistema debe permitir administrar lista maestra de documentos.

**RF-060** El sistema debe permitir administrar lista maestra de registros.

**RF-061** El sistema debe registrar tiempo de retencion y disposicion de registros.

### 7.12 Modulo de evidencias y adjuntos

**RF-062** El sistema debe permitir adjuntar archivos a objetivos, indicadores, mediciones, revisiones, acciones, reclamos y documentos.

**RF-063** Cada evidencia debe registrar origen, tipo, fecha, usuario y observacion.

**RF-064** El sistema debe permitir consultar evidencia relacionada desde cualquier proceso vinculado.

### 7.13 Modulo financiero

**RF-065** El sistema debe permitir registrar proyeccion financiera a 3 anos.

**RF-066** El sistema debe permitir registrar presupuesto anual por item.

**RF-067** El sistema debe permitir registrar flujo de caja mensual.

**RF-068** El sistema debe permitir comparar plan versus real.

**RF-069** El sistema debe generar alertas por desviaciones financieras relevantes.

### 7.14 Modulo de reportes

**RF-070** El sistema debe permitir emitir reportes ejecutivos de cumplimiento del plan.

**RF-071** El sistema debe permitir emitir reportes por objetivo, indicador, responsable y periodo.

**RF-072** El sistema debe permitir emitir reportes de auditoria con trazabilidad completa.

**RF-073** El sistema debe exportar reportes a PDF y Excel.

### 7.15 Modulo de bitacora y trazabilidad

**RF-074** El sistema debe registrar bitacora de auditoria de toda accion critica.

**RF-075** El sistema debe permitir consultar historial de cambios por entidad.

**RF-076** El sistema debe permitir rastrear desde un objetivo hasta sus evidencias, acciones y acuerdos relacionados.

## 8. Reglas de negocio

**RN-001** No puede existir mas de un plan vigente por ano.

**RN-002** No puede aprobarse un plan sin objetivos, indicadores, metas y responsables.

**RN-003** Todo indicador debe tener frecuencia y medio de verificacion.

**RN-004** Todo acuerdo de revision por la direccion debe tener responsable y plazo.

**RN-005** Toda accion correctiva o preventiva debe tener origen y verificacion de eficacia.

**RN-006** Toda nueva revision documental debe obsoletar la anterior.

**RN-007** Los registros deben poder conservarse por al menos 3 anos.

**RN-008** Un reclamo o no conformidad puede derivar en una o mas acciones correctivas.

## 9. Requerimientos no funcionales

**RNF-001** El sistema debe ser web y accesible desde navegadores modernos.

**RNF-002** El sistema debe contar con control de acceso por roles.

**RNF-003** El sistema debe mantener bitacora auditable inalterable.

**RNF-004** El sistema debe soportar carga y descarga de documentos adjuntos.

**RNF-005** El sistema debe permitir busqueda por codigo, nombre, objetivo, curso, cliente o documento.

**RNF-006** El sistema debe mantener historico de informacion por multiples anos.

**RNF-007** El sistema debe resguardar versiones obsoletas sin exponerlas como vigentes.

## 10. Casos de uso minimos del MVP

- CU-01 Crear plan anual
- CU-02 Definir objetivos e indicadores
- CU-03 Registrar medicion
- CU-04 Visualizar tablero ejecutivo
- CU-05 Programar revision por la direccion
- CU-06 Emitir acta de revision
- CU-07 Abrir accion correctiva
- CU-08 Verificar eficacia de accion
- CU-09 Publicar documento controlado
- CU-10 Emitir reporte de auditoria

## 11. Criterios de aceptacion global del MVP

- El plan anual puede crearse, aprobarse y cerrarse.
- Todo objetivo del MVP tiene al menos un indicador y un responsable.
- El sistema muestra cumplimiento visual por indicador.
- La revision por la direccion puede ejecutarse y generar acuerdos.
- Las acciones correctivas pueden abrirse, seguirse y cerrarse con evidencia.
- Los documentos controlados pueden versionarse y marcarse como obsoletos.
- Se pueden emitir reportes ejecutivos y de auditoria.

## 12. Entregables esperados del desarrollo

- aplicacion web operativa
- base de datos del sistema
- perfiles y permisos configurados
- reportes base
- documentacion tecnica
- manual de usuario
- capacitacion a usuarios clave
- plan de respaldo y continuidad operativa

## 13. Consideraciones para cotizacion

El proveedor o equipo de desarrollo debera estimar al menos:

- esfuerzo de analisis funcional detallado
- esfuerzo de UX/UI
- esfuerzo de desarrollo frontend y backend
- esfuerzo de base de datos
- esfuerzo de pruebas
- esfuerzo de despliegue
- esfuerzo de capacitacion
- tiempo de garantia y soporte posterior
