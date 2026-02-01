# Urbanalítica

## Laboratorio de Inteligencia Territorial

### Marco Teórico, Modelo de Negocio y Metodología Operativa

---

## Índice

1. Introducción
2. El problema de las decisiones territoriales
3. Urbanalítica como sistema
4. Marco teórico
   - 4.1 Economía urbana y localización
   - 4.2 Complejidad y sistemas adaptativos
   - 4.3 Space Syntax
   - 4.4 Amenity Space y co-localización
   - 4.5 Clustering espacial
5. Hipótesis operativas
6. Arquitectura del sistema
7. Algoritmos y modelos
8. Metodología
9. El UbX Score
   - Estructura jerárquica de métricas
10. Physical Asset Value (PAV)
    - Por qué UbX y PAV no pueden ser uno solo
    - PAV se mide con datos territoriales
    - Componentes y aplicación a portafolios
11. Casos de uso
12. Modelo de negocio
    - Propuesta de valor: cuatro pilares
    - ¿Must have o Nice to have?
    - Líneas de producto y facturación
    - Mitigación de riesgo SaaS
    - Medición de valor para clientes (ROI)
13. Costos, pricing y financiamiento
    - Estructura de costos
    - Pricing de productos
    - Proyecciones de revenue
    - Autofinanciamiento vs. inversión
    - Ronda Friends & Family (términos y retornos)
    - Use of funds y milestones
14. Clientes y equipo
15. Datos e IP
    - Propiedad intelectual
    - Protección contra replicación
    - Aprendizaje sin datos privados del cliente
    - Datasets premium a adquirir
16. Escalabilidad y límites
17. Posicionamiento competitivo
18. Ética y políticas públicas
19. Ventaja competitiva y roadmap
20. Conclusiones
21. Referencias

---

## 1. Introducción

Urbanalítica es un laboratorio de inteligencia territorial que reduce incertidumbre en decisiones de inversión y desarrollo urbano mediante análisis espacial avanzado, ciencia de datos y teoría de redes.

La propuesta es que el territorio no es una superficie pasiva, sino un sistema activo cuya estructura condiciona resultados económicos, sociales y ambientales. Esta estructura puede leerse, medirse y compararse sistemáticamente.

El laboratorio opera en la intersección de tres disciplinas:
- **Economía urbana clásica:** teorías de localización, externalidades de aglomeración.
- **Ciencia de redes:** topología, centralidad, flujos.
- **Ciencia de datos:** machine learning interpretable, clustering no supervisado, correlaciones espaciales.

**Dos índices centrales:**

El sistema produce dos métricas complementarias:

| Índice | Evalúa | Pregunta que responde |
|--------|--------|----------------------|
| **UbX Score** | Zonas y ubicaciones | ¿Qué tan buena es esta ubicación para un uso dado? |
| **PAV (Physical Asset Value)** | Activos físicos | ¿Cuál es la calidad estructural de este activo, independiente del precio? |

Juntos permiten evaluar tanto el "dónde" (territorio) como el "qué" (activo), y detectar divergencias entre precio de mercado y valor estructural.

---

## 2. El problema de las decisiones territoriales

Las decisiones territoriales —dónde invertir, qué desarrollar, cómo expandir una red— suelen tomarse con información fragmentada y metodologías inconsistentes.

**Fragmentación.** Los tomadores de decisiones reciben estudios de mercado aislados, análisis normativos desconectados y mapas descriptivos sin síntesis. Cada proveedor usa metodología propia. El resultado es un mosaico incomparable que el cliente debe sintetizar intuitivamente.

**Metodologías no replicables.** La mayoría de los estudios dependen de "criterio experto" que no puede auditarse. No hay un modelo subyacente que pueda probarse o mejorarse.

**Riesgo mal cuantificado.** Las decisiones territoriales implican apuestas de largo plazo, pero el riesgo se evalúa con proxies superficiales (precio histórico, "percepción") que no capturan la estructura del territorio.

**Sesgo hacia lo obvio.** Los métodos tradicionales favorecen ubicaciones ya exitosas, ignorando oportunidades emergentes y subestimando saturación en zonas consolidadas.

Urbanalítica parte de que estos problemas requieren un cambio de paradigma: entender el territorio como sistema complejo donde infraestructura, economía, población y riesgo interactúan en redes.

---

## 3. Urbanalítica como sistema

Urbanalítica no produce entregables cerrados. Produce modelos territoriales reutilizables, comparables y auditables. Cada proyecto alimenta una base de conocimiento acumulativa.

**Diferencia con estudios tradicionales.** Un estudio convencional responde una pregunta específica y se archiva. El conocimiento no se acumula. Urbanalítica invierte esta lógica: cada análisis contribuye a un modelo más amplio. Las métricas de un cliente pueden compararse con las de otro. El sistema aprende.

**El valor está en la estructura.** El entregable visible puede ser un mapa o ranking. El valor real está en la estructura analítica subyacente: algoritmos calibrados, correlaciones validadas, benchmarks acumulados. Esta estructura permite volver a interrogar el territorio cuando cambian las condiciones.

**Comparabilidad sistémica.** Todos los análisis usan las mismas métricas, fuentes procesadas consistentemente y algoritmos de normalización. Un terreno en Monterrey puede compararse estructuralmente con uno en Guadalajara.

**Auditabilidad.** Cada output puede rastrearse hasta sus fuentes, algoritmos y supuestos. Si un cliente pregunta "¿por qué este terreno tiene score 7.2?", hay una respuesta que descompone el índice en sus componentes.

---

## 4. Marco teórico

### 4.1 Economía urbana y localización

Urbanalítica se construye sobre una tradición de más de un siglo:

- **Von Thünen (1826):** Los usos del suelo se ordenan según costos de transporte. La localización responde a lógicas económicas modelables.
- **Hotelling (1929):** Los competidores tienden a aglomerarse en ubicaciones centrales para capturar mercado.
- **Christaller (1933) y Lösch (1940):** Las ciudades se organizan en jerarquías donde centros mayores ofrecen bienes especializados.
- **Krugman (1991):** Las economías de aglomeración generan patrones de concentración que se autorefuerzan.

Urbanalítica traduce estos principios en métricas operativas: centralidad como proxy de acceso a mercados, densidad como proxy de aglomeración, diversidad como proxy de resiliencia.

### 4.2 Complejidad y sistemas adaptativos

Las ciudades son sistemas complejos donde múltiples agentes toman decisiones interdependientes que generan patrones emergentes.

**Propiedades relevantes:**
- **No linealidad:** Pequeños cambios pueden tener efectos desproporcionados.
- **Emergencia:** Los barrios y clusters no se diseñan; emergen de decisiones individuales.
- **Retroalimentación:** El éxito atrae actividad que genera más éxito.
- **Distribuciones de cola pesada:** Pocos nodos concentran la mayor parte del valor.

