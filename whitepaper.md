# ELECTRONIC & DIGITAL SERVICES P2P MARKET
## Multi-Currency Settlement Whitepaper

**Versión:** 0.1 — Borrador fundacional  
**Estado:** Propuesta conceptual para revisión técnica, económica y legal  
**Idioma:** Español  
**Fecha:** 11 de octubre de 2026  
**Nombre de trabajo de la red:** Red descentralizada de producción y distribución de servicios digitales y electrónicos

> Este documento expresa una arquitectura propuesta. No afirma que exista una red operativa, un activo emitido, una integración con exchanges, una auditoría independiente ni una garantía de precio o rentabilidad. Los parámetros de consenso, emisión, recompensas y liquidación deberán definirse, probarse y auditarse antes de cualquier lanzamiento.

---

## Manifiesto

Proponemos una red descentralizada para producir, identificar, verificar, comercializar y distribuir unidades criptográficas vinculadas a servicios y productos digitales y electrónicos. La red conecta productores, mineros, proveedores u holders, mayoristas, distribuidores minoristas, mercados, exchanges compatibles y consumidores mediante protocolos modulares e interoperables.

La minería no se concibe únicamente como emisión de monedas. El diseño contempla una capa de consenso basada en Scrypt y un conjunto de protocolos de producción y trazabilidad que pueden registrar las etapas comerciales y operativas de las unidades: emisión, identificación, transferencia, instalación, activación, periodo de uso, renovación, suspensión, bloqueo, congelamiento, cancelación, revocación, quemado, consumo y reutilización cuando el producto lo permita.

La identidad criptográfica de una unidad se mantiene separada de su precio comercial y de la moneda utilizada para pagarla. Una misma unidad puede cotizarse o liquidarse mediante distintos instrumentos admitidos, de acuerdo con las reglas de cada mercado y la disponibilidad de los mecanismos de pago. La multiliquidación no garantiza un valor estable: permite separar el objeto comercial de los medios utilizados para liquidar la operación.

La red busca organizar una cadena de producción de servicios digitales y electrónicos donde cada participante tenga un papel definido y donde las recompensas se relacionen con trabajo válido, verificable y financiable. La meta es que el protocolo pueda extenderse por módulos sin confundir producción con tenencia, venta mayorista con distribución minorista, registro con prueba del acontecimiento, ni liquidación con identidad del activo.

## 1. Resumen ejecutivo

Electronic & Digital Services P2P Market (en adelante, **EDSPM**) es una propuesta para una red descentralizada y una familia de protocolos orientados a la producción y comercialización entre pares (*peer-to-peer*, P2P) de servicios y productos digitales y electrónicos.

El modelo integra seis planos principales:

1. **Red y consenso:** reglas comunes para validar el estado compartido y ordenar transacciones.
2. **Minería Scrypt:** mecanismo de prueba de trabajo propuesto para asegurar la cadena de bloques, sujeto a una especificación propia y a pruebas de seguridad.
3. **Producción y extensiones:** reglas para presentar, identificar y emitir unidades criptográficas ligadas a prestaciones autorizadas.
4. **Ciclo de vida y trazabilidad:** registro verificable de los acontecimientos pertinentes de cada unidad, desde su emisión hasta su consumo o retirada.
5. **Cadena comercial:** proveedores/holders, vendedores mayoristas, distribuidores minoristas, mercados y consumidores.
6. **Liquidación monetaria múltiple:** posibilidad de negociar una unidad usando distintas monedas o instrumentos de pago admitidos, sin alterar por ello su identidad criptográfica.

EDSPM distingue entre el trabajo de consenso de la red y el trabajo de verificación de eventos comerciales. La prueba de trabajo Scrypt puede contribuir a elegir y proteger la historia de bloques; no demuestra por sí sola que una licencia externa sea legítima, que un software se haya instalado o que un servicio se haya consumido. Esos hechos requieren reglas de autorización y evidencias adicionales, como firmas de emisores, respuestas autenticadas de proveedores, atestaciones o integraciones verificables.

Las recompensas a mineros y verificadores deberán financiarse mediante fuentes explícitas —por ejemplo, subsidios protocolarios predefinidos, comisiones, tarifas de servicio o ingresos comerciales— y no por la mera creación de eventos. No se propone garantizar precios, beneficios, liquidez, aceptación universal ni listados en exchanges.

## 2. Problema y oportunidad

