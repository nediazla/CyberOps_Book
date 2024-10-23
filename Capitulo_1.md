# Fundamentos de Ciber Seguridad

## Este capítulo cubre los siguientes temas:
- Introducción a la ciberseguridad
- Amenazas, vulnerabilidades y exploits
- Sistemas de seguridad de red
- Sistemas de detección de intrusiones y sistemas de prevención de intrusiones
- Protección avanzada contra malware
- Dispositivo de seguridad web
- Dispositivo de seguridad de correo electrónico
- Dispositivo de administración de seguridad de Cisco
- Cisco Identity Services Engine
- Soluciones de seguridad basadas en la nube
- Cisco NetFlow
- Prevención de pérdida de datos
- Los principios de la estrategia de defensa en profundidad
- Confidencialidad, integridad y disponibilidad: la tríada CIA
- Riesgo y análisis de riesgos
- Información de identificación personal e información de salud protegida
- Principio de privilegio mínimo y separación de funciones
- Centros de operaciones de seguridad
- Manuales, manuales de procedimientos y automatización de manuales de procedimientos
- Informática forense digital

¡Bienvenido al comienzo de su viaje hacia la certificación CyberOps Associate! Los programas de ciberseguridad reconocen que las organizaciones deben estar alertas, ser resilientes y estar listas para proteger y defender cada conexión de entrada y salida, así como los datos de la organización donde sea que se almacenen, transmitan o procesen. En este capítulo, aprenderá los conceptos de ciberseguridad y seguridad de la información. Luego, aprenderá la diferencia entre amenazas, vulnerabilidades y ataques de ciberseguridad. También explorará las amenazas de ciberseguridad más comunes, así como las vulnerabilidades comunes de software y hardware. Aprenderá los detalles sobre la tríada de confidencialidad, integridad y disponibilidad (CIA). Además, aprenderá sobre las diferentes amenazas de seguridad en la nube y de IoT.

En este capítulo, también se describen los diferentes tipos de dispositivos de seguridad de red y servicios en la nube en la industria. Compara los firewalls tradicionales y los firewalls de próxima generación (NGFW), así como los sistemas de prevención de intrusiones (IPS) tradicionales y los IPS de próxima generación (NGIPS).

Obtendrá detalles sobre las soluciones Cisco Web Security y Cisco Email Security, así como
qué es la protección avanzada contra malware (AMP), qué son los sistemas de administración de identidad, cómo usar Cisco NetFlow y detalles sobre la prevención de pérdida de datos (DLP).
El capítulo concluye con una introducción a la respuesta a incidentes y análisis forense digital (DFIR) y a las operaciones de seguridad. En el resto del libro se ofrecen más detalles sobre cada uno de estos temas.
## Introducción a la ciberseguridad
El objetivo de la ciberseguridad es proteger a cada uno de nosotros, nuestra economía, nuestras escuelas, nuestra infraestructura crítica y cualquier otra organización del daño que puede resultar del mal uso, la vulneración o la destrucción involuntaria o intencional de la información y los sistemas de información.

El riesgo de ciberseguridad incluye no solo el riesgo de una violación de datos, sino también el riesgo de que toda la organización se vea socavada por actividades comerciales que dependen de la digitalización y la accesibilidad. Como resultado, aprender a desarrollar un programa de ciberseguridad adecuado es crucial para cualquier organización. La ciberseguridad ya no puede ser algo que se delegue al equipo de tecnología de la información (TI). Todos deben participar, incluida la junta directiva.
## Ciberseguridad vs. Seguridad de la información (Infosec) 
Muchas personas confunden la seguridad de la información tradicional con la ciberseguridad. En el pasado, los programas y políticas de seguridad de la información se diseñaban para proteger la confidencialidad, la integridad y la disponibilidad de los datos dentro de los límites de una organización. Lamentablemente, esto ya no es suficiente. Las organizaciones rara vez son autónomas, y el precio de la interconectividad es un mayor nivel de exposición a ataques. Toda organización, independientemente de su tamaño o ubicación geográfica, es un objetivo potencial. La ciberseguridad es el proceso de proteger la información mediante la prevención, detección y respuesta a los ataques.

