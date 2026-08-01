# Historias de Usuario para Sistema de Gestion de Planificacion Estrategica

## 1. Objetivo del documento

Definir una propuesta funcional para construir un sistema de gestion de planificacion estrategica alineado con el Sistema de Gestion de Calidad (SGC) del OTEC, tomando como base los documentos revisados de la carpeta y, principalmente:

- `Manual-de-Calidad 2025 Rev. 04.docx`
- `PLANIFICACION ESTRATEGICA Rev 03.docx`

## 2. Alcance propuesto del sistema

El sistema debe permitir planificar, ejecutar, controlar y evidenciar la gestion estrategica anual del OTEC, integrando:

- FODA
- Politica, mision, vision y objetivos de calidad
- Indicadores, metas, responsables y medios de verificacion
- Seguimiento de resultados
- Revision por la direccion
- Acciones correctivas y preventivas
- Gestion de reclamos y no conformidades
- Control documental y de registros
- Evidencia operativa vinculada a cursos, clientes y partes interesadas
- Proyeccion financiera y control de flujo de caja asociado a la planificacion

## 3. Hallazgos de negocio relevantes

Del analisis documental se observa que la planificacion estrategica no es un documento aislado; funciona como eje de control del SGC.

Necesidades de negocio detectadas:

- La direccion debe aprobar anualmente objetivos, indicadores, metas y responsables.
- Los resultados de cursos, encuestas, quejas, auditorias y acciones correctivas alimentan la revision de direccion.
- Si un objetivo no se cumple, debe generarse accion correctiva.
- La organizacion requiere trazabilidad documental y control de versiones.
- Existen obligaciones de conservacion de registros por al menos 3 anos.
- La organizacion necesita evidencias para auditorias internas, externas y fiscalizaciones.
- La planificacion considera recursos financieros proyectados a 3 anos.
- La informacion hoy aparece dispersa entre procedimientos, actas, registros y documentos de cursos.

## 4. Usuarios del sistema

- Representante Legal
- Representante de la Direccion
- Encargada Area Academica
- Encargados de area
- Auditor interno o externo autorizado
- Administracion y finanzas
- Relator o facilitador con acceso restringido
- Consulta ejecutiva de direccion

## 5. Modulos funcionales propuestos

- Administracion del periodo estrategico
- FODA y definiciones estrategicas
- Objetivos, indicadores y metas
- Seguimiento y tablero de control
- Revision por la direccion
- Acciones correctivas y preventivas
- No conformidades y reclamos
- Control documental
- Gestion de evidencias
- Proyeccion financiera
- Reportes y auditoria
- Seguridad, roles y trazabilidad

## 6. Backlog de historias de usuario

### Epic 1. Configuracion de la planificacion estrategica

**HU-01. Crear periodo de planificacion**

Como Representante de la Direccion
quiero crear un periodo anual de planificacion estrategica
para organizar objetivos, indicadores, responsables y resultados del ano.

Criterios de aceptacion:

- Permite crear periodos por ano.
- Cada periodo queda con estado: borrador, en revision, aprobado, cerrado.
- Solo usuarios autorizados pueden aprobar o cerrar el periodo.

**HU-02. Registrar FODA**

Como Representante Legal
quiero registrar fortalezas, oportunidades, debilidades y amenazas
para fundamentar las decisiones estrategicas del periodo.

Criterios de aceptacion:

- Permite cargar items FODA por categoria.
- Cada item puede tener responsable, fecha, observacion y evidencia.
- Debe quedar historial de cambios.

**HU-03. Mantener mision, vision y politica de calidad**

Como Representante Legal
quiero administrar la mision, vision y politica de calidad vigentes
para asegurar que la planificacion se alinee con la direccion institucional.

Criterios de aceptacion:

- Permite registrar texto, fecha de vigencia, revision y aprobador.
- El sistema conserva versiones anteriores como obsoletas.
- La version vigente debe identificarse claramente.

### Epic 2. Objetivos, indicadores y metas

**HU-04. Definir objetivos estrategicos y de calidad**

Como Representante Legal
quiero definir objetivos por periodo
para formalizar las prioridades del OTEC.

Criterios de aceptacion:

- Cada objetivo debe registrar descripcion, responsable, frecuencia y estado.
- El objetivo puede marcarse como estrategico, de calidad o ambos.
- No se puede aprobar el periodo sin al menos un objetivo.

**HU-05. Definir indicadores y formulas**

Como Representante de la Direccion
quiero asociar indicadores medibles a cada objetivo
para controlar su cumplimiento de manera objetiva.

Criterios de aceptacion:

- Cada indicador registra nombre, formula, unidad, frecuencia, meta y estandar.
- Se puede indicar fuente de datos y medio de verificacion.
- El sistema valida que cada objetivo tenga al menos un indicador.

**HU-06. Definir responsables y fuentes de evidencia**

Como Encargada Area Academica
quiero asignar responsables y registros fuente
para asegurar quien alimenta cada indicador y con que evidencia.

Criterios de aceptacion:

- Se pueden asociar responsables primario y secundario.
- Se pueden vincular registros como encuestas, libro de clases, reclamos, auditorias o actas.
- Debe visualizarse la trazabilidad desde el indicador a la evidencia.

**HU-07. Planificar acciones ante incumplimiento**

Como Representante de la Direccion
quiero definir acciones previstas ante el no cumplimiento de una meta
para reaccionar oportunamente ante desviaciones.

Criterios de aceptacion:

- Cada indicador puede tener accion preventiva predefinida.
- El sistema permite registrar umbrales de alerta.
- Si la meta queda incumplida, debe sugerir abrir accion correctiva.

### Epic 3. Seguimiento de resultados

**HU-08. Cargar resultados periodicos de indicadores**

Como Encargado de area
quiero registrar resultados por periodo de medicion
para hacer seguimiento al avance real de los objetivos.

Criterios de aceptacion:

- Permite registrar valor, fecha, comentario y evidencia adjunta.
- Debe distinguir entre dato preliminar y dato validado.
- Debe mostrar semaforizacion segun cumplimiento.

**HU-09. Integrar resultados desde cursos y encuestas**

Como Encargada Area Academica
quiero vincular resultados de encuestas, cursos ejecutados y quejas
para alimentar automaticamente indicadores de satisfaccion, ventas y calidad.

Criterios de aceptacion:

- Permite registrar cursos ejecutados con codigo SENCE o costo empresa.
- Permite capturar promedio de encuestas de participantes y clientes.
- Permite registrar numero de quejas por curso o periodo.

**HU-10. Visualizar tablero ejecutivo**

Como Representante Legal
quiero visualizar un tablero consolidado de cumplimiento
para tomar decisiones rapidas sobre el desempeno del SGC.

Criterios de aceptacion:

- Debe mostrar objetivos, indicadores, metas, resultado actual y tendencia.
- Debe filtrar por ano, proceso, responsable y estado.
- Debe destacar brechas, alertas y acciones pendientes.

### Epic 4. Revision por la direccion

**HU-11. Planificar revision por la direccion**

Como Representante de la Direccion
quiero programar la revision anual por la direccion
para cumplir con la exigencia del SGC y coordinar entradas, agenda y responsables.

Criterios de aceptacion:

- Permite definir fecha, agenda, responsables de insumos y estado.
- Debe generar recordatorios previos.
- Debe impedir cerrar la revision si faltan insumos obligatorios.

**HU-12. Consolidar entradas de revision**

Como Representante de la Direccion
quiero consolidar automaticamente las entradas de la revision
para evaluar objetivos, satisfaccion, auditorias, proveedores, acciones y finanzas.

Criterios de aceptacion:

- Debe incluir al menos los 12 elementos identificados en el procedimiento de revision por la direccion.
- Debe mostrar faltantes de informacion.
- Debe permitir comentarios y conclusiones por cada punto.

**HU-13. Emitir acta y acuerdos de revision**

Como Representante Legal
quiero dejar acta formal de la revision y sus acuerdos
para evidenciar decisiones, responsables, plazos y necesidades de recursos.

Criterios de aceptacion:

- Permite generar acta con version imprimible y exportable.
- Cada acuerdo debe tener responsable, fecha compromiso y estado.
- Los acuerdos deben pasar a seguimiento automatico.

### Epic 5. Acciones correctivas y preventivas

**HU-14. Registrar accion correctiva o preventiva**

Como Representante de la Direccion
quiero registrar acciones correctivas o preventivas
para tratar no conformidades reales o potenciales.

Criterios de aceptacion:

- Permite clasificar la accion como correctiva o preventiva.
- Debe registrar causa, analisis, accion inmediata, accion definitiva, responsable y plazo.
- Debe vincularse con objetivo, auditoria, reclamo o revision de direccion.

**HU-15. Hacer seguimiento de eficacia**

Como Representante de la Direccion
quiero verificar la implementacion y eficacia de cada accion
para asegurar mejora continua real.

Criterios de aceptacion:

- Cada accion debe tener estados: abierta, en ejecucion, verificada, cerrada.
- Debe registrar metodo de verificacion de eficacia.
- Si la eficacia no es satisfactoria, debe permitir reabrir o generar nueva accion.

### Epic 6. Reclamos y no conformidades

**HU-16. Registrar reclamos y quejas**

