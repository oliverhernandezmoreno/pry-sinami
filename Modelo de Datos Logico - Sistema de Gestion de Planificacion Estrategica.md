# Modelo de Datos Logico - Sistema de Gestion de Planificacion Estrategica

## 1. Objetivo

Definir las entidades principales, sus atributos clave y relaciones logicas para soportar el sistema de gestion de planificacion estrategica y su integracion con el SGC.

## 2. Principios de modelado

- Un periodo estrategico es la entidad eje del sistema.
- La trazabilidad debe permitir navegar desde objetivo a evidencia.
- El modelo debe soportar historial, versionamiento y auditoria.
- Los procesos de calidad deben vincularse con la estrategia.

## 3. Entidades maestras

### 3.1 Usuario

Atributos clave:

- id_usuario
- nombres
- apellidos
- correo
- cargo
- estado
- fecha_creacion

### 3.2 Rol

Atributos clave:

- id_rol
- nombre_rol
- descripcion
- estado

### 3.3 UsuarioRol

Atributos clave:

- id_usuario_rol
- id_usuario
- id_rol
- fecha_asignacion
- estado

### 3.4 Area

Atributos clave:

- id_area
- nombre_area
- descripcion
- responsable_area
- estado

### 3.5 Cliente

Atributos clave:

- id_cliente
- razon_social
- rut
- tipo_cliente
- contacto_principal
- correo
- telefono
- estado

### 3.6 Curso

Atributos clave:

- id_curso
- nombre_curso
- codigo_sence
- tipo_curso
- modalidad
- estado

### 3.7 TipoDocumento

Atributos clave:

- id_tipo_documento
- nombre_tipo
- descripcion

### 3.8 TipoEvidencia

Atributos clave:

- id_tipo_evidencia
- nombre_tipo
- descripcion

### 3.9 TipoNoConformidad

Atributos clave:

- id_tipo_nc
- nombre_tipo
- descripcion

### 3.10 TipoAccion

Atributos clave:

- id_tipo_accion
- nombre_tipo
- descripcion

## 4. Entidades estrategicas

### 4.1 PeriodoEstrategico

Atributos clave:

- id_periodo
- anio
- nombre_periodo
- fecha_inicio
- fecha_termino
- estado
- objetivo_general
- id_usuario_creador
- id_usuario_aprobador
- fecha_aprobacion

### 4.2 FODAItem

Atributos clave:

- id_foda
- id_periodo
- categoria_foda
- descripcion
- id_responsable
- fecha_registro
- estado

### 4.3 PoliticaCalidad

Atributos clave:

- id_politica
- version
- contenido
- fecha_vigencia
- estado
- id_aprobador

### 4.4 Mision

Atributos clave:

- id_mision
- version
- contenido
- fecha_vigencia
- estado
- id_aprobador

### 4.5 Vision

Atributos clave:

- id_vision
- version
- contenido
- fecha_vigencia
- estado
- id_aprobador

### 4.6 Objetivo

Atributos clave:

- id_objetivo
- id_periodo
- codigo_objetivo
- descripcion
- tipo_objetivo
- frecuencia_seguimiento
- id_responsable
- estado

### 4.7 Indicador

Atributos clave:

- id_indicador
- id_objetivo
- nombre_indicador
- formula
- unidad_medida
- frecuencia_medicion
- meta
- estandar
- umbral_alerta
- id_responsable_primario
- id_responsable_secundario
- medio_verificacion
- estado

### 4.8 MedicionIndicador

Atributos clave:

- id_medicion
- id_indicador
- periodo_medicion
- fecha_medicion
- valor_obtenido
- porcentaje_cumplimiento
- tipo_registro
- comentario
- id_usuario_registra
- validado
- fecha_validacion
- id_usuario_valida

## 5. Entidades de revision y seguimiento

### 5.1 RevisionDireccion

Atributos clave:

- id_revision
- id_periodo
- fecha_programada
- fecha_realizacion
- estado
- agenda
- observaciones_generales
- id_responsable

### 5.2 RevisionEntrada

Atributos clave:

- id_revision_entrada
- id_revision
- tipo_entrada
- descripcion
- estado
- responsable_insumo
- fecha_entrega
- observacion

### 5.3 AcuerdoRevision

Atributos clave:

- id_acuerdo
- id_revision
- descripcion
- id_responsable
- fecha_compromiso
- estado
- resultado

## 6. Entidades de calidad

### 6.1 AccionCorrectivaPreventiva

Atributos clave:

- id_accion
- id_tipo_accion
- origen_accion
- descripcion_situacion
- analisis_causa
- accion_inmediata
- accion_definitiva
- metodologia_verificacion
- id_responsable
- fecha_apertura
- fecha_compromiso
- fecha_cierre
- estado
- eficaz

### 6.2 Reclamo

Atributos clave:

- id_reclamo
- fecha_reclamo
- origen_reclamo
- id_cliente
- id_curso
- descripcion
- gravedad
- estado
- id_responsable

### 6.3 NoConformidad

Atributos clave:

- id_nc
- id_tipo_nc
- fecha_deteccion
- origen_nc
- id_curso
- descripcion
- medida_contencion
- estado
- id_responsable

### 6.4 Auditoria

Atributos clave:

- id_auditoria
- tipo_auditoria
- fecha_programada
- fecha_realizacion
- alcance
- auditor_asignado
- estado
- informe