Los programas de ciberseguridad reconocen que las organizaciones deben estar alertas, ser resilientes y estar listas para proteger y defender cada conexión de entrada y salida, así como los datos de la organización donde sea que se almacenen, transmitan o procesen. Los programas y políticas de ciberseguridad amplían y se basan en los programas de seguridad de la información tradicionales, pero también incluyen lo siguiente:
- Gestión y supervisión de riesgos cibernéticos
- Inteligencia sobre amenazas e intercambio de información
- Búsqueda de amenazas (búsqueda proactiva de posibles compromisos y amenazas en su organización que no hayan sido detectados por sus productos o tecnologías de seguridad)
- Gestión de dependencias de hardware, software y organizaciones de terceros
- Respuesta a incidentes y resiliencia
## El marco de ciberseguridad del NIST
El Instituto Nacional de Estándares y Tecnología (NIST) es una agencia federal no regulatoria
reconocida dentro de la Administración de Tecnología del Departamento de Comercio de los EE. UU. La misión del NIST es desarrollar y promover la medición, los estándares y la tecnología para mejorar la productividad, facilitar el comercio y mejorar la calidad de vida. La División de Seguridad Informática (CSD) es una de las siete divisiones dentro del Laboratorio de Tecnología de la información del NIST. El marco de seguridad cibernética del NIST es una recopilación de estándares de la industria y mejores prácticas para ayudar a las organizaciones a gestionar los riesgos de seguridad cibernética. Este marco se creó en colaboración entre el gobierno de los Estados Unidos, corporaciones e individuos. Se puede acceder al marco de seguridad cibernética del NIST en www.nist.gov/cyberframework.

El marco de seguridad cibernética del NIST se desarrolló con una taxonomía común y uno de los objetivos principales es abordar y gestionar el riesgo de seguridad cibernética de una manera rentable para proteger la infraestructura crítica. Aunque está diseñado para un grupo específico, los requisitos pueden servir como modelo de seguridad para cualquier organización.

Guía y documentos adicionales del NIST Actualmente, hay más de 500 documentos relacionados con la seguridad de la información del NIST. Esta cantidad incluye FIPS, la serie SP 800 y 1800, boletines ITL e informes interinstitucionales del NIST:
- Estándares federales de procesamiento de información (FIPS): esta es la serie de publicaciones oficiales para estándares y pautas.
- Serie de publicaciones especiales (SP) 800: esta serie informa sobre las investigaciones, las pautas y los esfuerzos de divulgación del ITL en materia de seguridad de los sistemas de información y sus actividades de colaboración con la industria, el gobierno y las organizaciones académicas. Los documentos de la serie SP 800 se pueden descargar de https://csrc.nist.gov/publications/sp800.
- Serie de publicaciones especiales (SP) 1800: esta serie se centra en las prácticas y pautas de seguridad cibernética. El documento de la serie SP 1800 se puede descargar de https://csrc.nist.gov/publications/sp1800.
- Informes internos o interinstitucionales del NIST (NISTIR): estos informes se centran en los hallazgos de las investigaciones, incluida la información de referencia para los FIPS y los SP.
- Boletines del Laboratorio de Tecnología de la Información (ITL): cada boletín presenta un análisis en profundidad de un solo tema de interés significativo para la comunidad de sistemas de información. Los boletines se emiten según sea necesario.

Desde los controles de acceso hasta la seguridad inalámbrica, las publicaciones del NIST son un verdadero tesoro de orientación valiosa y práctica.
## Organización Internacional de Normalización
La Organización Internacional de Normalización (conocida como ISO) es una red de institutos de normalización nacionales de más de 160 países. La ISO ha desarrollado más de 13.000 normas internacionales sobre una variedad de temas, que van desde códigos de países hasta
seguridad de los pasajeros.

La serie ISO/IEC 27000 (también conocida como la Familia de Normas ISMS, o ISO27k para abreviar) comprende normas de seguridad de la información publicadas conjuntamente por la ISO y la Comisión Electrotécnica Internacional (IEC).