Los bienes y derechos digitales se comercializan a través de sistemas heterogéneos: licencias, suscripciones, códigos, créditos, certificados, aplicaciones, servicios de API, contenido digital y otras prestaciones. Sus inventarios, permisos, transferencias y estados de uso suelen depender de los sistemas particulares de cada proveedor.

Una infraestructura común podría facilitar la identificación de unidades, la trazabilidad de cambios, el abastecimiento entre mayoristas y distribuidores y la liquidación mediante distintos medios de pago. Sin embargo, una red compartida solo aporta valor si resuelve problemas concretos mejor que alternativas más simples, como bases de datos firmadas, APIs, credenciales verificables o contratos inteligentes.

EDSPM plantea investigar si una arquitectura modular descentralizada puede:

- mantener una identidad criptográfica verificable por unidad;
- distinguir producto, versión, condiciones y unidad individual;
- registrar procedencia, titularidad y cambios de estado;
- coordinar producción y canales comerciales con permisos definidos;
- remunerar tareas de verificación cuando exista trabajo real y financiación suficiente;
- separar el activo negociado de la moneda de liquidación;
- permitir integraciones sin asumir que todos los proveedores o exchanges adoptarán el protocolo.

## 3. Objetivos y límites

### 3.1 Objetivos

- Diseñar una red descentralizada para la producción y distribución de servicios digitales y electrónicos.
- Definir un protocolo de minería basado en Scrypt, con parámetros explícitos y auditables.
- Establecer protocolos de extensión para incorporar nuevas clases de unidades y servicios.
- Separar los roles de productor, minero/verificador, holder/proveedor, mayorista, distribuidor, exchange y consumidor.
- Definir una identidad criptográfica por unidad y un historial de ciclo de vida.
- Diseñar un modelo de recompensas que desaliente eventos ficticios y evite pagos duplicados.
- Permitir liquidaciones en distintos medios monetarios, sujetos a las integraciones disponibles.

### 3.2 Fuera de alcance en esta fase

Este whitepaper no afirma que EDSPM ya tenga una blockchain desplegada, moneda emitida, mercado líquido, acuerdos con proveedores, listados confirmados en exchanges, licencia de software, garantía de recompra ni validación jurídica. Tampoco define todavía parámetros finales de dificultad, subsidio por bloque, suministro máximo, comisiones, tipo de cambio de referencia o fórmula exacta de recompensas.

## 4. Participantes y responsabilidades

| Participante | Responsabilidad propuesta | Evidencia o control requerido |
|---|---|---|
| Red y nodos validadores | Mantener el estado común y verificar reglas de consenso | Reglas públicas, software reproducible y verificaciones de protocolo |
| Mineros Scrypt | Aportar prueba de trabajo para la producción de bloques | Encabezados, hashes y criterios de dificultad verificables |
| Mineros/verificadores de eventos | Validar tareas de trazabilidad cuando el protocolo lo habilite | Evidencia firmada, prueba del evento y prevención de duplicados |
| Productor/emisor | Crear o presentar unidades que está autorizado a emitir | Firma, contrato, autorización o prueba de procedencia |
| Holder/proveedor | Adquirir, custodiar y abastecer inventario | Historial de titularidad, permisos y registros de compra/venta |
| Vendedor mayorista | Vender lotes a distribuidores o comerciantes autorizados | Condiciones comerciales, inventario y órdenes verificables |
| Distribuidor minorista | Comercializar unidades al usuario final | Habilitación, precio y condiciones de la oferta |
| Proveedor del servicio | Reconocer, activar o atender la prestación representada | API, firma, atestación o comprobante verificable |
| Mercado o exchange | Facilitar órdenes o intercambio según sus propias reglas | Integración técnica, admisión y liquidación confirmada |
| Cliente final | Comprar, transferir o consumir la unidad conforme a las condiciones | Prueba de pago cuando corresponda y eventos de uso pertinentes |

Los roles pueden combinarse en una misma entidad o separarse en varias. Las restricciones de un contrato inteligente no sustituyen los contratos, permisos o licencias requeridos fuera de la cadena.

## 5. Arquitectura modular

EDSPM se concibe como una familia de protocolos, no como una sola función monolítica.

### 5.1 Capa de red y consenso

Define formatos de transacción y bloque, reglas de validez, propagación P2P, selección de cadena, ajuste de dificultad, finalización práctica y recuperación ante fallos. El mecanismo concreto de consenso requiere análisis de seguridad y simulación antes de fijarse.