### 4.3 Space Syntax

Teoría desarrollada por Bill Hillier que estudia cómo la configuración espacial condiciona movimiento y uso.

**Principios:**
- La configuración predice movimiento mejor que las características físicas.
- Espacios "integradores" (bien conectados) concentran actividad comercial.
- Espacios "segregados" tienden a usos residenciales o industriales.

**Métricas que usa Urbanalítica:**
- **Choice (betweenness):** Cuántos caminos mínimos pasan por un segmento.
- **Integration (closeness):** Qué tan cerca está un segmento del resto de la red.
- **NACH/NAIN:** Versiones normalizadas para comparar redes de distintos tamaños.

Urbanalítica extiende estas métricas a redes nacionales de carreteras, ferrocarriles y transporte público.

### 4.4 Amenity Space y co-localización

Marco de César Hidalgo que demuestra que los establecimientos siguen patrones de co-localización estadísticamente estables.

**Insight central:** Si dos tipos de negocio aparecen juntos más de lo esperado por azar, existe compatibilidad entre ellos (complementariedad de demanda, infraestructura compartida, externalidades).

**Aplicaciones:**
- **Diagnóstico:** ¿El entorno tiene la mezcla que predice éxito para el uso objetivo?
- **Detección de ausencias:** ¿Qué actividades "deberían" estar presentes pero no están?
- **Predicción de compatibilidad:** ¿Un nuevo uso es compatible con la estructura existente?

Urbanalítica generaliza el enfoque al DENUE completo (~5 millones de establecimientos).

### 4.5 Clustering espacial

Los barrios no se definen administrativamente; emergen de concentración de actividad.

**HDBSCAN** es el algoritmo principal. Ventajas:
- No requiere especificar número de clusters.
- Detecta formas arbitrarias.
- Maneja ruido y outliers.
- Es jerárquico (permite ver estructura a distintas escalas).

---

## 5. Hipótesis operativas

**1. La accesibilidad real explica más que la distancia euclidiana.**
Lo relevante es tiempo de traslado real considerando red vial, transporte público, tráfico y barreras físicas.

**2. La composición económica es más informativa que la densidad bruta.**
Saber que hay "muchos establecimientos" dice poco. Lo relevante es qué tipo son, cómo se relacionan y qué patrón de co-localización revelan.

**3. El riesgo territorial es una capa estructural, no un anexo.**
El riesgo se integra desde el inicio como variable que afecta todas las métricas. Un sitio con excelente accesibilidad pero alto riesgo hídrico no tiene la misma accesibilidad efectiva.

**4. La centralidad en red predice valor futuro mejor que el precio histórico.**
La estructura de la red predice mejor el valor potencial a largo plazo que el consenso actual de mercado.

---

## 6. Arquitectura del sistema

Urbanalítica se organiza en cinco capas analíticas que alimentan los índices de síntesis:

**Capa 1: Territorial base**
Topografía, hidrología, geología, cobertura vegetal. Define restricciones duras (no puedes construir en barranca) y blandas (puedes pero con costo adicional).

**Capa 2: Redes**
Vialidades, transporte público, ferrocarriles, puertos, redes eléctricas. Define accesibilidad efectiva de cada punto.

**Capa 3: Socioeconómica**
Población, empleo, establecimientos, ingreso. Define demanda y oferta de servicios.

**Capa 4: Riesgo y resiliencia**
Integración de riesgos físicos (hídrico, sísmico, climático), operativos (infraestructura, servicios), regulatorios (normativa, restricciones) y sociales (seguridad, fricción). El riesgo no es capa accesoria: afecta el cálculo de todas las demás métricas.

**Capa 5: Síntesis estratégica**
Integración en dos índices complementarios:
- **UbX Score:** Calidad de ubicación para un uso dado
- **PAV:** Calidad estructural del activo físico

**Mother: el sistema comparativo**

Marco que permite comparar activos heterogéneos:
- Normalización universal en las mismas variables
- Benchmarking por cohorte funcional
- Simulación de uso: "¿qué score tendría este activo si cambio el uso?"
- Detección de brechas precio-valor

---

## 7. Algoritmos y modelos

### Redes y métricas topológicas

**Betweenness Centrality:** $C_B(v) = \sum_{s \neq v \neq t} \frac{\sigma_{st}(v)}{\sigma_{st}}$

Nodos con alta betweenness son "puentes" críticos para conectividad.

**Closeness Centrality:** $C_C(v) = \frac{n-1}{\sum_{u \neq v} d(v,u)}$

Nodos con alta closeness alcanzan cualquier parte de la red rápidamente.

### Accesibilidad e isócronas

Áreas alcanzables desde un punto en tiempo determinado, calculadas con Dijkstra/A* sobre redes multimodales.

**Accesibilidad a oportunidades:** $A_i = \sum_j O_j \cdot f(t_{ij})$

Donde $O_j$ son oportunidades en destino $j$, $t_{ij}$ es tiempo de viaje, y $f$ es función de decaimiento.

### Métricas de diversidad

**Shannon (Entropía):** $H = -\sum_{i=1}^{n} p_i \ln(p_i)$

Alta entropía = muchas categorías equilibradas. Baja = dominancia de pocas.

**Herfindahl-Hirschman:** $HHI = \sum_{i=1}^{n} p_i^2$

Alto HHI = especialización. Bajo = diversificación.

**Cociente de Localización:** $LQ_i = \frac{e_i / e}{E_i / E}$

LQ > 1 indica especialización local; LQ < 1 indica subrepresentación.

### Correlaciones y Amenity Space

Matrices de co-localización usando correlación de Spearman sobre presencia en celdas espaciales (hexágonos H3). Red de compatibilidades proyectada en 2D con UMAP.

### Arquitectura de datos

**Fuentes actuales:**
- INEGI (DENUE, censos, cartografía)
- OSM (red vial, edificaciones, POIs)
- Google Places (POIs con popularidad)
- AMAI (niveles socioeconómicos)
- Atlas de Riesgo, CONAGUA, CENAPRED
- Datos propios de clientes

**Enriquecimiento:**
- Web scraping (portales inmobiliarios, noticias)
- Series de tiempo del DENUE
- Normalización a malla hexagonal H3

**Datos a adquirir:**
- Movilidad agregada de celulares
- Transacciones inmobiliarias reales
- Foot traffic

---

## 8. Metodología

### Lectura multiescalar

Cada sitio se lee desde múltiples escalas:
- **Nacional/regional:** Posición en corredores logísticos, conectividad a puertos.
- **Metropolitana:** Estructura policéntrica, accesibilidad a empleo.
- **Corredor/zona:** Carácter funcional, tendencias de transformación.
- **Sitio/manzana:** Entorno inmediato, accesos, microclima.

### Integración de datos heterogéneos

Retos: temporalidad distinta (censo cada 10 años vs. DENUE mensual), granularidad distinta (AGEB vs. manzana), calidad variable, formatos incompatibles.