Los primeros seis documentos de la serie ISO/IEC 27000 brindan recomendaciones para “establecer, implementar, operar, monitorear, revisar, mantener y mejorar un Sistema de Gestión de Seguridad de la Información”:
- ISO 27001 es la especificación para un sistema de gestión de seguridad de la información (SGSI).
- ISO 27002 describe el código de prácticas para la gestión de la seguridad de la información.
- La norma ISO 27003 proporciona una guía de implementación detallada.
- La norma ISO 27004 describe cómo una organización puede supervisar y medir la seguridad utilizando métricas.
- La norma ISO 27005 define el enfoque de gestión de riesgos de alto nivel recomendado por la ISO.
- La norma ISO 27006 describe los requisitos para las organizaciones que medirán el cumplimiento de la norma ISO 27000 para la certificación.

En total, hay más de 20 documentos en la serie y varios más aún están en desarrollo.
El marco es aplicable a organizaciones públicas y privadas de todos los tamaños. Según el sitio web de la ISO, “la norma ISO ofrece recomendaciones para la gestión de la seguridad de la información para su uso por parte de quienes son responsables de iniciar, implementar o mantener la seguridad en su organización. Su objetivo es proporcionar una base común para el desarrollo de estándares de seguridad organizacional y prácticas de gestión de seguridad efectivas y brindar confianza en las relaciones entre organizaciones”.
## Amenazas, vulnerabilidades y exploits
Las siguientes secciones describen las características de las amenazas, vulnerabilidades y exploits.
### ¿Qué es una amenaza?
Una amenaza es cualquier peligro potencial para un activo. Si existe una vulnerabilidad pero aún no se ha explotado (o, lo que es más importante, aún no se conoce públicamente), la amenaza está latente y aún no se ha percibido . Si alguien está lanzando activamente un ataque contra su sistema y accede con éxito a algo o compromete su seguridad contra un activo, la amenaza se hace realidad.
La entidad que aprovecha la vulnerabilidad se conoce como actor malicioso, y la ruta utilizada por este actor para realizar el ataque se conoce como agente de amenaza o vector de amenaza.
### ¿Qué es una vulnerabilidad?
Una vulnerabilidad es una debilidad en el diseño, la implementación, el software o el código del sistema o la falta de un mecanismo. Una vulnerabilidad específica puede manifestarse como cualquier cosa, desde una debilidad en el diseño del sistema hasta la implementación de un procedimiento operativo. La correcta implementación de salvaguardas y contramedidas de seguridad podría mitigar una vulnerabilidad y reducir el riesgo de explotación.

Las vulnerabilidades y debilidades son comunes, principalmente porque no existe ningún software o código perfecto. Algunas vulnerabilidades tienen un impacto limitado y se mitigan fácilmente; sin embargo, muchas tienen implicaciones más amplias.

Las vulnerabilidades se pueden encontrar en cada uno de los siguientes elementos:
- Aplicaciones: el software y las aplicaciones vienen con toneladas de funcionalidad. Las aplicaciones pueden estar configuradas para la facilidad de uso en lugar de para la seguridad. Las aplicaciones pueden necesitar un parche o una actualización que puede o no estar disponible. Los atacantes que atacan las aplicaciones tienen un entorno rico en objetivos para examinar. Piense en todas las aplicaciones que se ejecutan en su computadora de casa o del trabajo.
- Sistemas operativos: el software del sistema operativo se carga en las estaciones de trabajo y los servidores. Los atacantes pueden buscar vulnerabilidades en sistemas operativos que no han sido parcheados o actualizados.
- Hardware: las vulnerabilidades también se pueden encontrar en el hardware. La mitigación de una vulnerabilidad de hardware puede requerir parches para el microcódigo (firmware), así como para el sistema operativo u otro software del sistema. Algunos buenos ejemplos de vulnerabilidades basadas en hardware conocidas son Spectre y Meltdown. Estas vulnerabilidades se aprovechan de una característica llamada ejecución especulativa, común en la mayoría de las arquitecturas de procesadores modernas.
- Configuración incorrecta: el archivo de configuración y la configuración del dispositivo o software pueden estar mal configurados o implementados en un estado no seguro. Esto puede ser puertos abiertos, servicios vulnerables o dispositivos de red mal configurados. Solo piense en las redes inalámbricas. ¿Puede detectar algún dispositivo inalámbrico en su vecindario que tenga el cifrado desactivado?
- Software Shrinkwrap: esta es la aplicación o archivo ejecutable que se ejecuta en una estación de trabajo o servidor. Cuando se instala en un dispositivo, puede tener toneladas de funcionalidad o scripts o códigos de muestra disponibles.

