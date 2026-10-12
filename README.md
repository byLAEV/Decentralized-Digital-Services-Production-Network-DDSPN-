# Scrypt Mining & Distribution Network (SMDN)

> **Estado:** diseño conceptual. Este repositorio define la propuesta inicial de una red descentralizada y su conjunto de protocolos; todavía no representa una red operativa ni una implementación auditada.

## Descripción del repositorio

Red descentralizada con minería Scrypt y protocolos modulares de producción, extensión, proveedores/holders, venta mayorista y distribución minorista. Las unidades criptográficas siguen su trazabilidad comercial y admiten liquidación en múltiples monedas y acceso a mercados y exchanges globales.

## Visión

SMDN propone una red descentralizada de minería y comercio digital en la que la minería no se limita a emitir una moneda. El protocolo contempla la creación, identificación, verificación y trazabilidad de unidades criptográficas asociadas a productos, servicios, licencias, certificados u otras unidades comerciales digitales autorizadas.

La red separa la unidad criptográfica de su valor comercial y de la moneda utilizada para pagarla. Una misma unidad puede conservar su identidad mientras cambia de titular o se negocia en distintos mercados; el precio, la moneda de cotización y la moneda de liquidación son parámetros independientes.

La arquitectura se organiza en protocolos modulares para que la producción, el abastecimiento, la venta mayorista, la distribución minorista y la integración con exchanges puedan tener reglas diferenciadas, pero interoperables.

## Componentes de la red

### 1. Protocolo base y consenso

Define las reglas comunes de la red: participantes, validación, formato de transacciones, registro de estados, prevención de duplicaciones y consenso. La utilización de Scrypt debe concretarse en la especificación técnica: algoritmo de prueba de trabajo, parámetros, ajuste de dificultad, emisión, validación de bloques y compatibilidad con el hardware y software previstos.

### 2. Protocolo de minería

Los mineros aportan trabajo conforme a las reglas de la red. El trabajo puede abarcar la seguridad del consenso y tareas verificables relacionadas con las unidades comerciales, según lo que determine el diseño final. Las recompensas, tarifas y responsabilidades se especificarán de forma que no se remuneren eventos duplicados o artificiales.

### 3. Protocolos de producción y extensión

Definen cómo se incorporan nuevas clases de unidades, productos, servicios o funciones a la red. Cada extensión deberá establecer el formato de la unidad, quién está autorizado a emitirla, sus condiciones, sus estados válidos y las pruebas requeridas para reconocerla. La extensión del protocolo no debe permitir crear derechos comerciales que el emisor no esté autorizado a conceder.

### 4. Protocolo de proveedores y holders

Regula la adquisición y custodia de inventario por participantes que operan como proveedores o holders. Los productores pueden vender las unidades primarias a proveedores habilitados conforme a los permisos y contratos definidos; las reglas del protocolo distinguirán la producción de la tenencia y la reventa.

### 5. Protocolo de venta mayorista

Organiza la venta de inventario a distribuidores o comerciantes autorizados. Puede contemplar lotes, precios de salida, órdenes, asignaciones, límites, regiones y condiciones comerciales. Los márgenes y restricciones deben resultar de reglas explícitas o contratos, no de suposiciones implícitas del protocolo.

### 6. Protocolo de distribución minorista

Permite que distribuidores y vendedores acerquen las unidades al cliente final, incluyendo canales digitales y territoriales. Los requisitos de transferencia, uso, devolución, expiración y reventa dependerán de las características del producto o servicio representado.

### 7. Integración con mercados y exchanges

La arquitectura prevé integración con mercados y exchanges a escala internacional. La inclusión efectiva de una unidad en un exchange dependerá de la compatibilidad técnica, las reglas de admisión, la liquidez, los requisitos del operador y la normativa aplicable. El protocolo no puede garantizar que todos los exchanges del mundo vayan a listar sus activos.

### 8. Liquidación monetaria múltiple

La unidad criptográfica mantiene su identidad con independencia del medio de pago. Una compraventa puede cotizarse o liquidarse en monedas fiduciarias, criptoactivos u otros instrumentos admitidos. Cada integración debe definir el tipo de cambio, las comisiones, la confirmación del pago, la liquidación fallida y el tratamiento de disputas.

## Ciclo de vida de las unidades

Según el producto y sus condiciones, una unidad puede pasar por estados como:

1. **Propuesta o emisión:** presentación por un emisor autorizado.
2. **Identificación:** asignación o verificación de un identificador individual y de la clase de producto.
3. **Validación:** verificación de procedencia, permisos, versión, condiciones y ausencia de duplicación dentro del sistema.
4. **Consenso y registro:** aceptación o rechazo conforme a las reglas de la red.
5. **Venta primaria:** transferencia desde producción al canal de proveedores autorizado.
6. **Venta mayorista y distribución:** transferencia por los canales comerciales habilitados.
7. **Instalación o activación:** registro de esos eventos si el servicio los requiere y existe evidencia verificable.
8. **Periodo, renovación o transferencia:** administración de los estados admitidos por el derecho digital.
9. **Suspensión, bloqueo o congelamiento:** restricción temporal conforme a las condiciones y facultades establecidas.
10. **Cancelación, revocación, expiración o quemado:** cierre o retiro de circulación según las reglas de esa unidad.
11. **Consumo o reutilización:** cierre definitivo o retorno a un estado reutilizable cuando el producto lo permita.