Solución: pipelines de ETL espacial que normalizan todas las fuentes a malla común.

### Normalización y comparabilidad

- **Z-score:** Posición relativa centrada en media.
- **Min-max:** Escalado a [0,1] para agregar indicadores.
- **Percentil:** Robusto a outliers.

Cada sitio se compara contra promedio de su ciudad, su tipología funcional, mejores prácticas y competidores directos.

### Síntesis territorial

No es promedio ponderado. Es interpretación estructural que considera:
- **Coherencia interna:** ¿Los indicadores cuentan historia consistente?
- **Trayectoria:** ¿Crecimiento, consolidación o declive?
- **Sensibilidad:** ¿Qué tan robusto es el diagnóstico a variaciones?
- **Acción:** ¿Qué implica para la decisión concreta?

---

## 9. El UbX Score

Índice que sintetiza la calidad de una **ubicación** para un uso dado.

**Componentes:**

| Dimensión | Qué mide |
|-----------|----------|
| **Accesibilidad** | Facilidad de llegada multimodal, acceso a servicios |
| **Conectividad** | Centralidad topológica, conexión a redes logísticas |
| **Compatibilidad** | Alineación con Amenity Space, diversidad, complementadores |
| **Mercado laboral** | Masa salarial accesible, talento disponible |
| **Riesgo-Resiliencia** | Exposición a riesgos, capacidad de recuperación |
| **Forward Value** | Tendencia de indicadores, proyectos programados |

**Cálculo:** $UbX = f(Acc, Con, Comp, Lab, Risk, FV)$

La función incluye interacciones, umbrales y ponderaciones configurables por cliente según uso objetivo.

**Escala:**
- 8-10: Premium
- 6-8: Competitiva
- 4-6: Limitaciones
- 2-4: Desafíos significativos
- 0-2: No recomendada

### Estructura jerárquica de métricas

El UbX es un índice sintético de alto nivel diseñado para responder preguntas de negocio. Debajo se alimenta de métricas científicas subyacentes:

**Capa de decisión (índices sintéticos):**
- UbX traduce complejidad técnica en puntajes simples del 0 al 10
- Responde preguntas directas: "¿Qué tan buena es esta ubicación?"

**Capa de ingeniería (métricas científicas):**
- Space Syntax: Betweenness (flujo pasante), Integration (cercanía)
- Diversidad: Entropía de Shannon, HHI
- Co-localización: Matrices de Amenity Space

Esta estructura permite que el usuario vea un score interpretable mientras la auditoría técnica permanece disponible para quien la requiera.

---

## 10. Physical Asset Value (PAV)

Mientras el UbX evalúa ubicaciones, el PAV evalúa **activos físicos** independientemente de su precio de mercado.

### Por qué UbX y PAV no pueden ser uno solo

Aunque ambos usan datos territoriales, evalúan dimensiones distintas que pueden contradecirse:

| Índice | Evalúa | Pregunta |
|--------|--------|----------|
| **UbX** | El entorno ("dónde está") | ¿Qué tan bueno es este punto geográfico? |
| **PAV** | El objeto ("qué es") | ¿Qué tan robusto es este activo específico? |

**Ejemplo extremo:** Una mansión en un desierto sin carreteras (PAV alto, UbX bajo) o una choza en Manhattan (UbX alto, PAV bajo). Un índice único promediaría estos factores, ocultando la realidad.

**La separación permite identificar estrategias:**

| Combinación | Diagnóstico | Estrategia |
|-------------|-------------|------------|
| UbX Alto + PAV Bajo | Oportunidad de desarrollo | Comprar para demoler/remodelar |
| UbX Bajo + PAV Alto | "Elefante Blanco" | Evitar—edificio magnífico en zona desconectada |
| UbX Alto + PAV Alto | Activo premium | Precio justificado si no hay sobreprecio |
| UbX Bajo + PAV Bajo | Evitar | Sin valor estructural ni potencial |

**Función financiera:** El PAV existe para compararse contra el Precio de Mercado. Si estuviera mezclado con UbX, no podríamos aislar el valor estructural para detectar divergencias.

### PAV se mide con datos territoriales, no con visita al sitio

Aunque su nombre dice "Activo Físico", el PAV **no depende de inspección visual** (ver si hay grietas o si la pintura es nueva). Se mide con datos territoriales de alta precisión enfocados en vulnerabilidad y resiliencia.

**¿Qué evalúa el PAV que una visita no puede ver?**

| Tipo de riesgo | Método tradicional | Método PAV |
|----------------|-------------------|------------|
| Riesgo hídrico | "No se ve inundado" | Modelos hidrológicos + historial de eventos |
| Riesgo sísmico | "Parece firme" | Microzonificación + suelo + fallas cercanas |
| Redundancia de red | "Tiene buena calle" | Análisis de grafos: ¿si se bloquea la principal, queda aislado? |
| Riesgo regulatorio | "Está en zona urbana" | Normativa de uso de suelo + restricciones específicas |

**Escalabilidad:** La prueba de que no es visita manual es que puede evaluar 50 terrenos de un portafolio simultáneamente, generando rankings y mapas de concentración de riesgo.

### Por qué no basta el avalúo tradicional

El avalúo convencional (comparables, catastro, ajustes heurísticos) tiene tres limitaciones:
- **Retrospectivo:** Explica el pasado, no anticipa desempeño
- **Local:** Difícil comparar entre territorios heterogéneos
- **Aislado:** No considera el sistema territorial

**Diferencia clave:**
- Avalúo tradicional / Visita al sitio: Retrospectivo, manual. Mira estado de conservación actual.
- PAV (Urbanalítica): Prospectivo, sistémico. Mira si el activo sobrevivirá shocks futuros.

### Componentes del PAV

| Componente | Qué mide |
|------------|----------|
| Accesibilidad | Conectividad real y redundancia de red |
| Riesgo físico | Exposición hídrica, climática, geotécnica, regulatoria |
| Compatibilidad | Alineación económica del entorno |
| Adaptabilidad | Capacidad de cambio de uso |
| Robustez | Estabilidad operativa y normativa |

### Precio vs. valor estructural

| Divergencia | Interpretación |
|-------------|----------------|
| **Precio >> PAV** | Sobrevaloración, riesgo de corrección |
| **Precio << PAV** | Oportunidad latente, forward value |

Esta brecha es la señal más valiosa para inversión estratégica.

### Aplicación a portafolios

El PAV escala del activo individual al portafolio:
- Ranking de activos por calidad física
- Mapa de concentración de riesgo
- Identificación de activos ancla vs. frágiles
- Simulación de escenarios de estrés

Habilita: rotación de activos, priorización de mitigación, reequilibrio territorial.

### Variables que preceden movimientos de precio

