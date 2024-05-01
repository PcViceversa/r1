INF239 : BASES DE DATOS

--- --- --- --- --- --- --- --- ---
--- --- --- --- --- --- --- --- ---

CONCEPTOS

[] [*] [*] [*] Un __RECURSO__ es cuya entidad posee un __COSTO__ y un __VALOR__.
    
[] Un __DATO__ es __RECURSO__ de tipo hecho.                                              Es decir, eventos mensurables de entidades.

[] Un __INFORMACION__ es un conjunto de __DATO__ organizados.                             Es decir, insumos de una decicion y producto de una accion.

[] Un __SISTEMA_DE_INFORMACION__ transforma __DATO__ almacenados en __DATO__ organizados. Es decir, __INFORMACION__ , {datos_almacenados} -> {datos_organizados}.

[] Un __ARCHIVOS_PLANO__         transforma __DATO__             en __DATO__ almacenados.                Es decir, __DATO__ -> {datos_almacenados}.

[] Un __BASE_DE_DATO__           transforma __DATO__             en __DATO__ almacenados y relacionados. Es decir, __DATO__ -> {datos_almacenados}{datos_relacionados}.

MECANISMOS UTILES

[] Los __SISTEMA_DE_INFORMACION__ nesesitan datos_almacenados para generar __INFORMACION__.

[] Los __ARCHIVOS_PLANO__ si, y los __BASE_DE_DATO__ si,    permitenen producir {datos_almacenados} a partir de __DATO__

[] Los __ARCHIVOS_PLANO__ no, y los __BASE_DE_DATO__ si,    permitenen producir {datos_relacionados} a partir de __DATO__

[] La diferencia en __ARCHIVOS_PLANO__ y __BASE_DE_DATO__ , supone caracteristicas propias/compartidas  para cada uno respecto del otro.

[] La diferencia en __ARCHIVOS_PLANO__ y __BASE_DE_DATO__ , supone aspectos de     ventajas/desventajas para cada uno respecto del otro.

[] Los __ARCHIVOS_PLANO__ : producen {datos_almacenados}    que posean   la misma estructura. [dentro a fuera].

[] Los __ARCHIVOS_PLANO__ : producen {datos_almacenados}    que refieran el mismo ente.       [fuera a dentro].

[] Los __BASE_DE_DATO__   : producen {datos_almacenados} y {datos_relacionados} con definicion.

[] Los __BASE_DE_DATO__   : con definicion, interceptan NIVELES[estrategico-tactico-operacional] con AREAS[finanzas-marketing-rrhh].

COMPARATIVAS VENTAJAS/DESVENTAJAS

[] Los __ARCHIVOS_PLANO__ : Tienen redundancia por parte de la apliacion. Es decir, utilizacion eficiente del espacio comprometida perse.

[] Los __ARCHIVOS_PLANO__ : Tienen dependencia por parte de la apliacion. Es decir, el codigo del programa debe definir los __DATO__ que lo conforman.

[] Los __ARCHIVOS_PLANO__ : Tienen estandarizacion interezante. DESCENTRALIZADO. Es decir "NOTA" puede ser una calificacion o una orden de compra.

[] Los __ARCHIVOS_PLANO__ : Tienen aspectos de PRODUCTIVIDAD, INCONSISTENCIA, COMPARTIR, CLIENTE, ETC...

[] Los __BASE_DE_DATO__   : Tienen redundancia por parte de los __DATO__.

[] Los __BASE_DE_DATO__   : Tienen independencia por parte de la aplicacion.

[] Los __BASE_DE_DATO__   : Tienen estandarizacion interezante. CENTRALIZADO.

[] Los __BASE_DE_DATO__   : Tienen aspectos de PRODUCTIVIDAD, CONSISTENCIA, COMPARTIR, CLIENTE, ETC...

ENFOQUE

[] Los __ARCHIVOS_PLANO__ y __BASE_DE_DATO__ son dos enfoques para obtener {datos_almacenados}

[] Al preferir el enfoque de __BASE_DE_DATO__ como el enfoque a analizar, puede exirtir la posibilidad de analizarlo.

[] En consecuencia se estudia a continuacion el enfoque de __BASE_DE_DATO__ [NINGUNO MEJOR QUE OTRO - SON DISTINTOS]

BASE DE DATOS - COMPONENTES

[01] BASE DE DATOS        : infraestructura que da soporte al, conjunto de __DATO__ de carcter operacional.

[02] DICCIONARIO DE DATOS : infraestructura que da soporte al, conjunto de __DATO__ de carcter mas alla de lo operacional. Es decir __METADATOS__.

[03] DBMS                 : software que permite crear y mantener una __BASE_DE_DATO__ a lo largo del tiempo.

[04] PROGRAMAS DE APLICACION : software que permite interactuar con una __BASE_DE_DATO__ asiendo uso de ella. Es decir le brinda un proposito.

[05] INTERFAZ DE USUARIO     : software que comunica el DBMS con un punto final. Es decir un usuario.

[06] USUARIOS                : Puntos finales, consumidores de los servicios que una __BASE_DE_DATO__ da soporte.

[06] HERRAMIENTA CASE        : Son todo el conjunto de software que sirve de ayuda y soporte adicional, en cada parte de una __BASE_DE_DATO__.

DISEÑO DE BASE DE DATOS