Como usuario autorizado
quiero registrar reclamos de clientes o participantes
para asegurar tratamiento formal y trazable.

Criterios de aceptacion:

- Permite registrar origen, fecha, curso asociado, descripcion, gravedad y responsable.
- Debe permitir clasificar si genera no conformidad.
- Debe poder derivarse a accion correctiva.

**HU-17. Registrar servicio no conforme**

Como Encargada Area Academica
quiero registrar incidentes operativos del servicio
para controlar desviaciones como documentacion incompleta, retrasos, materiales o evaluaciones tardias.

Criterios de aceptacion:

- Permite categorizar el tipo de no conformidad.
- Debe registrar medida de contencion, decision y cierre.
- Debe mantener evidencia para auditoria o fiscalizacion.

### Epic 7. Control documental y de registros

**HU-18. Administrar documentos controlados**

Como Representante de la Direccion
quiero administrar documentos del SGC con control de revision
para asegurar vigencia, aprobacion y distribucion controlada.

Criterios de aceptacion:

- Permite registrar codigo, nombre, revision, vigencia, aprobador y tipo documental.
- Debe diferenciar documento vigente y obsoleto.
- Debe conservar historial de cambios.

**HU-19. Mantener lista maestra de documentos y registros**

Como Representante de la Direccion
quiero contar con listas maestras actualizadas
para controlar copias, poseedores, tiempos de retencion y disposicion.

Criterios de aceptacion:

- Debe generar lista maestra de documentos.
- Debe generar lista maestra de registros.
- Debe registrar retencion minima de 3 anos.

**HU-20. Gestionar distribucion y obsolescencia**

Como Representante de la Direccion
quiero distribuir nuevas versiones y retirar versiones obsoletas
para evitar uso no intencionado de documentos vencidos.

Criterios de aceptacion:

- Debe registrar fecha de distribucion y destinatarios.
- Debe marcar automaticamente la revision anterior como obsoleta.
- Debe mantener trazabilidad de retiro o archivo.

### Epic 8. Gestion financiera de la planificacion

**HU-21. Registrar proyeccion financiera a 3 anos**

Como Representante Legal
quiero registrar presupuesto y proyeccion financiera plurianual
para respaldar la viabilidad de la estrategia.

Criterios de aceptacion:

- Debe permitir proyectar ingresos, costos y resultados por 3 anos.
- Debe identificar responsable y fecha de aprobacion.
- Debe quedar asociada al periodo estrategico.

**HU-22. Registrar flujo de caja anual**

Como Administracion y Finanzas
quiero registrar el flujo de caja mensual
para monitorear disponibilidad financiera frente a la ejecucion del plan.

Criterios de aceptacion:

- Debe permitir ingresar items mensuales por concepto.
- Debe mostrar variaciones plan versus real.
- Debe generar alertas por desbalance relevante.

### Epic 9. Reportabilidad y auditoria

**HU-23. Emitir reportes de cumplimiento**

Como Representante Legal
quiero emitir reportes ejecutivos y de auditoria
para presentar evidencia ante direccion, certificacion o fiscalizacion.

Criterios de aceptacion:

- Debe exportar reportes en PDF y Excel.
- Debe incluir objetivos, indicadores, resultados, acciones y evidencias.
- Debe permitir reportes por periodo, proceso y responsable.

**HU-24. Consultar trazabilidad completa**

Como Auditor Interno
quiero rastrear desde un objetivo hasta sus evidencias y acciones derivadas
para verificar cumplimiento y consistencia del sistema.

Criterios de aceptacion:

- Debe navegar de objetivo a indicador, medicion, evidencia, no conformidad y accion.
- Debe mostrar usuario, fecha y cambio realizado.
- Debe mantener bitacora inalterable de auditoria.

### Epic 10. Seguridad y gobierno del sistema

**HU-25. Gestionar perfiles y permisos**

Como administrador del sistema
quiero asignar permisos por rol
para proteger informacion sensible y asegurar segregacion de funciones.

Criterios de aceptacion:

- Debe existir control de acceso por rol.
- La aprobacion de documentos y periodos debe restringirse a perfiles autorizados.
- El sistema debe registrar toda accion critica en bitacora.

**HU-26. Gestionar alertas y vencimientos**

Como Representante de la Direccion
quiero recibir alertas de revisiones, mediciones, acciones y documentos por vencer
para evitar incumplimientos del SGC.

Criterios de aceptacion:

- Debe alertar por indicadores sin actualizar.
- Debe alertar por acciones vencidas.
- Debe alertar por revision anual pendiente y documentos por actualizar.

## 7. Priorizacion recomendada

### MVP - Fase 1