Urbanalítica no predice precios directamente. Investiga qué variables estructurales preceden apreciación:
- Cambios en centralidad de red
- Incremento de diversidad económica
- Reducción de riesgo físico
- Mejora en accesibilidad

**Ciclo de validación:**
1. El sistema dice hoy: "Este terreno tiene PAV alto pero precio bajo—debería subir"
2. En 12-24 meses, verifica: ¿Subió de valor?
3. Si SÍ: confirma que las variables eran predictivas. Si NO: recalibra pesos.

Modelos longitudinales permiten validar qué combinaciones son predictivas.

---

## 11. Casos de uso

**Selección de sitios logísticos**

Operador busca centro de distribución. Urbanalítica genera ranking con UbX (conectividad, accesibilidad, mercado laboral) filtrado por riesgo operativo.

**Expansión de redes comerciales**

Cadena quiere abrir 20 tiendas. Urbanalítica modela catchments, simula canibalización, detecta gaps y rankea candidatos por UbX ajustado al formato.

**Evaluación de portafolios**

Fondo tiene 50 terrenos. Urbanalítica evalúa cada uno con PAV, detecta brechas precio-valor, identifica activos ancla vs. frágiles y genera recomendaciones de rotación.

**Due diligence territorial**

Inversionista evalúa adquisición. Urbanalítica combina UbX (potencial de la ubicación) con PAV (calidad del activo) para determinar si el precio se justifica estructuralmente.

**Planeación urbana**

Gobierno quiere orientar crecimiento. Urbanalítica mapea UbX por zona, identifica infraestructura subutilizada y simula impacto de proyectos públicos.

---

## 12. Modelo de negocio

### Propuesta de valor: cuatro pilares

**1. Detección de la brecha Precio vs. Valor Estructural**
El núcleo de la oferta. Mientras avalúos tradicionales son retrospectivos (comparables históricos), Urbanalítica es prospectivo: cruza UbX y PAV para responder si el precio de mercado está justificado estructuralmente.

**2. Sistematización vs. Intuición (Auditabilidad)**
Métricas estandarizadas y replicables. Un terreno en Monterrey puede compararse con uno en Guadalajara bajo los mismos parámetros. Cada score se desglosa hasta sus fuentes.

**3. Modelo Acumulativo de Conocimiento**
El conocimiento no se archiva, se acumula. Cada proyecto alimenta benchmarks y mejora modelos para los siguientes clientes.

**4. Posicionamiento Híbrido**
Ni consultoría artesanal ni SaaS genérico. Profundidad local + interpretación experta + infraestructura de datos.

### ¿Must have o Nice to have?

**Must Have (esencial) para:**
- Inversionistas institucionales (FIBRAS, fondos) que necesitan detectar riesgo financiero invisible
- Comités de inversión que requieren auditabilidad (no "criterio de experto")
- Actores que buscan ventaja estructural competitiva

**Nice to Have (opcional) para:**
- Compradores individuales de vivienda (costo desproporcionado)
- Decisiones pequeñas o validaciones superficiales
- Clientes que "ya tomaron la decisión" y solo buscan justificación

**No es para:**
- Quien busca validar decisiones ya tomadas ("rubber stamping")
- Sustitución de estudios legales o ingeniería de detalle

### Líneas de producto

**Proyectos de diagnóstico (High-Ticket One-Time)**
Análisis profundo para decisiones críticas. Precio por proyecto (6-7 cifras). Alta personalización. Desde due diligence hasta masterplanning completo.

**Licencias del sistema (SaaS - ARR)**
Acceso a plataforma para exploración: mapas, comparadores, alertas. Suscripción anual (5-6 cifras). Genera stickiness y flujo predecible.

**Acompañamiento estratégico (Retainers)**
El eslabón que conecta la plataforma con la toma de decisiones ejecutiva.

| Función | Descripción |
|---------|-------------|
| Interpretación | Traduce métricas técnicas (Space Syntax, Entropía) a lenguaje de negocio |
| Actualización | Sesiones mensuales para revisar cambios y recalibrar |
| Integración | Funciona como "brazo externo" de inteligencia territorial |

**Niveles de acompañamiento:**
- **Advisory:** 8-12 hrs/mes. Soporte ligero e interpretación.
- **Strategic:** 20-30 hrs/mes. Validación constante para equipos activos.
- **Embedded:** Dedicación parcial. Prácticamente un departamento interno externalizado.

**Impacto financiero del acompañamiento:**
- Genera ARR estable que suaviza flujos vs. proyectos episódicos
- Crea barrera de salida: una vez integrado en comités de inversión, difícil cambiar
- Retroalimenta desarrollo de producto al entender qué métricas son útiles

**APIs y datos**
Acceso a datasets y métricas para integración en sistemas del cliente.

### Modelo de facturación detallado

**Por línea de producto:**

| Línea | Modelo de cobro | Lógica |
|-------|-----------------|--------|
| Diagnósticos | Por proyecto (one-time) | Ticket alto, entregable cerrado |
| Licencias SaaS | Suscripción anual | Cuotas por tier (Explorer/Professional/Enterprise) |
| Acompañamiento | Retainer mensual | Horas reservadas, facturación recurrente |
| APIs y datos | Por volumen o uso | Requests a la API o datasets específicos |

**Cobro de APIs (tres modalidades):**

1. **Por consumo:** El cliente paga según cantidad de llamadas (requests) o tamaño de datasets descargados.
2. **Como parte del SaaS Enterprise:** API completa incluida en licencia alta ($1.35M-$2.7M/año)—funciona como "barra libre".
3. **Pass-through en proyectos:** Datos específicos adquiridos ad-hoc se suman a la factura del proyecto ($18K-$90K MXN).

### Mitigación de riesgo SaaS: "la gente no sabe usarlo"

Urbanalítica **no es SaaS puro de autoservicio**. Es modelo híbrido diseñado para evitar que el cliente se pierda en los datos.

**Mecanismos de mitigación:**

| Riesgo | Solución |
|--------|----------|
| Métricas técnicas complejas | Índices sintéticos (UbX/PAV) simplifican a puntaje 0-10 |
| Falta de interpretación | Acompañamiento estratégico traduce a lenguaje de negocio |
| Usuario no experto | Segmentación a clientes sofisticados (FIBRAS, fondos) con equipos internos |
| Abandono por complejidad | Tiers escalonados: Explorer (simple) → Enterprise (completo + soporte) |

**Argumento para clientes:** "No te vendemos las llaves del coche para que manejes solo. Te vendemos el coche (SaaS) junto con un copiloto experto (Acompañamiento) que te ayuda a interpretar el camino."

### Economía del modelo

- **Costo marginal bajo** una vez construida la infraestructura
- **Valor acumulativo:** cada proyecto enriquece la base de benchmarks
- **Escalabilidad** por ciudad y vertical
- **Stickiness:** difícil migrar una vez integrado (APIs conectadas, flujos dependientes)
- **Efecto de red:** más clientes → más validación → mejores modelos → más clientes