Los proveedores, investigadores de seguridad y centros de coordinación de vulnerabilidades generalmente asignan a las vulnerabilidades un identificador que se divulga al público. Esto se conoce como el identificador de vulnerabilidades y exposiciones comunes (CVE). CVE es un estándar de toda la industria. CVE está patrocinada por US-CERT, la oficina de Ciberseguridad y Comunicaciones del Departamento de Seguridad Nacional de los Estados Unidos. MITRE, que opera como Centro de Investigación y Desarrollo Financiado por el Gobierno Federal (FFRDC) del DHS, ha registrado los derechos de autor de la lista CVE para el beneficio de la comunidad a fin de garantizar que siga siendo un estándar libre y abierto, así como para proteger legalmente el uso continuo de la misma y cualquier contenido resultante por parte del gobierno, los proveedores y/o los usuarios.

La Figura 1-1 muestra un ejemplo de un aviso de seguridad de Cisco que revela una vulnerabilidad en los productos de Cisco. Este aviso incluye un identificador de CVE e información detallada sobre la gravedad de la vulnerabilidad, la descripción, la configuración afectada, las correcciones y otro contenido relacionado con la vulnerabilidad.

![](img/20241023204843.png)

MITRE mantiene la lista CVE y su sitio web público, administra el Programa de compatibilidad CVE, supervisa las autoridades de numeración CVE (CNA) y brinda orientación técnica imparcial al Consejo editorial de CVE durante todo el proceso para garantizar que CVE sirva al interés público.
El objetivo de CVE es facilitar el intercambio de datos entre herramientas, repositorios de vulnerabilidades y servicios de seguridad. La Figura 1-2 muestra la entrada CVE en el sitio web CVE de MITRE para la vulnerabilidad abordada en el aviso de seguridad que se muestra en la Figura 1-1.

La Base de Datos Nacional de Vulnerabilidades (NVD) también mantiene una lista detallada de las vulnerabilidades reveladas en la industria. Se puede acceder a la NVD en https://nvd.nist.gov/, y ​​en la Figura 1-3 se muestra un ejemplo del mismo informe de vulnerabilidades en NVD.

![](img/20241023205054.png)

### ¿Qué es un exploit?
Un exploit se refiere a un software, una herramienta, una técnica o un proceso que se aprovecha de una vulnerabilidad que conduce al acceso, la escalada de privilegios, la pérdida de integridad o la denegación de servicio en un sistema informático. Los exploits son peligrosos porque todo el software tiene vulnerabilidades; los piratas informáticos y los perpetradores saben que existen vulnerabilidades y buscan aprovecharse de ellas. Aunque la mayoría de las organizaciones intentan encontrar y reparar vulnerabilidades, algunas organizaciones carecen de fondos, procesos, políticas y prácticas de diseño suficientes para proteger sus redes. A veces, nadie puede saber que existe la vulnerabilidad y se explota.

Eso se conoce como exploit de día cero. Incluso cuando sabe que hay un problema, tiene la carga del hecho de que existe una ventana entre el momento en que se divulga una vulnerabilidad y el momento en que hay un parche disponible para evitar el exploit. Cuanto más crítico es el servidor, más lento suele ser el parche. La administración puede tener miedo de interrumpir el servidor o de que el parche pueda afectar la estabilidad o el rendimiento. Por último, el tiempo necesario para implementar e instalar el parche de software en servidores y estaciones de trabajo de producción expone la infraestructura de TI de una organización a un período adicional de riesgo.