### 5.2 Capa de minería Scrypt

Scrypt se propone como función de prueba de trabajo para minar bloques. Scrypt es una función de derivación de claves intensiva en memoria que ha sido adaptada en determinadas redes para prueba de trabajo; Litecoin, por ejemplo, documenta su uso con parámetros específicos [1]. EDSPM no debe copiar automáticamente esos parámetros: deberá definir su propio formato de encabezado, parámetros, objetivo de dificultad, intervalo de bloque, ajuste de dificultad y reglas de emisión, y revisar la compatibilidad del hardware que pretende admitir.

La prueba de trabajo ofrece una forma de costear la reescritura del historial, pero tiene costes energéticos y riesgos de concentración de hardware o poder de hash. La seguridad dependerá de la distribución real del poder de minería, el diseño de incentivos y los supuestos de amenaza; el uso de Scrypt no garantiza descentralización por sí solo.

### 5.3 Capa de producción y extensión

Cada protocolo de extensión debe definir un esquema de unidad: clase de servicio, productor autorizado, versión, condiciones, suministro, transferibilidad, duración, región si aplica, política de revocación y fuente de evidencia. Una extensión no debe poder declarar legítimo un derecho que el emisor no está autorizado a conceder.

### 5.4 Capa de identidad y trazabilidad

Registra la identidad criptográfica, la relación con el producto, la procedencia y el historial de cambios. Puede apoyarse en hashes de contenido, firmas digitales, registros de eventos y almacenamiento externo de datos voluminosos. Los datos personales y secretos comerciales no deberían publicarse sin necesidad en una cadena pública.

### 5.5 Capa de mercados y cadena comercial

Administra órdenes o referencias a órdenes, permisos por canal, lotes, inventario, márgenes declarados y transferencias entre niveles. La arquitectura puede definir protocolos distintos para venta primaria, abastecimiento mayorista y venta minorista; no es obligatorio que todas las operaciones ocurran dentro de la blockchain.

### 5.6 Capa de liquidación monetaria múltiple

Representa las opciones de pago admitidas y su estado. La liquidación puede realizarse en monedas fiduciarias, criptoactivos, stablecoins u otros instrumentos compatibles, sujeto a proveedores de pago, puentes, custodia, regulación y reglas de mercado. La red debe registrar qué moneda se cotizó, cuál se recibió, el tipo de cambio utilizado, las comisiones, la fecha de fijación de precio y la confirmación definitiva.

## 6. Modelo de unidades e identificadores

EDSPM debe diferenciar cuatro conceptos:

1. **Identificador del producto o clase:** señala qué servicio, licencia o certificado se ofrece.
2. **Identificador de versión y condiciones:** define la versión del servicio y las condiciones aplicables.
3. **Identificador individual de unidad:** identifica una unidad comercial específica.
4. **Identificador de evento:** identifica una transición o acción en el ciclo de vida de esa unidad.

La unicidad puede implementarse mediante identificadores derivados de un espacio de nombres, un número de serie, una raíz criptográfica o una combinación firmada de atributos. El método definitivo requiere análisis de colisiones, privacidad, capacidad de auditoría y migración de versiones.

Un identificador único no prueba por sí mismo la existencia ni la legitimidad del derecho. El protocolo debe validar quién emitió la unidad, qué autorizaciones tiene y qué evidencia respalda los atributos declarados.

Cuando proceda, los modelos de credenciales verificables pueden aportar conceptos útiles para expresar afirmaciones de emisores y verificarlas criptográficamente [2]. Los estándares de token existentes, como ERC-1155, también muestran cómo representar múltiples tipos de tokens y transferencias por lotes, aunque no resuelven por sí solos la autorización comercial ni la veracidad de eventos externos [3]. EDSPM deberá comparar reutilizar estándares existentes frente a desarrollar un formato propio.

## 7. Ciclo de vida de una unidad

Los siguientes estados son un modelo de referencia; no todos aplican a todos los productos.

