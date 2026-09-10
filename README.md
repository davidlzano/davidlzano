# David A. Lozano Rodríguez

**Analista de Datos y Business Intelligence** · Medellín, Colombia

Trabajo en la parte del dato que casi nadie ve: la integración, el modelado y la automatización que hacen que un dashboard signifique algo. Vengo de cuatro años dentro de áreas operativas antes de dedicarme a datos de tiempo completo, y esa ruta define cómo trabajo — entiendo por qué el dato llega sucio, quién lo digita y qué decisión depende de él.

Hoy construyo pipelines ETL en Python contra APIs de sistemas transaccionales, modelo en SQL Server con versionado histórico, desarrollo aplicaciones internas de captura y diseño motores que generan planes operativos bajo restricciones reales.

---

## Proyectos

Los cuatro son reimplementaciones demostrativas de sistemas que puse en producción. Código original, datos sintéticos, ejecutables con dos comandos.

### [Motor de optimización de traslados de inventario](https://github.com/davidlzano/motor-traslados-inventario)

Genera el plan diario de redistribución de inventario para una red de tiendas: qué mover, desde dónde, hacia dónde y cuánto. Resuelve una variante del problema de transporte con una heurística priorizada en tres etapas, respetando compatibilidad de producto, capacidad dinámica de cada punto y viabilidad económica del flete.

En producción cubre cerca de 470 tiendas y reemplazó un ejercicio manual que tomaba una semana al mes.

`Python` · `SQLite` · `pandas`

### [Pipeline ETL con tolerancia a fallos](https://github.com/davidlzano/pipeline-etl-tolerante-fallos)

Integración diaria desde una API hacia un data warehouse. Ventana móvil auto-recuperable, reintentos con espera creciente, manejo diferenciado de errores transitorios y permanentes, y carga incremental por hash de fila que descarta lo que no cambió.

La API simulada falla a propósito el 35% de las veces, así que la tolerancia a fallos se puede ver operando en lugar de solo leerse.

`Python` · `SQLite` · `pandas`

### [Aplicación de captura de datos en planta](https://github.com/davidlzano/app-captura-planta)

Formulario web para registro de producción por hora desde el celular, en piso de fábrica. El operario digita la lectura del contador y el sistema deriva la producción, que es lo que elimina el error de restar mentalmente cada hora. Catálogos que se recargan sin reiniciar el servicio y validación del lado del servidor.

`Python` · `Flask` · `SQLite`

### [Histórico versionado de programación de planta](https://github.com/davidlzano/historico-programacion-planta)

Convierte respaldos diarios de un archivo de Excel editado a mano en una base con línea de tiempo consultable. Mapea por nombre de encabezado porque las columnas se mueven entre archivos, guarda solo los cambios en lugar de fotos completas, y distingue una hoja ilegible de una fila borrada.

En producción cubre 22 centros de trabajo y permitió recuperar una pérdida de datos real.

`Python` · `openpyxl`

---

## Herramientas

**Datos:** SQL Server · SQL · procesos ETL · modelado dimensional · datos maestros (MDM)
**Python:** pandas · NumPy · Flask · consumo de APIs · automatización
**BI:** Power BI · DAX · Excel avanzado (Power Query, Power Pivot, VBA)

---

## Contacto

Abierto a oportunidades como Analista de Datos o BI, en modalidad **remota o híbrida**.

[LinkedIn](https://www.linkedin.com/in/david-a-lozano-rodríguez-7b2a62261) · davidlzano19@gmail.com
