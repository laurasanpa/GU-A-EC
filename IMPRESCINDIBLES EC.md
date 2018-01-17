# INFORMACIÓN RELEVANTE #
_______

## ¿QUÉ SABER PARA APROBAR EC?

1. En **x86-64**, el **contador de programa** (PC) se llama **RIP**.
2. En la **3ª generación** de computadores aparecen los **circuitos integrados, la microprogramación, la segmentación de cauce, la memoria caché, la memoria virtual, etc...**
3. La **diferencia entre mov y lea** es que mov accede a la posición indicada, mientras que lea no.
4. Flags:
    
    CF -> Acarreo
    
    SF -> Signo
    
    PF -> Paridad
    
    TF -> Trampa
    
    AF -> Ajuste
    
    IF -> Interrupción
    
    ZF -> Cero
    
    DF -> Dirección
    
    OF -> Desbordamiento
    
5. La instrucción **JGE/JNL** provoca un salto si **OF=SF**.
6. La combinación de flags que corresponde al código de condición **below** es **CF xor OF**.
7. La instrucción **cmovb** es igual que mov pero sólo se realiza si hay **acarreo**.
8. El lenguaje **C** no permite el paso de parámetros por **referencia**.
9. Al llamar a una función con dos argumentos "f(arg1, arg2)" las instrucciones se ejecutan en el siguiente orden: **push arg2, push arg1, call f, push %ebp**.
10. Cuando se ejecuta la instrucción **ret** al final de una subrutina, la dirección almacenada en la **cima de la pila** se transfiere **al contador de programa**.
11. En IA-32, la **pila** es un **conjunto de posiciones** de memoria usadas para almacenar información temporal durante la ejecución y el **puntero de pila** es un **registro de 32 bits** en el microprocesador.
12. **Guardar o recuperar** un registro de la pila **NO** es una operación básica de la **unidad de control**.
13. En la **técnica de salto retardado** el compilador puede reorganizar el código para **rellenar** los huecos de retardo con instrucciones útiles.
14. El método de interacción con los periféricos, en el que el procesador **vigila periódicamente** el estado de los dispositivos mediante una **encuesta activa** se llama **POLLING**.
15. Se necesitan **2** señales de control para poder implementar un sistema de **gestión de interrupciones**.
16. Las celdas de memoria **estática** **NO** tienen que ser **refrescadas** continuamente.
17. La **dirección efectiva del primer parámetro** de llamada a una función suele calcularse como **EBP+8**.
18. Casi **todos** los procesadores actuales tienen memoria caché **L2**.
19. Un procesador actual tiene **varias** cachés de **nivel 1**.
20. La caché de **nivel 3 NO** contine **toda** la memoria que maneja el programa.
21. El **mínimo** valor que causa acarreo en suma **SIN** signo sumado 32 veces es el **0x0800 0000**.
22. El **menor** valor positivo que repetido 32 veces causaría **overflow** en suma **CON** signo es **0x0400 0000**.
23. El **mínimo** valor que causa desbordamiento en suma **CON** signo sumado 32 veces es el **0xfbff ffff**.
24. Según la clasificaciónm/n, las máquinas de **acumulador** son de tipo **1/1**, y las **R/R** de tipo **x/0 con x=2,3**.
25. El **bus de sistema** es el que conecta la **CPU con Memoria**, ya sea un sitema con un únic bus o con múltiples buses.
26. La **ecuación básica de rendimiento** calcula el **promedio de las ganancias** obtenidas con una serie de programas de punto entero.
27. En el modo de direccionamiento del tipo **desplazamiento** puede usarse desplazamiento, cualquier constante de 1,
2 o 4 bytes (incluso el nombre de una
variable, por su dirección).
28. Para traducir una construcción **do-while** de lenguaje C a ensamblador, gcc utiliza un **salto condicional hacia atrás** con la **misma condición** que en C.
29. El **PC** (flags) **NO** sirve de **entrada** de la **unidad de control**, mientras que **SÍ** lo son: señal de reloj, IR o estado de la unidad de proceso.
30. La **dirección de la siguiente microinstrucción NO** es salida de la **unidad de control**.
31. Los **riesgos** en **cauces segmentados** son **riesgos de transferencia**.
32. Para un procesador con **segmentación de cauce** los modos **menos** recomendables son **directo** e **indirecto a través de memoria**.
33. El **salto retardado** ejecuta siempre, mientras que el **anulante** sólo si se cumple la **condición de salto**.
34. La técnica de direccionamiento por **selección lineal** permitiría escribir un **mismo dato** en **varios puertos* E/S.
35. La **E/S independiente** es:
 - Más fácil de proteger.
 - Aprovecha mejor el espacio.
 - Decodifica más elegantemente.
 - Tiene un diseño del procesador más complejo.