1. **Propuesta:** un productor presenta una unidad o lote.
2. **Autorización:** se valida que el emisor tiene derecho a crear o registrar la unidad.
3. **Identificación:** se asignan o verifican los identificadores de producto, versión y unidad.
4. **Verificación:** se revisan procedencia, condiciones, duplicación y evidencia exigida.
5. **Consenso y registro:** la red acepta o rechaza la transacción según las reglas vigentes.
6. **Venta primaria:** la unidad pasa del productor al holder/proveedor autorizado.
7. **Abastecimiento mayorista:** el proveedor vende o asigna inventario a mayoristas o distribuidores.
8. **Distribución minorista:** la unidad queda disponible para el cliente final a través de un canal compatible.
9. **Instalación o activación:** se registra el acontecimiento si la prestación lo requiere y hay evidencia verificable.
10. **Periodo y renovación:** se gestiona la vigencia, renovación o expiración de acuerdo con las condiciones.
11. **Transferencia o reventa:** se registra un cambio de titularidad si la licencia y las reglas lo permiten.
12. **Suspensión, bloqueo o congelamiento:** se aplica una restricción temporal con motivo, autoridad y condiciones de desbloqueo definidos.
13. **Cancelación, revocación o quemado:** se registra el fin del derecho o su retirada irreversible de circulación, según el tipo de unidad.
14. **Consumo o reutilización:** se confirma el consumo final o se permite reutilización únicamente si la especificación del producto lo autoriza.

La máquina de estados debe impedir transiciones incompatibles. Por ejemplo, una unidad quemada no puede volver a ser transferible salvo que exista una operación de recuperación explícitamente diseñada, segura y auditable. Toda excepción debe estar especificada y no quedar a criterio informal de un operador.

## 8. Minería, verificación y recompensas

### 8.1 Dos clases de trabajo

EDSPM distingue entre:

- **Trabajo de consenso:** prueba de trabajo Scrypt para contribuir a la producción y protección de bloques.
- **Trabajo de trazabilidad:** tareas autorizadas para comprobar registros y evidencias de eventos comerciales o de servicio.

No son equivalentes. Scrypt prueba que se ha encontrado un hash bajo un objetivo; no demuestra que una licencia haya sido activada o que una suscripción se haya consumido. Los eventos requieren pruebas específicas y reglas de aceptación. La red puede agrupar verificaciones y eventos en lotes para reducir costes sin exigir una nueva prueba de trabajo completa por cada cambio de estado.

### 8.2 Eventos que pueden generar trabajo remunerable

Sujeto a la especificación final, las tareas podrían incluir identificación inicial, verificación de procedencia, incorporación de lote, comprobación de una transferencia, registro de instalación o activación, validación de un periodo, renovación, suspensión, cancelación, revocación, quemado y consumo. La remuneración solo debe ocurrir cuando el evento está autorizado, es verificable, no está duplicado y su coste está cubierto por el modelo económico.

### 8.3 Principios de recompensa

La contabilidad debe distinguir la recompensa por bloque, las tarifas de transacción, las tarifas de verificación de eventos y cualquier pago comercial fuera de la cadena. Una fórmula conceptual sería:

**Recompensa del participante = participación válida en recompensas de consenso + tarifas asignadas por eventos aceptados − penalizaciones previstas por fraude probado.**

Esta expresión es un marco, no una fórmula final. Los pesos por evento, la medición de contribución, los límites por unidad y los procesos de apelación deben definirse en el protocolo.

Las salvaguardas deben evitar pagos duplicados, eventos creados entre cuentas relacionadas para extraer recompensas, colusión entre verificadores, abuso de identidades y emisión de unidades sin demanda o autorización. La penalización económica (*slashing*) solo debería aplicarse con reglas públicas, evidencia suficiente y un proceso de revisión definido.

### 8.4 Fuentes de financiación

Las recompensas podrían financiarse mediante una combinación explícita de subsidio protocolario temporal, tarifas de transacción, tarifas de verificación, tarifas de emisión y/o ingresos comerciales. Debe publicarse qué fuente paga cada clase de recompensa y qué ocurre cuando los ingresos son insuficientes. La red no puede prometer continuidad rentable de la minería solo por existir eventos de trazabilidad.

## 9. Mercado P2P y cadena comercial

El flujo comercial de referencia es:

**Productor/emisor → holder/proveedor → vendedor mayorista → distribuidor minorista → mercado o exchange compatible → consumidor.**

Este flujo es conceptual, no necesariamente lineal. Algunos participantes pueden cumplir más de una función; ciertas unidades podrían venderse directamente si la política comercial lo permite. Los límites de canal deben responder a acuerdos comerciales explícitos, no asumirse como protección técnica absoluta.

