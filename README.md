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

[01] BASE DE DATOS           : infraestructura que da soporte al, conjunto de __DATO__ de carcter operacional.

[02] DICCIONARIO DE DATOS    : infraestructura que da soporte al, conjunto de __DATO__ de carcter mas alla de lo operacional. Es decir __METADATOS__.

[03] DBMS                    : software que permite crear y mantener una __BASE_DE_DATO__ a lo largo del tiempo.

[04] PROGRAMAS DE APLICACION : software que permite interactuar con una __BASE_DE_DATO__ asiendo uso de ella. Es decir le brinda un proposito.

[05] INTERFAZ DE USUARIO     : software que comunica el DBMS con un punto final. Es decir un usuario.

[06] USUARIOS                : Puntos finales, consumidores de los servicios que una __BASE_DE_DATO__ da soporte.

[06] HERRAMIENTA CASE        : Son todo el conjunto de software que sirve de ayuda y soporte adicional, en cada parte de una __BASE_DE_DATO__.

DISEÑO DE BASE DE DATOS

[] Se espera que el diseño de una __BASE_DE_DATO__ siga el flujo de 3 etapas pricipales.

[01] MODELAMIENTO DE DATOS : Crear el {modelo_de_datos_conceptual} considerando todo lo requerido en el presente y todo lo requeible en el futuro, en lo posible.

[02] CREACION DE LA BASE DE DATOS : Crear el {modelo_de_datos_logico} a partir del {modelo_de_datos_conceptual} e integrada al DBMS.

[03] USO DE LA BASE DE DATOS : Crear infraestructura compatible con la __BASE_DE_DATO__ . Es decir programas de aplicacion, ETC...
                               !!! EN ESTA ESTA SE DIFERENCIA EL BD_LOGICO Y EL BD_FISICO.
                               !!! BD_LOGICO : Esquema arquitectral de la __BASE_DE_DATO__.
                               !!! BD_FISICO : Lugar fisico donde se almacena la __BASE_DE_DATO__.

SISTEMAS DE INFORMACION {SI}

[] Las __BASE_DE_DATO__ son una base para que los {SI} logren convertir __DATO__ en __INFORMACION__.

[] Un {SI} puede usar la misma __BASE_DE_DATO__ para entregar informacion relevante a cada nivel organizacional.

[] Clasificacion por gran rol en juego con las __BASE_DE_DATO__ son OLTP y OLAP.

[] OLTP : SI operacional-tactico automatizable llamados TPS o MIS : prefieren uso de __BASE_DE_DATO__ relacionales.

[] OLAP : SI estrategico-tactico               llamados DSS       : prefieren uso de __BASE_DE_DATO__ multidimencionales.

[] (-) valor-volumen (OLTP) ->  __DATO__ -> __INFORMACION__ -> __CONOCIMIENTO__ -> (+) valor-volumen (OLAP)

[] Los OLTP van del orden de los Kilobytes hasta los Terabytes.

[] Los OLAP van del orden de los Terabytes hasta los Yottabytes.

[] La diferencia de tamaño es porque :
                                       !!! OLTP usa una __BASE_DE_DATO__ funcional y acotada con datos actuales.
                                       !!! OLTP con el paso del tiempo dejara datos en una {base_historica}.
                                       !!! Por ende solo __DATO__ pasan a ser __INFORMACION__.
                                       !!! Pero OLAP con la ayuda de un ETL, junta las, {base_historica} + __BASE_DE_DATO__ = {warehouse}
                                       !!! OLAP/data_mining toma el {warehouse} y cualquier dato externo para el analisiz.
                                       !!! Por ende solo __INFORMACION__ pasan a ser __CONOCIMIENTO__.

TIPOS DE BASES DE DATOS

[] Estructura de datos para almacenamiento :
                                             !!! Parametro fundamental para el DBMS, ya que el se encarga de organizar los __DATO__ internamente.
                                             !!! 01 : Jerarquico, es decir, 
                                                                             Arbol de nodos,
                                                                             Un nodo puede tener 0 o mas hijos,
                                                                             Un nodo tiene solo 1 padre,
                                                                             Hay un nodo raiz.
                                             !!! 02 : Reticular, es decir,
                                                                             Grafo o red de nodos,
                                                                             Extencion jerarquico donde cada nodo puede tener mas de un padre.
                                             !!! 03 : Orientada a objetos, es decir,
                                                                             La unidad atomica son objetos de orientacion a objetos,
                                                                             Gran afinidad a programacion orientada a objetos,
                                                                             Gran flexibilidad.
                                             !!! 04 : multidimencional, es decir,
                                                                             Datos en dispocicion hiper-cubica/hiper-dimencional,
                                                                             Util para manejar el {warehouse}.
                                                                             DRILL DOWN se usa para agregar/quitar dimenciones al navegar desendente.
                                                                             DRILL DOWN se usa para quitar/agregar dimenciones al navegar asendente.
                                             !!! 05 : Relacional, es decir,
                                                                             Los __DATO__ son incrustados en tablas bidimencionales o relaciones,
                                                                             Especial interes.
                                                                             Conjunto de relaciones relacionadas.
                                                                             Cada columna tiene un unico valor.
                                                                             Todas las filas son de un unico tipo.
                                                                             Las filas y columnas no tienen un orden en particular.
                                                                             las relacionas se logran por clave primaria y foranea.
                                                                             clave primaria : subconjunto de columnas qie identifican la relacion de forma unica.
                                                                             clave foranea  : columna de relacion extranjera para identificarla.

[] Nivel organizacional.
                                             !!! 01 : __BASE_DE_DATO__ operacional : que utiliza OLTP.
                                             !!! 02 : __BASE_DE_DATO__ tactico     : que utiliza OLAP.
                                             !!! 03 : __BASE_DE_DATO__ estrategico : que utiliza data_mining.

[] Tipo de datos.
                                             !!! 01 : Estructurado (preciso) : relciones = tablas bidimencionales,
                                                                               filas y columnas independientes.
                                             !!! 02 : Agregado               : hiper-cubo, filas y columnas sobrepuestas entre si.
                                             !!! 03 : Semiestructurado       : sistema no-relacional con capacidad de consulta.
                                             !!! 04 : No estructurado        : NoSQL o NOSQL, la estructura no es rigida, es flexible y se adapta a nuevos datos,
                                                                               surge debido a manejar BIG-DATA, por ejemplo, por redes sociales.

[] Ubicacion de la copia princial.
                                             !!! 01 : Memoria principal         - nivel 1 : __BASE_DE_DATO__ veloz, pero volatil.
                                             !!! 02 : Memoria secundaria        - nivel 2 : __BASE_DE_DATO__ lenta, pero persistente.
                                             !!! 03 : almacenamiento terciario  - nivel 3 : __BASE_DE_DATO__ medio offline de cararcter externo.
                                             
[] Numero de procesadores.
                                             !!! 01 : 


[] Estructura de datos para almacenamiento.