35. Las CPUs actuales contemplan las interrupciones internas, externas y software, no firmware.
36. Para **determinar la causa de una interrupción** se pueden usar: múltiples líneas, polling, interrupciones vectorizdas, pero **NO línea de reconocimiento**.
37. Podemos usar la palabra **directo** para referirnos a: caché con correspondencia directa, acceso directo a memoria y modo de direccionamiento directo, pero **NO** para **dispositivos de almacenamiento secuencial directo**.
38. La **unidad de transferencia** varía **xi <= xi+1**.
39. Las técnicas **write-trough** y **write-back** están relacionadas con **coherencia de caché**.
40. En contraposición a un ejecutable ELF, un fichero **objeto** ubica el código y los datos a partir de la posición 0x0, las direcciones definitivas sólo se calculan tras enlazar.
41. En x86-64 se pueden referenciar los registros **%rax, %eax, %ax, %ah, %al**.
42. Las arquitecturas de **registros** de propósito general se impusieron a las basadas en pila porque las basadas en registros son capaces de lograr un **mejor rendimiento** cuando se asignan variables a registros.
43. Cuestiones sobre direccionamiento: 
- El direccionamiento **indexado** es útil para **vectores**.
- El direccionamiento **implícito NO** indica la **dirección del operando**.
- El direccionamiento **inmediato** el dato se encuentra en la **instrucción**.
- El direccionamiento **indirecto NO** indica la **dirección del operando**.

44. Sobre el direccionamiento **absoluto**:
- La **instrucción** contiene la **dirección de memoria** en la que se encuentra el **objeto**.
- El **objeto** está en una posición de **memoria**.
- El rango de **posiciones direccionables** queda limitado por el **tamaño del campo de direccionamiento**.
- El tamaño del **operando de direccionamiento NO** queda limitado por el nº de bits del **campo de direccionamiento**.
45. La diferencia entre el **desplazamiento a la derecha lógico y aritmético** es que insertan de **forma distinta** el bit más a la izquierda.
46. La instrucción **seta %al** pone AL a 1 si **CF=0 y ZF=0**.
47. Los **arrays bidimensionales** en C se almacenan en orden **mayor-de-fila**.
48. El desplazamiento **directo** a memoria utiliza **un desplazamiento**.
49. Las subrutinas **NO** necesitan recibir parámetros desde el programa que hace la llamada para saber **qué registros se pueden alterar**.
50. Cuanto mayor sea la **relación** entre el **tiempo de ejecución de una instrucción** y el **tiempo de una etapa**, mayor será la ganancia máxima.
51. En la **segmentación**, **retrasar** la fase de decisión saltar/no saltar de las instrucciones de salto condicional **deteriora** el rendimiento del procesador.
52. La **precaptación** está relacionada con los riesgos **estructurales**.
53. La **predicción de saltos** está relacionada con los riegos de **control**.
54. Si en un computador cada dirección especifica **uno o dos** puerto, un puerto será solo de **entrada** y el otro solo de **escritura** y ambos decodifican en la misma dirección.
55. Si el repertorio de un procesador tiene instrucciones de tipo **IN/OUT**, es que el computador dispone de **E/S Mapeada**.
56. Cuando dos procesadores con el mismo número de líneas en los buses de bus de direcciones, uno E/S mapeada, y el otro E/S independiente, podrá acceder a **mayor cantidad de memoria** el que tiene **E/S independiente**.
57. Sólo la E/S por **DMA** libera a la CPU de realizar la **consulta de estado** del dispositivo de E/S.
58. En la caché de **nivel 1**, la **tasa de fallos** tiende a **disminuir** si el tamaño total de L1 **crece**.
59. En IA32 **NO** se puede hacer **pop %eip**.
60. La instrucción **leave** hace lo mismo que **mov %ebp, %esp; pop %ebp**.
61. El **primer procesador** de Intel de 64 bits en la familia x86 fue el Pentium 4F.
62. x86-64 **NO** usa %rbp como puntero **base** para el marco de pila. 
63. La **emisión múltiple NO** es un motivo de que **NO** se alcance la **ganancia ideal** en un cauce segmentado.
64. Las cachés **totalmente asociativas** ofrecen tasas de fallo más bajas, mientras que las de **correspondencia directa** tienen mejor latencia.
65. El programa que convierte un programa **fuente de alto nivel** en lenguaje **máquina** es un **compilador**.
66. En el direccionamiento **inmediato** el operando reside en la **instrucción** tras el código de operación.
67. Cuando un **Intel Atom** ejecuta una instrucción CALL, el registro **eip** se guarda en la pila.
68. Una tarea propia de la **Unidad de control** es **decodificar** las instrucciones del programa.
69. Una **operación segmentada**(segmentación de cauce) requiere el **mismo tiempo o más**, desde el principio hasta el fin, que la misma operación en una implementación no segmentada.
70. Las interrupciones generadas por el **teclado** interrumpirán al procesador sólo si el procesador tiene activado el indicador de **habilitación de interrupciones**.
71. Las interrupciones iniciadas por un dspositivo de E/S son normalmente **externas**.
72. La **unidad de control** necesita como netrada el registro de estado para poder controlar la ejecución de las instruccions de salto condicional.
73. **Microcódigo** es el **contenido** de la memoria de control y una **microinstrucción** es una **palabra** de dicha memoria.
74.**MAR** requiere **menos** señales de control que **MBR**.
75. Un posible formato de microprogramación se caracteriza como **horizontal** o **vertical** según tenga más o menos **solapamiento, codificación y longitud relativa de microinstrucción**.
76. El **control residual** se utiliza para **reducir** el tamaño de la memoria de **control**.
77. En un procesador con segmentación de cauce, al **aumentar** el número de etapas se produce un **incremento** de las prestaciones.
78. El registro **WC** es un controlador de **DMA**.
79. La política de correspondencia de una memoria caché con 1 **único conjunto** es **totalmente asociativa**.
80. La política de correspondencia de una memoria caché con la **mitad de conjunto que líneas** es **asociativa pr conjuntos de dos vías**.
81. Las máquinas con arquitectura **Von Neuman** ejecutan programas **almacenados**.
82. El **PC** apunta a la **siguiente instrucción**.
83. La **palabra de estado** contiene el **código de operación** de la instrucción en curso.
84. La información sobre el **sentido** de las transferencias de información circula por el bus de  **control**.
85. Normalmente, el bus de **datos** de un ordenador es **bidireccional**.
86. Emparejamientos entre tipos de aquitecturas de procesador e instrucciones máquinas:
 - Pila: xor.