### Productores

Producen, emiten o presentan las unidades y acreditan la autorización para representar el servicio o derecho descrito.

### Holders/proveedores

Compran o custodian inventario, organizan el abastecimiento y responden según los contratos aplicables. Tener una unidad no equivale automáticamente a estar autorizado para emitirla o modificar sus condiciones.

### Mayoristas

Distribuyen lotes, pueden gestionar precios escalonados, inventario territorial y términos comerciales. Los márgenes son variables comerciales y no rendimientos garantizados.

### Distribuidores minoristas

Ofrecen las unidades a clientes finales, informan condiciones, atienden soporte y procesan las operaciones de consumo o devolución conforme al producto.

### Exchanges y mercados globales

La visión contempla interoperabilidad con mercados y exchanges internacionales. Ningún protocolo puede garantizar que todos los exchanges del mundo acepten, listen o mantengan negociable un activo. Cada operador decide su admisión, evalúa compatibilidad y puede estar sujeto a requisitos legales, de custodia y de liquidez. EDSPM debe proveer APIs y formatos de integración, no asumir listados universales.

## 10. Multiliquidación monetaria

La multiliquidación separa el activo objeto del negocio de la moneda utilizada para pagar la operación.

Una orden debe especificar al menos:

- unidad comercial y cantidad;
- precio y moneda de cotización;
- moneda o instrumento aceptado para el pago;
- fuente y hora del tipo de cambio, cuando se necesite conversión;
- comisiones y quién las paga;
- vencimiento de la cotización;
- mecanismo de confirmación y finalización;
- tratamiento de pagos parciales, retrasos, errores, devoluciones o reembolsos.

Por ejemplo, un producto podría publicarse a un precio de referencia en USD, mientras la compraventa se liquide en CRC o en un criptoactivo, siempre que comprador y vendedor acepten ese método y exista una vía de liquidación verificable. El equivalente no será constante si cambia el tipo de cambio. Una unidad con varias monedas de liquidación no posee necesariamente un precio de mercado estable.

Para operaciones entre cadenas o redes, se requerirán mecanismos como escrow, swaps atómicos o intermediarios de liquidación, según el caso. Cada opción tiene riesgos: congestión, fallos de puente, riesgo de contraparte, volatilidad, confirmaciones incompletas y discrepancias entre proveedores de precio. El whitepaper técnico posterior deberá elegir qué mecanismos se implementan y cuáles quedan fuera del protocolo base.

La tokenización y las plataformas programables se están investigando también para liquidación multidivisa institucional; por ejemplo, el Banco de Pagos Internacionales publicó en 2026 resultados de Project Agorá sobre una plataforma programable de liquidación mayorista multidivisa [4]. Esa iniciativa tiene un alcance institucional distinto y no demuestra por sí sola la viabilidad de EDSPM.

## 11. Precios, liquidez y sostenibilidad

El precio de emisión, el precio mayorista, el precio minorista y el precio secundario son variables distintas.

- **Precio de emisión:** precio o regla de valoración al incorporarse la unidad al inventario.
- **Precio mayorista:** precio acordado entre proveedores y compradores mayoristas.
- **Precio minorista:** precio ofrecido al cliente final.
- **Precio secundario:** resultado de órdenes de compra y venta en un mercado.
- **Moneda de liquidación:** instrumento con el que se realiza el pago.

La red puede definir precios de referencia o límites contractuales para ciertos canales, pero no puede asegurar el precio secundario sin mecanismos de respaldo, reservas, obligaciones de recompra y liquidez suficientes. Cualquier promesa de recompra debe especificar quién la financia, las condiciones, los límites y los riesgos. La estabilidad de precio no debe confundirse con una consecuencia automática de utilizar criptografía.

La sostenibilidad debe evaluarse mediante demanda real, coste de producción del servicio, tarifas, devoluciones, fraude, costes de distribución, recompensas, soporte y capital de trabajo. La emisión debe ajustarse a la capacidad del proveedor y a señales de demanda, evitando inventarios indefinidos sin comprador.

## 12. Seguridad, privacidad y modelo de amenazas

El diseño debe contemplar, como mínimo:

- doble emisión o duplicación de derechos;
- emisor no autorizado o claves comprometidas;
- datos falsos o eventos simulados;
- colusión entre mineros y verificadores;
- ataques Sybil y concentración del poder de hash;
- censura, reorganizaciones de cadena y fallos de disponibilidad;
- abuso de privilegios de bloqueo, congelamiento o revocación;
- errores de contratos inteligentes y extensiones incompatibles;
- fallos de puente, custodia o liquidación;
- fuga de datos personales o secretos comerciales;
- fraude de reventa, reclamaciones y uso simultáneo no permitido.

Las medidas previstas incluyen firmas digitales, rotación y recuperación de claves, permisos limitados, registros de auditoría, validación de estado, pruebas de integración, revisiones de código, límites de emisión y mecanismos de apelación. La información personal o comercial sensible debería minimizarse y mantenerse fuera de la cadena cuando no sea indispensable. Los hashes aportan integridad de datos, pero no demuestran por sí solos la verdad del contenido original.

## 13. Gobernanza y actualizaciones

La gobernanza deberá definir quién propone cambios, cómo se publican las especificaciones, qué pruebas se exigen, cómo se evalúan actualizaciones y qué mecanismos existen para migraciones o emergencias. Debe diferenciarse gobernanza del consenso, gobernanza de extensiones comerciales y administración de servicios externos.

Ninguna autoridad de extensión debería poder cambiar unilateralmente una unidad ya emitida de forma que altere sus derechos sin una regla de actualización previamente conocida. Las acciones de emergencia, como congelamientos o revocaciones, requieren condiciones, autoridad, evidencia, alcance y registro auditables.

Las decisiones iniciales pendientes incluyen: parámetros de Scrypt, estrategia de ajuste de dificultad, tiempos de bloque, modelo de emisión, clases de activos, tipos de cuenta, finalización, gobernanza y plan de transición si el protocolo se actualiza.

## 14. Métricas de éxito

El piloto debería medir indicadores técnicos, operativos y económicos:

- tiempo y coste de registrar una unidad;
- coste medio por evento de ciclo de vida;
- tasa de eventos aceptados, rechazados y disputados;
- duplicaciones detectadas y falsos positivos;
- disponibilidad y latencia de la red;
- concentración de hash y distribución de validadores;
- proporción de eventos con evidencia externa verificable;
- coste total de recompensas frente a ingresos atribuibles;
- tiempo de liquidación por moneda y tasa de fallos;
- inventario sin vender y tiempo hasta el consumo final;
- tasa de fraude, devoluciones y reclamaciones;
- coste total para el productor y precio final para el consumidor.

## 15. Hoja de ruta de implementación

### Fase 0 — Especificación

Cerrar glosario, actores, modelo de unidad, estados, amenazas, esquema de recompensa y límites del alcance. Publicar decisiones de diseño y cuestiones aún abiertas.

### Fase 1 — Prototipo de identidad y trazabilidad

Implementar unidades de prueba, emisores firmados, historial de eventos y validadores. Comparar el coste frente a un registro convencional y a estándares existentes.

### Fase 2 — Testnet de consenso

Implementar y probar el diseño Scrypt: parámetros, ajuste de dificultad, nodos, bloques, reorganizaciones y recuperación. Realizar análisis de seguridad y resistencia a ataques.

### Fase 3 — Mercado de prueba

Usar un servicio digital propio o expresamente autorizado. Simular producción, holder/proveedor, mayorista, distribuidor, compra minorista, activación, renovación y cancelación.

### Fase 4 — Liquidación múltiple controlada

Integrar dos o más medios de pago en entorno de pruebas. Medir cotización, tipo de cambio, conciliación, fallos y recuperación de transacciones.

### Fase 5 — Auditoría y piloto limitado

Solicitar revisión independiente de seguridad, economía, privacidad, contratos y obligaciones regulatorias aplicables. Publicar resultados, limitaciones y riesgos pendientes.

### Fase 6 — Lanzamiento condicionado

Solo considerar el despliegue público cuando el protocolo, el modelo económico, los proveedores, las reglas de gobernanza, las respuestas a incidentes y los requisitos legales estén suficientemente definidos y probados.

## 16. Preguntas que el whitepaper técnico debe resolver