![](img/20241023205244.png)

Existen varios lugares donde las personas intercambian exploits con intenciones maliciosas. El más frecuente es la dark web. La dark web (o red oscura) es una superposición de redes y sistemas que utiliza Internet, pero requiere software y configuraciones específicas para acceder a ella. La dark web es solo una pequeña parte de la deep web. La deep web es una colección de información y sistemas en Internet que no está indexada por los motores de búsqueda web. A menudo, las personas confunden incorrectamente el término deep web con dark web.

No todos los exploits se comparten con intenciones maliciosas. Por ejemplo, muchos investigadores de seguridad comparten exploits de prueba de concepto (POC) en sitios públicos como The Exploit Database (o Exploit-DB) y GitHub. The Exploit Database es un sitio mantenido por Offensive Security donde los investigadores de seguridad y otras personas publican exploits para vulnerabilidades conocidas. Se puede acceder a la Exploit Database en www.exploit-db.com. La Figura 1-4 muestra un ejemplo de un exploit disponible públicamente en Exploit Database.

![](img/20241023205417.png)

### Riesgo, activos, amenazas y vulnerabilidades
Como sucede con cualquier tema de nueva tecnología, para comprender mejor el campo de la seguridad, debe aprender la terminología que se utiliza. Para ser un profesional de la seguridad, debe comprender la relación entre riesgo, amenazas, activos y vulnerabilidades.

El riesgo es la probabilidad o posibilidad de que ocurra o se materialice una amenaza. Hay tres elementos básicos del riesgo: activos, amenazas y vulnerabilidades. Para abordar el riesgo, el gobierno federal de los EE. UU. ha adoptado un Marco de gestión de riesgos (RMF). El proceso RMF se basa en los conceptos clave de seguridad de sistemas de información empresarial, rentable y basada en la misión y el riesgo. La Publicación especial 800-37 del NIST, “Guía para aplicar el Marco de gestión de riesgos a los sistemas de información federales”, transforma el proceso tradicional de Certificación y acreditación (C&A) en el RMF de seis pasos. Veamos los diversos componentes asociados con el riesgo, que incluyen activos, amenazas y vulnerabilidades.

Un activo es cualquier elemento de valor económico que posee una persona o una empresa. Los activos pueden ser reales (como enrutadores, servidores, discos duros y computadoras portátiles) o virtuales (como fórmulas, bases de datos, hojas de cálculo, secretos comerciales y tiempo de procesamiento). Independientemente del tipo de activo del que se trate, si este se pierde, se daña o se ve comprometido, puede suponer un coste económico para la organización.