### Cómo medir el valor para clientes (ROI)

El ahorro se mide desde tres dimensiones:

**1. Ahorro en due diligence (tiempo y consultoría)**

| Concepto | Tradicional | Urbanalítica |
|----------|-------------|--------------|
| Tiempo de ejecución | Semanas/meses | Días/horas |
| Coordinación de proveedores | Múltiples (mercado, legal, técnico) | Síntesis integrada |
| Costo-hombre de equipo directivo | Alto (reuniones, integración manual) | Bajo (reporte listo para comité) |

**Cálculo:** Si el costo de oportunidad de capital es 10% anual, tener detenida una decisión de $100M durante 3 meses cuesta ~$2.5M en capital inactivo. Reducir a 1 semana recupera casi todo ese costo.

**2. Ahorro por prevención de sobreprecio**

El sistema detecta cuando Precio >> PAV (sobrevaloración).

| Métrica | Cálculo |
|---------|---------|
| Sobreprecio evitado | (Precio de lista - PAV ajustado) × probabilidad de corrección |
| Ejemplo | Si el sistema detecta sobreprecio de 15% en activo de $50M = $7.5M de riesgo evitado |

**3. Ahorro por mitigación de riesgos ocultos**

| Tipo de riesgo | Costo potencial evitado |
|----------------|------------------------|
| Activo varado (inundable, sin acceso) | 100% de la inversión |
| Canibalización (nueva tienda roba ventas a otra) | Ventas perdidas de la red existente |
| Riesgo regulatorio (cambio de uso imposible) | Costo de reconversión o pérdida total |

**Fórmula de valor total:**

```
Ahorro = (Costo_Consultoria_Tradicional - Costo_Urbanalitica)
       + Sobreprecio_Evitado
       + Riesgo_Mitigado
```

**Argumento de venta:** "Nuestro servicio cuesta una fracción de lo que te ahorra en una sola mala decisión inmobiliaria. Un due diligence de $2.7M MXN puede evitar un sobreprecio de $15M o un activo varado de $50M."

### Comparativa de ahorro vs. consultoría tradicional

| Dimensión | Consultoría tradicional | Urbanalítica |
|-----------|------------------------|--------------|
| Velocidad | Semanas/meses | Días/horas |
| Costo marginal por análisis | Alto (horas-hombre) | Bajo (infraestructura ya construida) |
| Auditabilidad | "Confía en el experto" | Desglosable a fuentes y algoritmos |
| Acumulación | Se archiva, se pierde | Mejora benchmarks para futuros análisis |
| Detección de riesgos ocultos | Proxies superficiales | Capa estructural de riesgo |
| Comparabilidad | Cada estudio es único | Mismo marco para todas las ciudades |

---

## 13. Costos, pricing y financiamiento

### Estructura de costos operativos

**Costos fijos mensuales (operación base):**

| Concepto | MXN/mes | USD/mes |
|----------|---------|---------|
| Equipo core (2-3 personas) | $180,000 - $280,000 | $10,000 - $15,500 |
| Infraestructura cloud (AWS/GCP) | $18,000 - $36,000 | $1,000 - $2,000 |
| APIs y datos (Google, etc.) | $9,000 - $27,000 | $500 - $1,500 |
| **Dataset premium (movilidad, transacciones)** | **$41,667** | **$2,315** |
| Software y licencias | $5,400 - $9,000 | $300 - $500 |
| Oficina/coworking | $9,000 - $18,000 | $500 - $1,000 |
| Legal, contable, admin | $9,000 - $18,000 | $500 - $1,000 |
| **Total mensual (sin dataset premium)** | **$230,000 - $390,000** | **$12,800 - $21,500** |
| **Total mensual (con dataset premium)** | **$272,000 - $432,000** | **$15,100 - $24,000** |
| **Total anual (sin dataset premium)** | **$2.8M - $4.7M** | **$154K - $258K** |
| **Total anual (con dataset premium)** | **$3.3M - $5.2M** | **$181K - $288K** |

**Costos variables por proyecto:**

| Concepto | Por proyecto |
|----------|--------------|
| Adquisición de datos específicos | $18,000 - $90,000 MXN |
| Horas adicionales de análisis | $1,800 - $3,600 MXN/hora |
| Visualización y entregables custom | $27,000 - $72,000 MXN |

### Pricing de productos

**Proyectos de diagnóstico (one-time)**

| Tipo | Alcance | Precio MXN | Precio USD |
|------|---------|------------|------------|
| Diagnóstico básico | 1 sitio, 1 ciudad, reporte estándar | $180,000 - $350,000 | $10K - $19K |
| Diagnóstico profundo | 1-5 sitios, análisis comparativo | $450,000 - $900,000 | $25K - $50K |
| Due diligence territorial | Portafolio completo, múltiples ciudades | $900,000 - $2,700,000 | $50K - $150K |
| Masterplan estratégico | Ciudad/zona completa, escenarios | $1,800,000 - $5,400,000 | $100K - $300K |

**Licencias anuales (recurring)**

| Tier | Incluye | Precio anual MXN | Precio anual USD |
|------|---------|------------------|------------------|
| Explorer | Acceso a mapas, 1 ciudad, consultas limitadas | $270,000 - $450,000 | $15K - $25K |
| Professional | Multi-ciudad, comparadores, alertas, API básica | $540,000 - $900,000 | $30K - $50K |
| Enterprise | Ilimitado, API completa, soporte dedicado | $1,350,000 - $2,700,000 | $75K - $150K |

**Retainers de acompañamiento (recurring)**

| Nivel | Horas/mes | Precio mensual MXN | Precio mensual USD |
|-------|-----------|--------------------|--------------------|
| Advisory | 8-12 hrs | $72,000 - $108,000 | $4K - $6K |
| Strategic | 20-30 hrs | $144,000 - $216,000 | $8K - $12K |
| Embedded | Dedicación parcial | $270,000 - $450,000 | $15K - $25K |

### Proyección de revenue (escenarios año 1-2)

**Escenario supervivencia (mínimo viable):**
- 2 proyectos diagnóstico/año @ $300K promedio = $600K
- 1 licencia Explorer @ $270K = $270K
- Consultoría suelta (sin retainer fijo) = $180K
- **Total año 1: $1.05M MXN (~$58K USD)**
- *Nota: Este escenario requiere mantener costos en mínimo y/o ingresos paralelos del equipo*

**Escenario conservador:**
- 3 proyectos diagnóstico/año @ $500K promedio = $1.5M
- 2 licencias Explorer @ $350K = $700K
- 1 retainer Advisory @ $90K × 12 = $1.08M
- **Total año 1: $3.3M MXN (~$183K USD)**

**Escenario base:**
- 5 proyectos diagnóstico/año @ $650K promedio = $3.25M
- 4 licencias (2 Explorer + 2 Professional) = $1.6M
- 2 retainers @ $120K × 12 = $2.88M
- **Total año 1: $7.7M MXN (~$428K USD)**

