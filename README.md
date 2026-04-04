# MenteSingular

Marca de ropa print-on-demand para personas neurodivergentes en España, diseñada para operar de forma altamente automatizada mediante agentes y sistemas coordinados desde Mission Control.

> **Importante:** este proyecto se apoya en un segundo documento maestro llamado **`agents.md`**, donde se define la arquitectura de agentes, sus responsabilidades, inputs, outputs, límites de autonomía, integraciones y flujos operativos.  
> El archivo `README.md` describe la visión general, estrategia, modelo operativo y roadmap del negocio.  
> El archivo `agents.md` debe utilizarse como referencia principal para la ejecución automatizada del proyecto dentro de Mission Control.

---

## 1. Resumen del proyecto

**MenteSingular** es una marca de ropa POD enfocada en personas neurodivergentes en España, con expansión posterior a la UE. El proyecto nace con una visión clara: construir una marca digital sensible, respetuosa y comercialmente viable, operada de forma muy automatizada mediante Mission Control, con supervisión humana solo por excepción.

La estrategia inicial se basa en:
- validación rápida,
- baja fricción operativa,
- catálogo corto,
- combinación de Etsy + Shopify,
- un único proveedor POD principal,
- y escalado solo cuando exista señal real de demanda.

El objetivo no es solo vender camisetas, sino crear una **marca automatizable**, con operaciones, marketing, catálogo, contenido, soporte y analítica organizados desde una arquitectura multiagente.

---

## 2. Propósito del proyecto

Construir una marca de ropa para personas neurodivergentes que combine:

- identidad,
- comodidad,
- mensajes respetuosos,
- validación rápida de producto,
- venta digital simple,
- automatización realista,
- y posibilidad de crecimiento posterior.

El proyecto debe ser diseñado para que Mission Control pueda operar la mayor parte del negocio y que el fundador solo tenga que intervenir en:
- aprobaciones sensibles,
- conexión de APIs,
- supervisión general,
- y decisiones críticas.

---

## 3. Visión del negocio

MenteSingular debe convertirse en una marca digital con una operación escalable y altamente automatizada, capaz de:

- detectar oportunidades de producto,
- crear nuevas colecciones,
- generar mockups,
- publicar listings,
- optimizar fichas de producto,
- mejorar la web,
- generar emails,
- programar contenido,
- responder soporte básico,
- monitorizar métricas,
- y proponer acciones de mejora.

La automatización debe ser profunda, pero no irresponsable.  
La arquitectura del sistema debe diseñarse como un negocio **autónomo con supervisión humana por excepción**, no como una automatización ciega del 100%.

---

## 4. Propuesta de valor

> **MenteSingular transforma una necesidad de expresión, identidad y comodidad en una marca de ropa POD sensible, escalable y operada por sistemas automatizados desde Mission Control.**

### Diferenciadores
- foco específico en neurodivergencia desde el respeto,
- mensajes identitarios sin tono médico,
- atención al confort y a la fricción sensorial,
- validación de producto con estructura low-risk,
- operación diseñada para automatización desde el inicio,
- combinación de marketplace + tienda propia,
- escalado basado en datos reales.

---

## 5. Público objetivo

### Público principal
Personas neurodivergentes en España que valoran:
- prendas con mensajes con los que identificarse,
- estética sobria o minimalista,
- compra sencilla,
- comodidad,
- tono respetuoso y no invasivo.

### Público secundario
- familiares,
- parejas,
- amistades que compran para regalar,
- personas afines a la neurodiversidad,
- compradores sensibles a proyectos inclusivos.

### Segmento inicial recomendado
Adultos con afinidad hacia mensajes relacionados con:
- claridad,
- procesamiento,
- sensibilidad,
- rutinas,
- comunicación diferente,
- autorreconocimiento.

---

## 6. Posicionamiento de marca

MenteSingular debe posicionarse como una marca:

- sensible,
- clara,
- minimalista,
- emocionalmente inteligente,
- respetuosa,
- moderna,
- no infantilizada,
- no agresiva,
- no paternalista.

### Principios de comunicación
- hablar desde experiencias, no en nombre de todo el colectivo,
- evitar promesas terapéuticas o claims médicos,
- priorizar claridad, calma y legibilidad,
- usar mensajes directos, humanos y limpios,
- evitar complejidad innecesaria.