### 6.5 HallazgoAuditoria

Atributos clave:

- id_hallazgo
- id_auditoria
- tipo_hallazgo
- descripcion
- evidencia
- estado
- requiere_accion

## 7. Entidades operativas vinculadas a indicadores

### 7.1 EjecucionCurso

Atributos clave:

- id_ejecucion
- id_curso
- id_cliente
- fecha_inicio
- fecha_termino
- tipo_ejecucion
- cantidad_participantes
- participantes_aprobados
- participantes_reprobados
- lugar_ejecucion
- estado

### 7.2 EncuestaParticipante

Atributos clave:

- id_encuesta_participante
- id_ejecucion
- fecha_aplicacion
- promedio_resultado
- observaciones

### 7.3 EncuestaCliente

Atributos clave:

- id_encuesta_cliente
- id_ejecucion
- fecha_aplicacion
- promedio_resultado
- observaciones

## 8. Entidades documentales

### 8.1 DocumentoControlado

Atributos clave:

- id_documento
- id_tipo_documento
- codigo_documento
- nombre_documento
- descripcion
- responsable_documento
- estado

### 8.2 RevisionDocumento

Atributos clave:

- id_revision_documento
- id_documento
- numero_revision
- fecha_revision
- fecha_vigencia
- id_aprobador
- estado_revision
- resumen_cambios
- ruta_archivo

### 8.3 DistribucionDocumento

Atributos clave:

- id_distribucion
- id_revision_documento
- destinatario
- fecha_distribucion
- tipo_copia
- observacion

### 8.4 RegistroControlado

Atributos clave:

- id_registro
- nombre_registro
- proceso_asociado
- responsable_archivo
- modo_archivo
- tiempo_retencion
- disposicion_final
- estado

## 9. Entidades de soporte financiero

### 9.1 ProyeccionFinanciera

Atributos clave:

- id_proyeccion
- id_periodo
- anio_proyeccion
- item
- monto_presupuestado
- id_responsable

### 9.2 FlujoCaja

Atributos clave:

- id_flujo
- id_periodo
- mes
- item
- monto_planificado
- monto_real
- variacion
- observacion

## 10. Entidades transversales

### 10.1 Evidencia

Atributos clave:

- id_evidencia
- id_tipo_evidencia
- nombre_archivo
- ruta_archivo
- fecha_carga
- id_usuario_carga
- observacion

### 10.2 BitacoraAuditoria

Atributos clave:

- id_bitacora
- fecha_hora
- id_usuario
- entidad
- id_entidad
- accion
- valor_anterior
- valor_nuevo
- direccion_ip

## 11. Relaciones principales

- Un `PeriodoEstrategico` tiene muchos `FODAItem`.
- Un `PeriodoEstrategico` tiene muchos `Objetivo`.
- Un `Objetivo` tiene muchos `Indicador`.
- Un `Indicador` tiene muchas `MedicionIndicador`.
- Un `PeriodoEstrategico` tiene muchas `RevisionDireccion`.
- Una `RevisionDireccion` tiene muchas `RevisionEntrada`.
- Una `RevisionDireccion` tiene muchos `AcuerdoRevision`.
- Un `Reclamo` puede generar una o mas `AccionCorrectivaPreventiva`.
- Una `NoConformidad` puede generar una o mas `AccionCorrectivaPreventiva`.
- Una `Auditoria` tiene muchos `HallazgoAuditoria`.
- Un `HallazgoAuditoria` puede generar una `AccionCorrectivaPreventiva`.
- Un `DocumentoControlado` tiene muchas `RevisionDocumento`.
- Una `RevisionDocumento` tiene muchas `DistribucionDocumento`.
- Una `EjecucionCurso` tiene muchas `EncuestaParticipante` y `EncuestaCliente`.
- Una `EjecucionCurso` puede asociarse a `Reclamo`, `NoConformidad` y `Evidencia`.
- Una `Evidencia` puede vincularse logicamente a varias entidades mediante relacion polimorfica o tablas de enlace.

## 12. Tablas de enlace recomendadas

Para evitar rigidez, se recomienda usar tablas de relacion para asociaciones multiples:

- `IndicadorEvidencia`
- `MedicionEvidencia`
- `ObjetivoEvidencia`
- `AccionEvidencia`
- `ReclamoEvidencia`
- `NoConformidadEvidencia`
- `RevisionEvidencia`
- `AcuerdoEvidencia`
- `AccionOrigenRelacion`

## 13. Recomendaciones de arquitectura de datos

- Mantener catalogos normalizados para tipos y estados.
- Implementar auditoria de cambios a nivel de entidad critica.
- Separar documento maestro de su revision versionada.
- Manejar adjuntos en repositorio seguro con metadatos en base de datos.
- Incluir campos de fecha de creacion, actualizacion y usuario responsable en entidades criticas.

## 14. Vista logica resumida

La cadena principal de trazabilidad esperada es:

`Periodo -> Objetivo -> Indicador -> Medicion -> Evidencia`

Y la cadena de mejora:

`Medicion/Reclamo/Auditoria/No Conformidad -> Accion Correctiva o Preventiva -> Verificacion de eficacia -> Cierre`

Y la cadena de gobierno:

`Periodo -> Revision por la Direccion -> Acuerdos -> Seguimiento`