**Escenario optimista:**
- 8 proyectos diagnóstico/año @ $800K promedio = $6.4M
- 6 licencias diversificadas = $3.6M
- 3 retainers + 1 enterprise = $5.4M
- **Total año 1: $15.4M MXN (~$856K USD)**

**Escenario hiper-optimista (whale + momentum):**
- 1 contrato enterprise ancla (FIBRA o corporativo grande) = $5M
- 12 proyectos diagnóstico @ $900K promedio = $10.8M
- 10 licencias (3 Enterprise + 5 Professional + 2 Explorer) = $8.1M
- 5 retainers diversificados = $7.2M
- **Total año 1: $31.1M MXN (~$1.7M USD)**
- *Nota: Requiere un "whale" que valide y abra puertas + ejecución impecable + algo de suerte*

### Autofinanciamiento vs. inversión

**¿Cuántos clientes para break-even sin inversión?**

Para cubrir costos operativos base:
- **Sin dataset premium:** $2.8M - $4.7M MXN/año
- **Con dataset premium ($500K/año):** $3.3M - $5.2M MXN/año

| Ventas requeridas (escenario conservador) | Cantidad |
|-------------------------------------------|----------|
| Proyectos diagnóstico | 3 @ $500K promedio = $1.5M |
| Licencias SaaS | 2 Explorer @ $350K = $700K |
| Retainer Advisory | 1 @ $90K × 12 = $1.08M |
| **Total** | **$3.3M MXN** |

Esto cubre apenas los costos fijos mínimos **sin dataset premium**. Con el dataset premium, el break-even sube a ~$3.8M MXN/año.

**El riesgo del escenario de supervivencia:**

Si las ventas son lentas (solo 2 proyectos + 1 licencia = $1.05M), los ingresos están muy por debajo de los costos operativos mínimos. Sin inversión, este escenario requiere que el equipo trabaje sin sueldo completo o con ingresos paralelos.

**El dataset premium como decisión estratégica:**

El dataset de $500K/año es un costo significativo (~15% del break-even), pero:
- Diferencia el producto vs. competidores que usan solo datos públicos
- Habilita métricas imposibles de replicar con fuentes gratuitas
- Las actualizaciones trimestrales mantienen relevancia

**Conclusión:** Aunque técnicamente es posible autofinanciarse con ~6-7 ventas/año, el riesgo de quedarse sin liquidez es alto. Se recomienda levantar capital para operar con tranquilidad y poder pagar el dataset premium desde el inicio.

### Ronda Friends & Family

**¿Cuánto levantar?**

| Objetivo | Monto MXN | Monto USD | Runway |
|----------|-----------|-----------|--------|
| Mínimo viable | $1,800,000 | $100K | 6-8 meses |
| Recomendado | $3,600,000 | $200K | 12-15 meses |
| Cómodo | $5,400,000 | $300K | 18-24 meses |

**Recomendación: $3.6M - $5.4M MXN ($200K - $300K USD)**

Razón: Suficiente runway para cerrar 3-5 clientes ancla y demostrar tracción antes de necesitar siguiente ronda.

**Términos sugeridos F&F:**
- SAFE o nota convertible
- Cap de valuación: $18M - $27M MXN ($1M - $1.5M USD)
- Descuento: 20% sobre siguiente ronda priced
- Sin intereses o interés mínimo (5-8% anual)

### ¿Cuándo y cómo ganan dinero los inversionistas F&F?

**Importante:** Esta inversión **no es un préstamo** con pagos mensuales. Es una apuesta de capital (equity) a largo plazo.

**¿Cuándo reciben su dinero?**
- No en el corto plazo. El dinero se convierte en participación de la empresa.
- **Evento de conversión:** En 12-18 meses, al levantar la ronda Seed, el SAFE/Nota se convierte en acciones.
- **Salida real (cash out):** Generalmente en un evento de liquidez futuro: adquisición (Exit), salida a bolsa (IPO), o venta de acciones en rondas futuras.

**Mecanismos de ganancia:**

**A. El Descuento (ganancia inmediata en papel)**
Los F&F entran con 20% de descuento sobre el precio de la siguiente ronda.
- Ejemplo: Si un VC paga $10/acción en la Seed, los F&F compran a $8/acción.
- Ganancia instantánea: 20% de valor en el momento de conversión.

**B. El Tope de Valuación (Cap) — la ganancia mayor**
Cap sugerido: $18M - $27M MXN.
- Si a Urbanalítica le va muy bien y en la siguiente ronda vale $50M, los nuevos inversionistas pagan precio de $50M.
- Pero los F&F convierten como si valiera solo $18M-$27M.
- Resultado: reciben muchas más acciones por su dinero que los nuevos inversionistas.

**C. Interés acumulado (solo en Nota Convertible)**
- Si se usa Nota Convertible con interés del 5-8% anual, ese interés **no se paga en efectivo**.
- Se acumula y se suma al principal para comprar más acciones en la conversión.

**¿Se reparten utilidades (dividendos)?**

**No.** En modelo de startup de alto crecimiento, las ganancias no se sacan—se reinvierten como combustible.

| Destino del capital | Uso |
|---------------------|-----|
| 50-55% | Equipo (salarios) |
| 12-15% | Infraestructura y datos |
| 15-18% | Desarrollo de producto |
| Resto | Ventas, marketing, buffer |

La ganancia de los inversionistas viene de **plusvalía** (aumento de valor de sus acciones), no de rentas.

**¿Qué pasa si no hay ronda Seed?**

| Escenario | Consecuencia para F&F |
|-----------|----------------------|
| Ventas < $2.8M/año | Crisis de liquidez. Alto riesgo de pérdida total. |
| Ventas = $3.3M/año | Empresa sobrevive. Inversión "flota" sin convertirse ni liquidarse. |
| Ventas > $5M/año | Tracción demostrada. Conversión y ganancia potencial activas. |

**Resumen para inversionistas:** "Tu ganancia es que compras una parte de la empresa hoy a precio muy bajo (con cap de $18M-$27M y 20% de descuento). No recibirás pagos mensuales, pero si la empresa crece y vale $100M+, tu participación valdrá muchas veces lo que invertiste."

### Use of funds (distribución del capital)

**Para ronda de $3.6M MXN ($200K USD):**

| Categoría | % | Monto MXN | Uso específico |
|-----------|---|-----------|----------------|
| **Equipo** | 55% | $1,980,000 | Salarios core team 12 meses |
| **Infraestructura** | 15% | $540,000 | Cloud, APIs, datos, herramientas |
| **Desarrollo de producto** | 15% | $540,000 | Mejoras plataforma, nuevas features |
| **Ventas y marketing** | 10% | $360,000 | Eventos, materiales, viajes a clientes |
| **Buffer/contingencia** | 5% | $180,000 | Imprevistos, oportunidades |