Una amenaza establece el escenario para el riesgo y es cualquier agente, condición o circunstancia que podría causar daño, pérdida o comprometer un activo de TI o un activo de datos. Desde la perspectiva de un profesional de seguridad, las amenazas se pueden categorizar como eventos que pueden afectar la confidencialidad, integridad o disponibilidad de los activos de la organización. Estas amenazas pueden resultar en destrucción, divulgación, modificación, corrupción de datos o denegación de servicio. Algunos ejemplos de los tipos de amenazas que una organización puede enfrentar incluyen los siguientes:
- Desastres naturales, clima y daños catastróficos: huracanes, tormentas, cortes de energía, incendios, inundaciones, terremotos y otros eventos naturales componen una amenaza constante.
- Ataques de piratas informáticos: un interno o externo que no está autorizado y ataca deliberadamente la infraestructura, los componentes, los sistemas o los datos de una organización.
- Ciberataque: Atacantes que tienen como objetivo infraestructuras nacionales críticas, como plantas de agua, plantas eléctricas, plantas de gas, refinerías de petróleo, refinerías de gasolina, plantas de energía nuclear, plantas de gestión de residuos, etc. Stuxnet es un ejemplo de una de esas herramientas diseñadas precisamente para ese propósito.
- Virus y malware: Una categoría completa de herramientas de software que son maliciosas y están diseñadas para dañar o destruir un sistema o datos.
- Divulgación de información confidencial: Cada vez que se produce una divulgación de información confidencial, puede ser una amenaza crítica para una organización si dicha divulgación causa pérdida de ingresos, genera posibles responsabilidades o proporciona una ventaja competitiva a un adversario. Por ejemplo, si su organización sufre una infracción y se expone información detallada de los clientes (por ejemplo, información de identificación personal [PII]), dicha infracción podría tener posibles responsabilidades y pérdida de confianza de sus clientes. Otro ejemplo es cuando un actor de amenazas roba el código fuente o los documentos de diseño y los vende a sus competidores.
- Ataques de denegación de servicio (DoS) o de denegación de servicio distribuida (DDoS): un ataque contra la disponibilidad que está diseñado para poner de rodillas a la red, o al acceso a un host/servidor TCP/IP en particular, inundándolo con tráfico inútil. Hoy en día, la mayoría de los ataques DoS se lanzan a través de botnets, mientras que en el pasado se podían haber utilizado herramientas como Ping of Death y Teardrop. Al igual que con el malware, los piratas informáticos desarrollan constantemente nuevas herramientas DoS para que Storm y Mariposa, por ejemplo, sean reemplazadas por otras amenazas más actuales.
### Actores de amenazas
Los actores de amenazas son las personas (o un grupo de personas) que realizan un ataque o son responsables de un incidente de seguridad que afecta o tiene el potencial de afectar a una organización o individuo. Existen varios tipos de actores de amenazas:
- Script kiddies: estas personas utilizan "scripts" o herramientas existentes para hackear computadoras y redes. Carecen de la experiencia para escribir sus propios scripts.
- Grupos de crimen organizado: el objetivo principal de estos grupos es robar información, estafar a personas y ganar dinero.
- Patrocinadores estatales y gobiernos: estos agentes están interesados ​​en robar datos, incluidos datos de propiedad intelectual e investigación y desarrollo de los principales fabricantes, agencias gubernamentales y contratistas de defensa.
- Hacktivistas: estas personas llevan a cabo ataques de ciberseguridad destinados a promover una causa social o política.
- Grupos terroristas: estos grupos están motivados por creencias políticas o religiosas.
- 
Originalmente, el término hacker se usaba para un entusiasta de la informática. Un hacker era una persona que disfrutaba entendiendo el funcionamiento interno de un sistema, computadora y red informática y que continuaba hackeando hasta que entendía todo acerca del sistema. Con el tiempo, la prensa popular comenzó a describir a los hackers como individuos que irrumpían en las computadoras con intenciones maliciosas. La industria respondió desarrollando la palabra cracker, que es la abreviatura de hacker criminal. El término cracker fue desarrollado para describir a individuos que buscan comprometer la seguridad de un sistema sin el permiso de una parte autorizada.

Con toda esta confusión sobre cómo distinguir a los buenos de los malos, se acuñó el término hacker ético. Un hacker ético es un individuo que realiza pruebas de seguridad y otras actividades de evaluación de vulnerabilidad para ayudar a las organizaciones a proteger sus infraestructuras. A veces, a los hackers éticos se los conoce como hackers de sombrero blanco.

Los motivos e intenciones de los hackers varían. Algunos hackers son estrictamente legítimos, mientras que otros violan la ley de manera rutinaria. La Figura 1-5 muestra algunas de las categorías más comunes utilizadas en la industria para identificar a los hackers y sus motivos.
### Inteligencia sobre amenazas
La inteligencia sobre amenazas se refiere al conocimiento sobre una amenaza existente o emergente a los activos, incluidas las redes y los sistemas. La inteligencia sobre amenazas incluye contexto, mecanismos, indicadores de compromiso (IoC), implicaciones y consejos prácticos. La inteligencia sobre amenazas incluye detalles sobre las tácticas, técnicas y procedimientos de estos adversarios. El objetivo principal de la inteligencia sobre amenazas es informar las decisiones comerciales con respecto a los riesgos y las implicaciones asociadas con las amenazas.