1. ¿La unidad extraída es el activo nativo de la red, una unidad de servicio o una combinación diferenciada?
2. ¿Qué exactamente se mina mediante Scrypt y qué se verifica mediante pruebas de evento?
3. ¿Cuál es el algoritmo de consenso completo y qué supuestos de seguridad tiene?
4. ¿Quién puede emitir cada unidad y cómo se acredita su autorización?
5. ¿Qué fuente financia cada clase de recompensa y cómo se fija su límite?
6. ¿Cómo se previenen eventos artificiales, autoconsumo y colusión?
7. ¿Cómo se representan los derechos transferibles, no transferibles, consumibles y renovables?
8. ¿Qué sucede si un proveedor externo cierra, cambia sus términos o deja de reconocer una unidad?
9. ¿Qué monedas y vías de pago se admitirán inicialmente, y quién asume sus riesgos?
10. ¿Qué controles dependen del protocolo y cuáles dependen de acuerdos contractuales o de operadores externos?

## 17. Conclusión

EDSPM propone una red descentralizada para conectar la producción de unidades criptográficas relacionadas con servicios digitales y electrónicos con su abastecimiento, comercialización, distribución y ciclo de vida. La minería Scrypt forma parte de la capa de consenso propuesta; los protocolos de producción, identificación y trazabilidad describen los activos y sus eventos; los participantes comerciales distribuyen las unidades; y la multiliquidación separa la identidad del activo de los medios de pago.

La solidez del proyecto no dependerá de la cantidad de componentes anunciados, sino de demostrar que funcionan juntos de manera verificable y económicamente sostenible. El siguiente paso es convertir este manifiesto en una especificación: decidir el modelo exacto de unidad, diseñar la minería y el consenso, establecer pruebas fiables para eventos externos, simular la economía de las recompensas y validar un caso comercial real.

**Principio rector:** identificar cada unidad, verificar quién está autorizado a emitirla, registrar los cambios relevantes de su ciclo de vida, distribuirla mediante reglas transparentes y permitir que las operaciones se liquiden en los medios monetarios que el sistema admita, sin confundir identidad, derecho comercial, precio y pago.

## Glosario

- **Activo o unidad criptográfica:** registro digital identificable y transferible según las reglas del protocolo.
- **Unidad de servicio:** unidad que representa o referencia una licencia, código, certificado o prestación digital autorizada.
- **Scrypt:** función criptográfica utilizada por algunas redes como base de su prueba de trabajo.
- **Prueba de trabajo (PoW):** mecanismo que exige producir una prueba computacional verificable para participar en la producción o aceptación de bloques, según el protocolo.
- **Trazabilidad:** historial verificable de procedencia, titularidad y cambios de estado.
- **Holder/proveedor:** participante que adquiere o mantiene inventario y abastece otros canales comerciales.
- **Mayorista:** comerciante que distribuye unidades en lotes o bajo condiciones mayoristas.
- **Distribuidor minorista:** participante que ofrece las unidades al mercado final.
- **Liquidación monetaria múltiple:** posibilidad de realizar pagos de una operación utilizando distintos medios monetarios admitidos.
- **Quemado:** registro de retirada permanente de una unidad de la circulación protocolaria.
- **Evento verificable:** acontecimiento aceptado por la red según pruebas y reglas predefinidas; el registro no elimina la necesidad de probar los hechos externos.

## Referencias técnicas

[1] Litecoin, “Proof of Work,” Learning Center. Explica el uso de Scrypt como prueba de trabajo en Litecoin y documenta parámetros específicos de esa implementación. https://litecoin.com/learning-center/proof-of-work

[2] W3C, “Verifiable Credentials Data Model v2.0,” W3C Recommendation, 15 de mayo de 2025. https://www.w3.org/TR/2025/REC-vc-data-model-2.0-20250515/

[3] Ethereum Improvement Proposals, “EIP-1155: Multi Token Standard.” Especificación de una interfaz para administrar múltiples tipos de tokens. https://eips.ethereum.org/EIPS/eip-1155

[4] Bank for International Settlements, “Project Agorá: a shared programmable platform for wholesale cross-border payments,” 27 de mayo de 2026. https://www.bis.org/publications/project-agora-shared-programmable-platform-wholesale-cross-border-payments

[5] Satoshi Nakamoto, “Bitcoin: A Peer-to-Peer Electronic Cash System,” 2008. Referencia histórica para el diseño de una red P2P con prueba de trabajo. https://bitcoin.org/bitcoin.pdf

---

**Aviso:** borrador conceptual; no constituye asesoría financiera, jurídica o fiscal, oferta de inversión ni garantía de rendimiento. Validar técnica, económica y legalmente antes de implementarlo.