**Para ronda de $5.4M MXN ($300K USD):**

| Categoría | % | Monto MXN | Uso específico |
|-----------|---|-----------|----------------|
| **Equipo** | 46% | $2,500,000 | Salarios + 1 hire adicional |
| **Infraestructura** | 10% | $540,000 | Cloud escalado |
| **Desarrollo de producto** | 17% | $900,000 | Plataforma robusta, simulador |
| **Ventas y marketing** | 11% | $600,000 | BD dedicado, eventos, contenido |
| **Datos premium** | 9% | $500,000 | Dataset principal (movilidad, transacciones, foot traffic) — 1 año con actualizaciones trimestrales |
| **Buffer** | 7% | $360,000 | Contingencia + renovación datos año 2 |

### Milestones para siguiente ronda

Para levantar una ronda Seed ($500K - $1M USD) en 12-18 meses:

| Milestone | Meta |
|-----------|------|
| ARR (Annual Recurring Revenue) | $5M+ MXN ($280K+ USD) |
| Clientes pagando | 8-12 clientes |
| Retención | >80% renovación |
| Logo quality | 2-3 clientes reconocibles |
| Producto | Plataforma funcional con self-service parcial |
| Equipo | 4-6 personas core |

### Unit economics objetivo

| Métrica | Target |
|---------|--------|
| CAC (Costo de adquisición) | <$15K USD por cliente |
| LTV (Lifetime value) | >$75K USD |
| LTV/CAC | >5x |
| Gross margin | >70% |
| Payback period | <6 meses |
| Net Revenue Retention | >110% (expansión > churn) |

---

## 14. Clientes y equipo

### Clientes ideales

**Fondos de inversión inmobiliaria**
FIBRAS, capital privado, family offices. Necesitan due diligence sistematizada y monitoreo de portafolio.

**Desarrolladores de gran escala**
Proyectos de uso mixto, ciudades planeadas, parques industriales. Necesitan reducir incertidumbre en inversiones de largo plazo.

**Corporativos con redes territoriales**
Retail, bancos, telecomunicaciones, salud. Necesitan optimización de red y priorización de expansión.

**Gobiernos con visión estratégica**
Municipios/estados con capacidad técnica. Necesitan ordenamiento territorial basado en datos.

**No son clientes ideales:** Compradores individuales de vivienda, desarrolladores pequeños, gobiernos sin capacidad de uso, clientes que buscan validar decisiones ya tomadas.

### Equipo operativo

Núcleo experto que combina:
- Programación (Python, GeoPandas, PostGIS)
- Teoría urbana y economía de localización
- Visualización geoespacial
- Traducción técnica a lenguaje de negocio

### Estrategia

Diseñada por perfiles híbridos: arquitectura/urbanismo + economía + datos + negocio. Este perfil es raro y concentrarlo es parte de la ventaja competitiva.

### Inversionistas

Entienden que el territorio es infraestructura de valor a largo plazo. Tesis: quien sistematice la inteligencia territorial tiene ventaja estructural. Perfil: paciente, sofisticado, con acceso a deal flow.

---

## 15. Datos e IP

### Propiedad intelectual

**Es IP de Urbanalítica:**
- Algoritmos y pipelines
- Bases de datos curadas
- Modelos entrenados
- Metodología de scoring

**Se licencia al cliente:**
- Visualización de resultados
- Outputs específicos
- En algunos casos, datos procesados para uso interno

**No se cede:**
- Código fuente
- Bases de datos completas
- Modelos descargables
- Derecho a sublicenciar

### ¿Cómo garantizar que el cliente no replique la base de datos?

El activo principal se protege mediante estrategia legal y técnica:

**1. Modelo de licencia, no de venta**
- El cliente recibe licencia limitada para usar outputs específicos
- No se vende la base de datos completa
- Prohibición explícita de sublicenciar

**2. La "caja negra" técnica**
Incluso si el cliente copiara los datos accesibles, no podría replicar el negocio:
- El valor está en los pipelines de ETL que normalizan fuentes heterogéneas
- Los algoritmos de Space Syntax, Amenity Space, etc. no se entregan
- El cliente ve el score final (ej. UbX = 8.5), pero no la fórmula ponderada

**3. Protección legal y auditoría**
- Cláusulas de confidencialidad estrictas
- Restricciones de uso y compartición
- Derecho de auditoría de cumplimiento

**4. Barrera de acumulación**
El sistema se enriquece continuamente. Una copia estática de la base de datos se vuelve obsoleta rápidamente vs. el servicio vivo.

**Analogía:** "El cliente compra la leche (el insight/reporte), pero Urbanalítica nunca entrega la vaca (la base de datos completa) ni la fórmula del alimento (los algoritmos)."

### ¿Cómo enriquecer datos sin usar datos privados del cliente?

Pregunta común de clientes: "¿Voy a entrenar tu algoritmo para que luego ayudes a mi competencia?"

**Respuesta:** El aprendizaje del algoritmo **no depende de datos privados del cliente**, sino de observación masiva del entorno público.

**Fuentes de aprendizaje:**

| Fuente | Qué aporta |
|--------|------------|
| DENUE (~5M establecimientos) | Patrones de co-localización públicos |
| OpenStreetMap | Red vial, edificaciones, POIs |
| Datos de movilidad (comprados) | Flujos reales sin depender del cliente |
| Web scraping | Tendencias de precios inmobiliarios |
| Space Syntax | Métricas topológicas de la red vial pública |

**El algoritmo aprende de:**
- Análisis de 5 millones de puntos económicos públicos
- Patrones de éxito/fracaso observados en el tiempo
- Correlaciones entre estructura territorial y desempeño

**Los datos del cliente se usan exclusivamente para:**
- Calibrar el análisis de SU proyecto (ajustar pesos del UbX a sus necesidades)
- NO se almacenan en la "memoria compartida" del modelo
- NO se usan para entrenar predicciones para otros

**Argumento para clientes:** "Nuestra ventaja es que medimos el Territorio (público y sistémico), no tu Operación (privada). No necesitamos tus tickets de venta para saber que esa ubicación funciona—ya aprendimos las reglas de éxito analizando 5 millones de negocios públicos en México."

### Ciclo de aprendizaje del modelo

El algoritmo aprende comparando diagnósticos pasados con resultados reales (no datos privados):

1. **Hipótesis:** El sistema dice "Este terreno tiene PAV alto pero precio bajo—debería subir"
2. **Validación:** En 12-24 meses, verifica con datos públicos: ¿subió de valor?
3. **Calibración:** Si SÍ, confirma variables predictivas. Si NO, recalibra pesos.

**Roadmap de predicción:**
- Fase actual: Diagnóstico (cómo está hoy)
- Fase futura: Predicción validada (qué pasará, con intervalos de confianza)