![](img/20241023210145.png)

La conversión de estas definiciones en un lenguaje común podría traducirse en que la inteligencia de amenazas sea un conocimiento basado en evidencia de las capacidades de los actores de amenazas internos y externos.

Este tipo de datos puede ser beneficioso para el centro de operaciones de seguridad (SOC) de cualquier organización. La inteligencia de amenazas extiende la conciencia de la ciberseguridad más allá de la red interna al consumir inteligencia de otras fuentes de Internet relacionadas con posibles amenazas para usted o su organización. Por ejemplo, puede obtener información sobre amenazas que han afectado a diferentes organizaciones externas. Posteriormente, puede prepararse de manera proactiva en lugar de reaccionar una vez que se detecta la amenaza contra su red. Proporcionar una fuente de datos de enriquecimiento es un servicio que las plataformas de inteligencia de amenazas normalmente brindarían.

La Figura 1-6 muestra un proceso de inteligencia de amenazas de cinco pasos para evaluar las fuentes y la información de inteligencia de amenazas.

![](img/20241023210306.png)

En la actualidad, existen en el mercado muchas plataformas y servicios de inteligencia sobre amenazas diferentes. La inteligencia sobre amenazas cibernéticas se centra en brindar información útil sobre los adversarios, incluidos los indicadores de riesgo. Los feeds de inteligencia sobre amenazas lo ayudan a priorizar las señales de los sistemas internos contra amenazas desconocidas. La inteligencia sobre amenazas cibernéticas le permite concentrarse más en la investigación de ciberseguridad porque, en lugar de buscar ciegamente eventos “nuevos” y “anormales”, puede buscar indicadores de riesgo, direcciones IP, URL o patrones de explotación específicos.

Se están desarrollando varios estándares para difundir información de inteligencia sobre amenazas.
A continuación, se ofrecen algunos ejemplos:
- **Structured Threat Information eXpression (STIX)**: este lenguaje exprés está diseñado para compartir información sobre ciberataques. Los detalles de STIX pueden contener datos como direcciones IP o nombres de dominio de servidores de comando y control (a menudo denominados C2 o CnC), hashes de malware, etc. STIX fue desarrollado originalmente por MITRE y ahora lo mantiene OASIS. Puede obtener más información en http://stixproject.github.io.
- **Trusted Automated eXchange of Indicator Information (TAXII)**: este mecanismo de transporte abierto estandariza el intercambio automatizado de información sobre amenazas cibernéticas. TAXII fue desarrollado originalmente por MITRE y ahora lo mantiene OASIS. Puede obtener más información en http://taxiiproject.github.io.
- **Cyber ​​Observable eXpression (CybOX)**: este esquema estandarizado gratuito se utiliza para la especificación, captura, caracterización y comunicación de eventos de propiedades con estado que son observables en el dominio operativo. CybOX fue desarrollado originalmente por MITRE y ahora lo mantiene OASIS. Puede obtener más información en https://cyboxproject.github.io.
- **Open Indicators of Compromise (OpenIOC)**: este marco abierto se utiliza para compartir inteligencia sobre amenazas en un formato digerible por máquina. Obtenga más información en www.openioc.org.
- **Open Command and Control (OpenC2)**: este lenguaje se utiliza para el comando y control de tecnologías de ciberdefensa. El foro OpenC2 era una comunidad de partes interesadas en la ciberseguridad que fue facilitada por la Agencia de Seguridad Nacional de los EE. UU. OpenC2 es ahora un comité técnico (TC) y una especificación de OASIS. Puede obtener más información en www.oasis-open.org/committees/tc_home.php?wg_abbrev=openc2.

Cabe señalar que también se pueden aprovechar muchas fuentes de código abierto y no relacionadas con la seguridad para obtener información sobre amenazas. Algunos ejemplos de estas fuentes son las redes sociales, los foros, los blogs y los sitios web de los proveedores.
### Plataforma de inteligencia de amenazas

59