---

## 7. Objetivo operativo

Diseñar una operación donde Mission Control gestione la mayor parte del trabajo diario del negocio.

### Resultado deseado
Un sistema donde la automatización cubra:

- diseño conceptual,
- mockups,
- copy,
- listings,
- SEO,
- web,
- email,
- contenido,
- reporting,
- soporte inicial,
- y propuestas de optimización.

### Intervención humana esperada
La intervención humana debe quedar limitada a:
- revisión legal,
- aprobaciones de marca,
- revisión de mensajes delicados,
- decisiones estratégicas,
- validación de campañas,
- conexión de APIs y plataformas,
- y resolución de incidencias complejas.

---

## 8. Canales de venta

### Canal principal de validación
**Etsy**

Razones:
- menor fricción de lanzamiento,
- tráfico interno,
- SEO propio,
- menor coste fijo inicial,
- ideal para validar diseños y mensajes.

### Canal de construcción de marca
**Shopify**

Razones:
- mejor control de experiencia,
- mejor branding,
- mejor estructura para email marketing y SEO,
- mejor base para automatización y escalado.

---

## 9. Modelo de producto inicial

### Estrategia
Comenzar con:
- 6 diseños,
- 3 SKUs principales,
- pocas variantes,
- baja complejidad,
- lanzamiento rápido.

### SKUs base
1. **Unisex Core**
2. **Premium Heavy**
3. **Sensory-Lite**

### Colección inicial
Mensajes orientados a identidad, claridad, sensibilidad y experiencia cotidiana.

Ejemplos iniciales:
- MenteSingular
- No es pereza. Es procesamiento.
- Sensibilidad alta · Ruido bajo
- Necesito claridad, no presión
- Mis rutinas me cuidan
- Comunico diferente

---

## 10. Producción y fulfillment

### Estructura recomendada
- 1 proveedor POD principal
- 1 opción secundaria
- 1 proveedor local para lotes futuros si aparece un diseño ganador

### Recomendación inicial
- **POD principal:** Printful
- **Alternativa:** TPOP
- **Escalado local futuro:** impresor local para batch si la demanda lo justifica

### Principio operativo
No añadir complejidad al principio.  
La prioridad es validar:
- mensajes,
- conversión,
- aceptación del producto,
- señal de mercado,
- y margen básico.

---

## 11. Automatización del negocio

La operación debe estar estructurada por agentes especializados coordinados desde Mission Control.

### Referencia obligatoria
Toda la arquitectura multiagente, la lógica de automatización, la asignación de tareas y los límites de autonomía están definidos en el archivo:

# `agents.md`

Ese archivo debe considerarse el documento de referencia operativa para:
- definición de agentes,
- automatizaciones,
- flujos,
- prioridades por sistema,
- reglas de escalado,
- y ejecución autónoma del proyecto.

---

## 12. Qué debe automatizarse

### Alta prioridad de automatización
- propuestas de diseños,
- generación de copy,
- mockups,
- alta de productos en borrador,
- títulos y descripciones,
- SEO básico,
- colecciones,
- mejoras de home y landings,
- secuencias de email,
- reporting,
- análisis de métricas,
- soporte FAQ inicial,
- calendario de contenido.

### Automatización con revisión humana
- publicación final de productos,
- campañas promocionales,
- nuevos mensajes de marca,
- cambios de pricing,
- nuevos drops,
- nuevas landings estratégicas.

### Supervisión humana obligatoria
- legal y marca,
- mensajes sensibles,
- soporte complejo,
- devoluciones conflictivas,
- colaboraciones,
- decisiones de expansión.

---

## 13. Stack e integraciones recomendadas

### Ecommerce
- Etsy
- Shopify

### POD
- Printful
- TPOP
- impresor local para batch futuro

### Marketing
- plataforma de email conectada a Shopify
- Instagram Graph API como canal secundario
- SEO básico en Etsy y Shopify

### Datos y automatización
- Mission Control como capa de coordinación
- Supabase o Airtable como capa operativa
- integraciones vía API
- sistema de reporting centralizado

---

## 14. Flujos principales del negocio