### Datasets premium a adquirir

Con parte del capital de inversión se planea adquirir:

| Dataset | Valor agregado | Costo |
|---------|----------------|-------|
| **Base de datos principal** | Movilidad, transacciones, foot traffic integrados | **$500,000 MXN/año** |
| Actualizaciones | Trimestrales (4 actualizaciones/año) | Incluido |

**Detalle del dataset principal:**
- Movilidad agregada de celulares — Flujos reales de población (supera visión estática de censos)
- Transacciones inmobiliarias reales — Precios de cierre vs. precios de lista/aspiracionales
- Foot traffic (tráfico peatonal) — Vibrancia comercial a nivel de calle

**Presupuesto:** $500K MXN/año representa ~14% de una ronda de $3.6M o ~9% de una ronda de $5.4M. Es una inversión significativa pero crítica para la diferenciación.

---

## 16. Escalabilidad y límites

### Escalabilidad geográfica

La infraestructura es agnóstica a la ciudad. Pasos para nueva ciudad:
1. Adquirir fuentes de datos locales
2. Ejecutar pipelines estándar
3. Calibrar parámetros
4. Validar con conocimiento local
5. Integrar al sistema multi-ciudad

### Escalabilidad por vertical

Las mismas herramientas sirven para retail, industrial, residencial, oficinas. La diferencia está en qué variables ponderar.

### Límites

**No sustituye estudios legales.** No verifica títulos, gravámenes ni situación fiscal.

**No sustituye ingeniería de detalle.** No evalúa capacidad de carga ni factibilidad de servicios a nivel de lote.

**No predice el futuro con certeza.** Los modelos proyectan tendencias pero el territorio está sujeto a shocks impredecibles.

**No elimina necesidad de juicio.** Los indicadores informan pero no deciden.

**No funciona sin datos.** En zonas con escasa cobertura, la precisión se degrada.

---

## 17. Posicionamiento competitivo

### vs. Consultoría tradicional

| Dimensión | Consultoría | Urbanalítica |
|-----------|-------------|--------------|
| Metodología | Implícita, varía | Explícita, replicable |
| Comparabilidad | Cada estudio único | Mismo marco |
| Auditabilidad | "Confía en el experto" | Rastreable |
| Acumulación | Se va con el consultor | Se acumula en sistema |
| Velocidad | Semanas/meses | Días/horas |
| Costo marginal | Alto | Bajo |

### vs. SaaS genéricos

| Dimensión | SaaS genérico | Urbanalítica |
|-----------|---------------|--------------|
| Adaptación local | Datos globales, poca profundidad | Fuentes mexicanas curadas |
| Métricas | Estándar (población, ingreso) | Especializadas (Amenity Space, Space Syntax) |
| Interpretación | Self-service | Acompañamiento disponible |
| Riesgo | Ausente o superficial | Capa completa |

Urbanalítica busca ser el sistema que sabe más del territorio mexicano que cualquier competidor global.

---

## 18. Ética y políticas públicas

### Responsabilidad territorial

Las decisiones territoriales tienen consecuencias que trascienden al inversor individual.

**Riesgos de mal uso:**
- Especulación que desplaza comunidades
- Información asimétrica que perjudica actores menos sofisticados
- Optimización que ignora externalidades negativas

**Principios:**
- Transparencia metodológica
- No participación en proyectos manifiestamente dañinos
- Consideración de impactos comunitarios
- Promoción de usos que mejoren el territorio

### Políticas públicas

Urbanalítica puede informar políticas sin capturarlas.

**Contribuciones:**
- Identificar zonas prioritarias para inversión pública
- Detectar áreas de riesgo
- Evaluar impacto ex-ante de proyectos
- Proveer benchmarks para planes de desarrollo

**Límites:**
- La política involucra valores que no se resuelven técnicamente
- El análisis debe complementarse con participación ciudadana
- El riesgo de "tecnocracia" es real

---

## 19. Ventaja competitiva y roadmap

### Ventaja competitiva

Difícil de replicar porque combina elementos que se refuerzan:

- **Integración teoría-datos-decisión:** No es solo datos, ni solo consultoría, ni solo software.
- **Base acumulativa:** Años de ventaja en datos procesados y modelos calibrados.
- **Red de validación:** Resultados probados contra desempeño real.
- **Talento escaso:** Perfiles híbridos concentrados.
- **Efecto de red:** Más clientes → más validación → mejores modelos → más clientes.

### Roadmap

**Fase actual: Diagnóstico sistematizado**
UbX y PAV funcionales para cualquier ubicación/activo en México.

**Fase siguiente: Simulación y escenarios**
"¿Qué pasa con el UbX/PAV si se construye esta infraestructura o cambia el uso?"

**Fase futura: Predicción validada**
Modelos entrenados con desempeño real, predicciones con intervalos de confianza.

**Fase aspiracional: Optimización prescriptiva**
"Dado tu objetivo y restricciones, este es el portafolio óptimo."

### Investigación abierta

Preguntas que guían desarrollo:
- ¿Qué combinación de variables del PAV mejor predice apreciación?
- ¿Cómo incorporar movilidad en tiempo real al UbX?
- ¿Cómo evoluciona el Amenity Space en el tiempo?
- ¿Qué umbrales de riesgo son aceptables por tipo de inversión?

---

## 20. Conclusiones

Urbanalítica propone leer el territorio como sistema complejo cuya estructura puede medirse y aprovecharse.

**Dos herramientas centrales:**
- **UbX Score:** Evalúa ubicaciones para usos específicos
- **PAV:** Evalúa activos físicos independiente del precio

Juntos permiten detectar la brecha entre precio de mercado y valor estructural—la señal más valiosa para inversión territorial.

**Es:**
- Laboratorio con fundamento teórico sólido
- Sistema que integra fuentes y metodologías en métricas comparables
- Infraestructura que acumula conocimiento con cada proyecto

**No es:**
- Predictor infalible del futuro
- Sustituto de estudios legales o ingeniería
- Herramienta para validar decisiones ya tomadas

**Apuesta:** Quien sistematice la lectura territorial tiene ventaja sobre quien opere con intuición y estudios aislados.

---

## 21. Referencias

**Economía urbana:**
- Von Thünen (1826). *Der isolierte Staat*
- Hotelling (1929). *Stability in Competition*
- Christaller (1933). *Die zentralen Orte in Süddeutschland*
- Krugman (1991). *Geography and Trade*

**Sistemas complejos:**
- Batty (2013). *The New Science of Cities*
- Barabási (2016). *Network Science*

**Space Syntax:**
- Hillier & Hanson (1984). *The Social Logic of Space*

**Amenity Space:**
- Hidalgo & Castañer (2015). *The Amenity Space and the Evolution of Neighborhoods*

**Clustering:**
- Campello et al. (2013). *HDBSCAN*
- Anselin (1995). *Local Indicators of Spatial Association*