- HU-01 Crear periodo de planificacion
- HU-02 Registrar FODA
- HU-04 Definir objetivos estrategicos y de calidad
- HU-05 Definir indicadores y formulas
- HU-06 Definir responsables y fuentes de evidencia
- HU-08 Cargar resultados periodicos
- HU-10 Visualizar tablero ejecutivo
- HU-11 Planificar revision por la direccion
- HU-12 Consolidar entradas de revision
- HU-13 Emitir acta y acuerdos
- HU-14 Registrar accion correctiva o preventiva
- HU-15 Hacer seguimiento de eficacia
- HU-18 Administrar documentos controlados
- HU-25 Gestionar perfiles y permisos
- HU-26 Gestionar alertas y vencimientos

### Fase 2

- HU-03 Mantener mision, vision y politica de calidad
- HU-07 Planificar acciones ante incumplimiento
- HU-09 Integrar resultados desde cursos y encuestas
- HU-16 Registrar reclamos y quejas
- HU-17 Registrar servicio no conforme
- HU-19 Mantener lista maestra de documentos y registros
- HU-20 Gestionar distribucion y obsolescencia
- HU-23 Emitir reportes de cumplimiento
- HU-24 Consultar trazabilidad completa

### Fase 3

- HU-21 Registrar proyeccion financiera a 3 anos
- HU-22 Registrar flujo de caja anual

## 8. Requisitos no funcionales minimos

- Trazabilidad total de cambios por usuario, fecha y hora.
- Control de versiones documentales.
- Respaldo digital de evidencias y adjuntos.
- Exportacion a PDF y Excel.
- Busqueda por periodo, objetivo, indicador, curso, cliente y responsable.
- Seguridad por roles.
- Bitacora auditable no editable por usuarios finales.
- Disponibilidad para conservar registros al menos 3 anos.

## 9. Entidades de informacion recomendadas

- Periodo estrategico
- FODA
- Politica de calidad
- Mision
- Vision
- Objetivo
- Indicador
- Meta
- Medicion
- Evidencia
- Revision por la direccion
- Acuerdo de revision
- Accion correctiva/preventiva
- Reclamo
- No conformidad
- Documento controlado
- Registro controlado
- Curso
- Cliente
- Encuesta
- Proyeccion financiera
- Flujo de caja
- Usuario
- Rol

## 10. Reglas de negocio clave

- No debe aprobarse un periodo sin objetivos, indicadores, metas y responsables.
- Todo objetivo incumplido debe permitir apertura de accion correctiva.
- La revision por la direccion debe ejecutarse al menos una vez cada 12 meses.
- Todo documento controlado debe tener revision, aprobador y estado de vigencia.
- Las revisiones anteriores deben quedar como obsoletas y trazables.
- Los registros deben conservarse al menos 3 anos.
- Las quejas y no conformidades deben poder derivarse a acciones correctivas.
- Los indicadores deben poder alimentarse con informacion de cursos, encuestas, reclamos, auditorias y finanzas.

## 11. Recomendacion de implementacion

Se recomienda construir el sistema con enfoque en cumplimiento y evidencia, no solo como tablero gerencial. En estos documentos, la planificacion estrategica opera como un registro rector del SGC; por eso el producto debe priorizar:

- trazabilidad
- control documental
- evidencia auditable
- seguimiento de acciones
- integracion con resultados operativos de cursos

Si el sistema se desarrolla solo como modulo de KPI, quedaria corto frente a los requisitos reales observados en los procedimientos revisados.

## 12. Trazabilidad documental usada para esta propuesta

- Manual de Calidad: compromiso de direccion, planificacion estrategica, objetivos de calidad, revision por la direccion, satisfaccion del cliente, auditoria, acciones correctivas, control del servicio no conforme, control documental.
- Planificacion Estrategica: FODA, objetivos, indicadores, metas, registros, resultados, proyeccion financiera y flujo de caja.
- PROC 01: planificacion financiera, ejecucion del curso, encuestas y cierre.
- PROC 02: programacion y contenido de la revision por la direccion.
- PROC 03: diseno y validacion de cursos, evidencia y relacion con satisfaccion.
- PROC 04: origen, aprobacion, seguimiento y eficacia de acciones correctivas y preventivas.
- PROC 05: auditorias internas, hallazgos y seguimiento.
- PROC 09: reclamos y servicios no conformes.
- PROC 11: control documental, listas maestras, revisiones y retencion.

## 13. Siguiente nivel sugerido

Como siguiente paso de analisis funcional, conviene desarrollar:

- mapa de procesos del sistema
- matriz de roles y permisos
- backlog refinado con prioridad MoSCoW
- mockups de pantallas
- modelo de datos logico
- casos de uso o criterios BDD para desarrollo