87. La instrucción **pushf** utiliza direccionamiento **implícito**.
88. El código **reeentrante** debe usar direccionamiento **relativo**.
89. Si los códigos de operación de las instrucciones de un procesador tienen diferentes longitudes, se emplean las técnicas de **extensión o Huffman**.
90. La **modificación** de la secuencia de ejecución es el **segundo** tipo de instruccionesmás usado.
91. En un sistema de memoria caché el **directorio caché** suele contener **direcciones de bloques**.
92. El mejor método para **comparar prestaciones** de dos sistemas con CPUs del mismo tipo es usar **prograas d prueba**.
93. La ejecución de una instrucción en una arquitectura **Von Newmann** suele dividirse en **carga, decodificación, ejecución y escritura**.
94. El conjunt de todos los atributos de un sistema qeu son visibles para el programador y sn necesarios para programasr en lenguaje máquina se denomina **arquitectura del computador**.
95. El registro de estado **(flags)** es un registro de propósito específico cuyo contenido puede ser vsto directa o indirectamente or el usuario mediante el uso de ciertas instrucciones específicas.
96. En una arquitectura de  **acumulador**, la instrucción **LOAD X** tranfiere el contenido de la posición de memoria X al acumulador-
97. Una instrucción máquina del tipo **Add M,R** podría formar parte del repertorio de una máquina con arquitectura **M/M**.
98. Un **bus** se compone de **líneas de control/estado, líneas de direccción y líneas de datos**.
99.El **primer computador** electrónico basaba su funcionamiento en **tubos de vacío**.
100. La instrucción **leave** aasegura que en ese punto del programa ya **NO** hay registros **salva-invocados** que recuperar.
101. En IA32, para **intercambiar** el valor de dos variables son necesarios al menos **4 mov**.
102. En IA32, **esp** no puede ser registro **índice**.
103. Una unidad de control microprogramada se denomina con **secuenciamiento de microinstrucciones explícito** segun tenga o no unn m **micro-contador** de programa atacando a las líneas de dirección de la memoria de control. 
104. Uno de los **motivos** que impiden que la ganancia de un **cauce segmentado** sea ideal es la **cola de instrucciones**.
105. La técnica de **adelanto de registros** en un cauce segmentado se usa para **limpiar** el impacto de los riegos de dependencia de datos. 
106.
