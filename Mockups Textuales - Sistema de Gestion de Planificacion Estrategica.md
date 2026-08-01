# Mockups Textuales - Sistema de Gestion de Planificacion Estrategica

## 1. Objetivo

Describir las pantallas principales del sistema a nivel funcional, para facilitar conversaciones con direccion, usuarios clave, UX/UI o proveedores de desarrollo.

## 2. Estructura general de navegacion

Menu principal sugerido:

- Inicio
- Planificacion estrategica
- Objetivos e indicadores
- Seguimiento
- Revision por la direccion
- Acciones correctivas/preventivas
- Reclamos y no conformidades
- Documentos y registros
- Finanzas
- Reportes
- Administracion

## 3. Pantalla de inicio / dashboard ejecutivo

### Objetivo

Entregar una vision rapida del estado del plan y del SGC.

### Estructura sugerida

Bloque superior:

- selector de periodo
- estado del plan
- fecha de ultima actualizacion
- boton `Ver plan completo`

Tarjetas resumen:

- Objetivos totales
- Indicadores en verde
- Indicadores en alerta
- Acciones abiertas
- Reclamos abiertos
- Documentos por vencer

Seccion central:

- grafico de cumplimiento por objetivo
- tabla de indicadores criticos
- tabla de acciones proximas a vencer

Seccion inferior:

- proximas revisiones por la direccion
- ultimos documentos actualizados
- ultimos acuerdos pendientes

## 4. Pantalla de planificacion estrategica

### Objetivo

Crear y administrar el plan del periodo.

### Estructura sugerida

Cabecera:

- Ano
- Nombre del periodo
- Estado
- Responsable
- Fecha de aprobacion

Pestanas:

- Resumen
- FODA
- Politica/Mision/Vision
- Objetivos
- Finanzas
- Historial

Botones principales:

- `Guardar borrador`
- `Enviar a revision`
- `Aprobar plan`
- `Cerrar periodo`

## 5. Pantalla FODA

### Objetivo

Registrar y analizar fortalezas, oportunidades, debilidades y amenazas.

### Estructura sugerida

Vista de cuatro columnas:

- Fortalezas
- Oportunidades
- Debilidades
- Amenazas

Cada tarjeta FODA debe mostrar:

- descripcion
- responsable
- fecha
- estado
- icono de evidencia adjunta

Acciones:

- `Agregar item`
- `Editar`
- `Adjuntar evidencia`
- `Ver historial`

## 6. Pantalla de objetivos e indicadores

### Objetivo

Definir objetivos, indicadores, metas y responsables.

### Estructura sugerida

Panel izquierdo:

- listado de objetivos del periodo
- filtro por tipo y estado

Panel derecho:

Seccion objetivo:

- codigo
- descripcion
- tipo
- responsable
- frecuencia
- estado

Seccion indicadores asociados:

tabla con columnas:

- indicador
- formula
- meta
- frecuencia
- responsable
- ultimo valor
- semaforo

Botones:

- `Nuevo objetivo`
- `Nuevo indicador`
- `Duplicar objetivo`
- `Adjuntar evidencia`

## 7. Pantalla de seguimiento

### Objetivo

Registrar y consultar mediciones de indicadores.

### Estructura sugerida

Filtros superiores:

- periodo
- objetivo
- indicador
- responsable
- estado

Tabla principal:

- objetivo
- indicador
- meta
- valor actual
- cumplimiento
- fecha ultima medicion
- estado
- accion

Al seleccionar una fila:

- historial de mediciones
- evidencias adjuntas
- comentarios
- boton `Registrar medicion`

Formulario de medicion:

- fecha
- valor
- comentario
- estado preliminar/validado
- adjunto

## 8. Pantalla de revision por la direccion

### Objetivo

Programar, consolidar y cerrar la revision anual.

### Estructura sugerida

Cabecera:

- fecha programada
- estado
- responsable
- boton `Generar acta`

Pestanas:

- Agenda
- Entradas
- Acuerdos
- Evidencias
- Acta

Vista de entradas:

tabla con:

- item obligatorio
- estado
- responsable de insumo
- fecha entrega
- observacion

Vista de acuerdos:

- descripcion
- responsable
- fecha compromiso
- estado
- avance

## 9. Pantalla de acciones correctivas y preventivas

### Objetivo

Gestionar causas, responsables, plazos y eficacia.

### Estructura sugerida

Filtros:

- tipo AC/AP
- estado
- origen
- responsable
- vencimiento

Tabla:

- codigo
- tipo
- origen
- descripcion resumida
- responsable
- fecha compromiso
- estado
- eficacia

Vista detalle:

- situacion detectada
- analisis de causa
- accion inmediata
- accion definitiva
- metodologia de verificacion
- evidencias
- historial

Botones:

- `Nueva accion`
- `Cambiar estado`
- `Verificar eficacia`
- `Reabrir`

## 10. Pantalla de reclamos y no conformidades

### Objetivo

Registrar y tratar incidencias del servicio o del SGC.

### Estructura sugerida

Pestanas:

- Reclamos
- No conformidades

Tabla de reclamos:

- fecha
- cliente/participante
- curso
- gravedad
- estado
- accion derivada

Tabla de no conformidades:

- fecha
- tipo
- origen
- curso
- estado
- accion derivada

Detalle:

- descripcion completa
- medida de contencion
- responsable
- evidencia
- relacion con AC/AP

## 11. Pantalla de documentos y registros

### Objetivo

Controlar documentos vigentes, obsoletos y listas maestras.

### Estructura sugerida

Pestanas:

- Documentos vigentes
- Revisiones
- Obsoletos
- Lista maestra de documentos
- Lista maestra de registros

Tabla documentos:

- codigo
- nombre
- tipo
- revision vigente
- aprobador
- fecha vigencia
- estado

Detalle de documento:

- metadatos
- historial de revisiones
- destinatarios de distribucion
- archivo vigente
- cambios relevantes

Botones:

- `Nuevo documento`
- `Nueva revision`
- `Distribuir`
- `Marcar obsoleto`

## 12. Pantalla financiera

### Objetivo

Registrar proyecciones y flujo de caja del plan.

### Estructura sugerida

Pestanas:

- Proyeccion 3 anos
- Presupuesto anual
- Flujo de caja
- Analisis de desviacion

Vista proyeccion:

- item
- ano 1
- ano 2
- ano 3
- responsable

Vista flujo:

- item
- enero a diciembre
- total plan
- total real
- variacion

## 13. Pantalla de reportes

### Objetivo

Generar salida ejecutiva y de auditoria.

### Estructura sugerida

Filtros:

- periodo
- tipo de reporte
- objetivo
- responsable
- estado

Tipos sugeridos:

- Cumplimiento general del plan
- Indicadores por objetivo
- Acciones abiertas
- Revision por la direccion
- Trazabilidad de auditoria
- Documentos vigentes y obsoletos

Botones:

- `Vista previa`
- `Exportar PDF`
- `Exportar Excel`

## 14. Pantalla de administracion

### Objetivo

Gestionar parametros y seguridad.

### Estructura sugerida

Pestanas:

- Usuarios
- Roles
- Catalogos
- Permisos
- Bitacora
- Parametros de alertas

Funciones:

- crear usuario
- asignar rol
- activar/desactivar cuenta
- administrar catalogos del sistema
- consultar log de auditoria

## 15. Recomendaciones UX

- usar semaforos para cumplimiento
- resaltar alertas y vencimientos en rojo o amarillo
- mantener acceso rapido a evidencias desde cualquier pantalla
- privilegiar tablas filtrables y exportables
- incluir botones de trazabilidad: `Ver origen`, `Ver evidencias`, `Ver acciones relacionadas`
- mostrar siempre periodo y estado vigente en cabecera