No todas las unidades admiten todos los estados. Un registro en la cadena no demuestra, por sí solo, que una instalación, activación o consumo externo haya ocurrido: esos hechos necesitan una fuente autorizada, una firma, una atestación o una integración verificable.

## Función y recompensas de los mineros

El modelo contempla recompensar trabajo válido en distintas fases, según las reglas de consenso y servicio que finalmente se adopten: seguridad de red, identificación, verificación de procedencia, registro de cambios de estado y trazabilidad de eventos autorizados.

El diseño económico deberá especificar:

- qué trabajo se recompensa y cómo se demuestra;
- cómo se evita pagar varias veces por un mismo evento;
- cómo se detectan autoconsumo artificial, colusión y eventos ficticios;
- qué fuentes financian las recompensas;
- cómo se limita la emisión y se mantiene la sostenibilidad económica;
- cómo se distribuyen las recompensas entre minería, verificación y otras funciones de la red.

El hecho de registrar un evento no genera ingresos automáticamente. Las recompensas requieren una fuente de financiación explícita, como comisiones, tarifas de servicio, ingresos comerciales u otro mecanismo definido y auditable.

## Principios de diseño

- **Descentralización:** las reglas de consenso y validación deben ser públicas y verificables.
- **Identidad criptográfica persistente:** la identidad de una unidad no depende de la moneda con la que se negocie.
- **Unicidad y procedencia:** los identificadores deben vincularse a emisiones autorizadas; ser únicos no demuestra por sí solo que un derecho sea legítimo.
- **Protocolos modulares:** minería, producción, proveedores, venta mayorista, distribución y liquidación pueden especificarse por módulos interoperables.
- **Trazabilidad:** registrar la cadena de transferencias y los cambios de estado relevantes.
- **Liquidación multidivisa:** permitir distintos medios de pago sin confundir pago, precio y activo transferido.
- **Privacidad por diseño:** reducir los datos sensibles almacenados públicamente y proteger secretos comerciales.
- **Sostenibilidad:** limitar recompensas y emisiones según reglas verificables y fuentes económicas definidas.
- **Interoperabilidad realista:** usar adaptadores e interfaces, sin suponer que una integración obliga a terceros a aceptar o listar activos.

## Modelo conceptual de participantes

| Participante | Función principal |
|---|---|
| Red y validadores | Mantienen el consenso y verifican las reglas compartidas. |
| Mineros | Aportan trabajo según el mecanismo de minería y las tareas autorizadas. |
| Productores/emisores | Crean o presentan unidades que están autorizados a emitir. |
| Holders/proveedores | Adquieren y administran inventario para abastecer los canales siguientes. |
| Vendedores mayoristas | Comercializan unidades en lotes o condiciones mayoristas. |
| Distribuidores minoristas | Ofrecen unidades a clientes finales. |
| Mercados y exchanges | Facilitan órdenes e intercambio cuando admiten el activo. |
| Proveedores de servicios | Reconocen, activan o atienden el derecho digital representado. |
| Clientes finales | Adquieren y utilizan las unidades según sus condiciones. |

Los roles pueden combinarse o separarse de acuerdo con las reglas de cada implementación. El acceso a un canal comercial puede requerir permisos de protocolo, contratos o ambos.

## Preguntas pendientes de especificación

Antes de implementar, se deben resolver al menos estos puntos:

- mecanismo de consenso, parámetros Scrypt y relación entre minería de bloques y trabajo de trazabilidad;
- definición de unidad criptográfica, identificador, producto representado y posibles extensiones;
- autorización y firma de productores;
- modelo de titularidad, transferencia y prevención de doble uso;
- esquema de recompensas, tarifas y sostenibilidad;
- reglas para productores, holders/proveedores, mayoristas y distribuidores;
- compatibilidad con varias monedas y redes de liquidación;
- integración con mercados externos y límites de lo que puede garantizar el protocolo;
- privacidad, gestión de claves, resolución de disputas y recuperación de errores;
- implicaciones contractuales, de propiedad intelectual y regulatorias según cada jurisdicción.

## Hoja de ruta propuesta

- [ ] Definir glosario, objetivos y alcance del protocolo.
- [ ] Especificar la arquitectura de red y el uso concreto de Scrypt.
- [ ] Diseñar el modelo de unidades, identificadores y extensiones de producción.
- [ ] Definir los protocolos de proveedores/holders, venta mayorista y distribución minorista.
- [ ] Diseñar el ciclo de vida de las unidades y las pruebas de eventos.
- [ ] Especificar el sistema de recompensas y las fuentes de financiación.
- [ ] Diseñar el modelo de liquidación multidivisa e interoperabilidad.
- [ ] Comparar la propuesta con tecnologías y protocolos existentes.
- [ ] Desarrollar un prototipo con unidades de prueba y servicios autorizados.
- [ ] Evaluar seguridad, rendimiento, costo por operación y viabilidad económica.
- [ ] Elaborar el whitepaper y someterlo a revisión técnica, económica y legal independiente.

## Alcance y estado

SMDN es una propuesta conceptual. Los nombres de los componentes, las reglas económicas, el consenso, la estructura de extensiones y la viabilidad técnica están pendientes de especificación. Este repositorio no representa una criptomoneda operativa, una implementación auditada, un servicio de liquidación disponible ni una promesa de rentabilidad.

## Licencia

Pendiente de elección. La licencia del código, si se publica, no concede por sí misma derechos sobre marcas, software, licencias o servicios de terceros.