### Flujo de producto
1. Detectar oportunidad o colección.
2. Proponer diseños.
3. Generar mockups.
4. Redactar listing y SEO.
5. Crear borrador.
6. Revisar y publicar.
7. Monitorizar.
8. Iterar o escalar.

### Flujo de marketing
1. Detectar lanzamiento o producto ganador.
2. Generar emails, banners y piezas de contenido.
3. Preparar publicaciones.
4. Lanzar.
5. Analizar resultados.
6. Ajustar.

### Flujo de soporte
1. Clasificar consulta.
2. Responder automáticamente si es FAQ.
3. Escalar si es sensible o compleja.

### Flujo de mejora continua
1. Revisar métricas.
2. Detectar producto fuerte o débil.
3. Proponer acción:
   - mejorar listing,
   - cambiar imagen,
   - crear nueva variación,
   - pausar producto,
   - ampliar colección.

---

## 15. Roadmap por fases

### Fase 1 — Fundamentos
- naming y revisión preliminar,
- dominios,
- identidad visual mínima,
- setup técnico base,
- elección de proveedor POD.

### Fase 2 — Catálogo inicial
- 6 diseños,
- 3 SKUs,
- mockups,
- listings Etsy,
- políticas básicas,
- primeras pruebas de venta.

### Fase 3 — Shopify y marca
- home,
- colección,
- FAQ,
- páginas básicas,
- SEO inicial,
- base de email marketing.

### Fase 4 — Automatización operativa
- agentes clave activos,
- reporting,
- soporte básico,
- automatizaciones de catálogo,
- optimización recurrente.

### Fase 5 — Escalado
- detección de ganador,
- nueva colección,
- prueba batch local,
- campañas puntuales,
- expansión de automatización.

---

## 16. KPIs principales

### Validación
- 6 listings publicados,
- primeras 10 ventas,
- 1 diseño ganador,
- CTR por listing,
- favoritos,
- conversión por producto.

### Operación
- margen por unidad,
- incidencias por pedido,
- tiempo de preparación,
- devoluciones,
- ratio de soporte.

### Escalado
- crecimiento de email,
- ventas repetidas,
- tráfico Shopify,
- rendimiento por colección,
- estabilidad de automatizaciones.

---

## 17. Riesgos clave

- conflicto de marca o naming,
- tono poco sensible,
- complejidad operativa prematura,
- demasiados SKUs al inicio,
- escalado sin validación,
- automatización sin reglas claras,
- mala calidad de producto o mensaje.

---

## 18. Supuestos iniciales

- el canal principal inicial será Etsy,
- Shopify actuará como base de marca y escalado,
- se trabajará con un único POD principal al principio,
- el catálogo inicial será pequeño,
- la automatización será muy amplia, pero no total sin supervisión,
- el tono de marca priorizará respeto, claridad y simplicidad,
- Mission Control será el coordinador principal del sistema.

---

## 19. Prioridades inmediatas

1. Revisar naming y variantes defensivas.
2. Registrar dominios.
3. Definir identidad visual mínima.
4. Elegir proveedor POD principal.
5. Preparar 6 diseños base.
6. Crear mockups.
7. Configurar Etsy.
8. Montar Shopify básico.
9. Definir agentes y automatizaciones.
10. Activar reporting y mejora continua.

---

## 20. Relación con `agents.md`

Este documento define **qué es el proyecto y cómo debe funcionar a nivel de negocio**.

El archivo **`agents.md`** define:
- quién hace qué dentro del sistema,
- qué automatizaciones existen,
- qué herramientas usa cada agente,
- qué tareas requieren aprobación,
- cómo se conectan entre sí los agentes,
- y cómo debe ejecutarse la operación del negocio dentro de Mission Control.

**Toda decisión técnica u operativa sobre agentes debe consultar primero `agents.md`.**

---

## 21. Estado del documento

Este `README.md` es la fuente principal de verdad estratégica del proyecto MenteSingular.

Debe servir como base para:
- visión,
- estrategia,
- posicionamiento,
- roadmap,
- estructura operativa,
- y coordinación general del proyecto.

La ejecución automatizada del proyecto debe apoyarse de forma complementaria y obligatoria en el archivo `agents.md`.
