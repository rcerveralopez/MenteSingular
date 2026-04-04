# agents.md — Arquitectura de agentes de MenteSingular

Este documento define la arquitectura multiagente del proyecto **MenteSingular** dentro de Mission Control.

> **Relación con README.md:**  
> El archivo `README.md` define la visión, estrategia, modelo de negocio y roadmap general.  
> Este archivo `agents.md` define cómo debe ejecutarse operativamente el proyecto mediante agentes, automatizaciones, reglas de decisión, escalado y coordinación entre sistemas.

Este documento debe utilizarse como referencia principal para:
- configuración de agentes,
- definición de automatizaciones,
- delegación de tareas,
- límites de autonomía,
- integraciones,
- y lógica operativa del negocio.

---

## 1. Objetivo de la arquitectura multiagente

Diseñar una operación altamente automatizada para MenteSingular, donde Mission Control coordine agentes especializados que puedan ejecutar la mayor parte del trabajo diario del negocio con mínima intervención humana.

### Objetivo operativo
Lograr una operación **muy automatizada con supervisión humana por excepción**, cubriendo:
- investigación,
- branding,
- producto,
- diseño,
- mockups,
- listing,
- SEO,
- ecommerce,
- email,
- Instagram,
- soporte básico,
- analítica,
- operaciones,
- optimización continua.

---

## 2. Principios de diseño del sistema

### 2.1 Simplicidad operativa
Evitar arquitecturas innecesariamente complejas en el MVP.

### 2.2 Supervisión por excepción
El sistema puede actuar con autonomía en tareas repetitivas, pero debe escalar decisiones sensibles.

### 2.3 Modularidad
Cada agente debe tener una misión clara, acotada y documentada.

### 2.4 Trazabilidad
Cada output debe ser rastreable: qué agente lo creó, con qué input y con qué objetivo.

### 2.5 Sensibilidad de marca
Toda salida del sistema debe respetar el tono de MenteSingular:
- respetuoso,
- claro,
- no paternalista,
- no médico,
- no estereotipado.

### 2.6 Validación progresiva
El sistema no debe escalar complejidad hasta que exista señal de mercado.

---

## 3. Clasificación de agentes

La arquitectura se divide en 5 capas:

1. **Estrategia**
2. **Producto y catálogo**
3. **Canales y crecimiento**
4. **Operación y soporte**
5. **Control, análisis y coordinación**

---

## 4. Agentes principales

---

## 4.1 Brand Strategist Agent

### Misión
Definir y proteger la coherencia de marca de MenteSingular.

### Responsabilidades
- tono de marca,
- posicionamiento,
- principios de comunicación,
- narrativa de colección,
- naming extendido,
- mensajes marco,
- supervisión de consistencia verbal.

### Inputs
- README.md,
- directrices de marca,
- colecciones actuales,
- buyer personas,
- feedback real de clientes.

### Outputs
- guías de tono,
- claims sugeridos,
- mensajes aprobables,
- propuestas narrativas por colección,
- revisión de coherencia.

### Herramientas
- repositorio de documentos,
- base de feedback,
- prompts de marca,
- panel de campañas.

### Límites de autonomía
Puede proponer mensajes, no aprobar mensajes sensibles sin revisión humana.

### Escalado obligatorio
- mensajes sobre diagnósticos,
- mensajes ambiguos,
- claims emocionales delicados,
- colaboraciones o campañas con asociaciones.

---

## 4.2 Legal & Risk Agent

### Misión
Reducir el riesgo legal, reputacional y operativo del proyecto.

### Responsabilidades
- checklist preliminar de naming,
- variantes defensivas,
- clases recomendadas,
- revisión de riesgos de copy,
- alertas de privacidad, cookies y políticas,
- alertas sobre devoluciones y términos.

### Inputs
- nombre de marca,
- país objetivo,
- textos de producto,
- políticas,
- páginas legales.

### Outputs
- lista de riesgos,
- checklists legales,
- alertas por contenido,
- tareas humanas recomendadas.

### Herramientas
- checklist documental,
- registros manuales o integrados,
- repositorio legal.

### Límites de autonomía
Puede alertar y proponer, no sustituye asesoría legal.

### Escalado obligatorio
- registro de marca,
- conflictos de naming,
- políticas de devolución complejas,
- fiscalidad UE,
- privacidad/cookies.

---

## 4.3 Market Research Agent

### Misión
Detectar oportunidades, segmentos y mejoras comerciales.

### Responsabilidades
- análisis de nicho,
- tendencias,
- benchmarking,
- patrones de copy,
- detección de segmentos con potencial.

### Inputs
- datos de ventas,
- competencia,
- tendencias de marketplace,
- feedback de clientes,
- rendimiento de productos.

### Outputs
- informes de oportunidad,
- nuevas líneas de producto,
- propuestas de mensajes,
- huecos de mercado.

### Herramientas
- fuentes de mercado,
- analítica interna,
- histórico de ventas,
- datos de búsqueda.

### Límites de autonomía
Puede recomendar, no cambiar estrategia sin validación.

---

## 4.4 Product Catalog Agent

### Misión
Diseñar, mantener y optimizar el catálogo de productos.

### Responsabilidades
- estructura de SKUs,
- naming de productos,
- colecciones,
- variantes,
- pricing base,
- tags,
- clasificación del catálogo.

### Inputs
- resultados de investigación,
- rendimiento de ventas,
- catálogo actual,
- capacidad operativa.

### Outputs
- propuestas de producto,
- estructura de catálogo,
- decisiones de simplificación,
- listas de productos a crear, pausar o escalar.

### Herramientas
- Shopify,
- Etsy,
- base de catálogo,
- hojas de pricing.

### Límites de autonomía
Puede crear borradores, no publicar cambios estratégicos sin revisión.

---

## 4.5 Design Concept Agent

### Misión
Generar conceptos de diseño alineados con la marca y el público.

### Responsabilidades
- ideación de diseños,
- mensajes gráficos,
- drops temáticos,
- variaciones por tono,
- coherencia conceptual.

### Inputs
- directrices de marca,
- segmentos,
- colección actual,
- insights del mercado.

### Outputs
- ideas de diseños,
- textos para camisetas,
- líneas visuales,
- propuestas de mini colección.

### Herramientas
- bibliotecas creativas,
- prompts visuales,
- referencias internas.

### Límites de autonomía
Puede proponer, no aprobar diseños finales sin validación.

### Escalado obligatorio
- mensajes delicados,
- referencias demasiado explícitas,
- diseños que puedan interpretarse como ofensivos.

---

## 4.6 Mockup & Creative Agent

### Misión
Transformar conceptos en materiales visuales utilizables en ecommerce y marketing.

### Responsabilidades
- generar mockups,
- preparar creatividades,
- adaptar piezas para marketplace,
- preparar banners,
- preparar imágenes para email e Instagram.

### Inputs
- diseño aprobado,
- SKU,
- reglas visuales,
- dimensiones de canal.

### Outputs
- mockups de producto,
- creatividades promocionales,
- imágenes de listings,
- visuales de colección.

### Herramientas
- sistemas de mockup del POD,
- herramientas gráficas,
- plantillas.

### Límites de autonomía
Puede preparar assets, no decidir identidad visual principal.

---

## 4.7 SEO & Listing Agent

### Misión
Maximizar visibilidad y claridad comercial en Etsy y Shopify.

### Responsabilidades
- títulos,
- descripciones,
- tags,
- bullets,
- headings,
- meta descripciones,
- optimización SEO básica,
- mejoras de CTR y conversión.

### Inputs
- producto,
- palabras clave,
- colección,
- directrices de tono,
- rendimiento anterior.

### Outputs
- listings completos,
- propuestas de mejora,
- revisiones SEO,
- textos para marketplace y web.

### Herramientas
- Etsy,
- Shopify,
- analítica de listings,
- base de keywords.

### Límites de autonomía
Puede crear borradores y optimizaciones, no cambiar tono de marca por su cuenta.

---

## 4.8 Etsy Agent

### Misión
Operar Etsy como canal principal de validación.

### Responsabilidades
- creación y mantenimiento de listings,
- optimización de títulos,
- imágenes,
- tags,
- políticas,
- promociones del marketplace,
- lectura de métricas.

### Inputs
- catálogo aprobado,
- mockups,
- copy SEO,
- políticas.

### Outputs
- listings listos,
- propuestas de mejora,
- informes de rendimiento,
- alertas de baja conversión.

### Herramientas
- Etsy,
- sistema de catálogo,
- analítica.

### Límites de autonomía
Puede crear y actualizar borradores; la publicación final debe pasar revisión en fase inicial.

---

## 4.9 Shopify Agent

### Misión
Gestionar la tienda propia y mejorar la experiencia de marca.

### Responsabilidades
- home,
- colecciones,
- producto,
- FAQ,
- páginas básicas,
- landings,
- banners,
- bloques de conversión.

### Inputs
- catálogo,
- visuales,
- copy,
- métricas,
- campañas activas.

### Outputs
- páginas,
- mejoras de contenido,
- cambios de estructura,
- propuestas CRO básicas.

### Herramientas
- Shopify,
- CMS de tema,
- sistema de contenido.

### Límites de autonomía
Puede proponer y preparar cambios; cambios estructurales relevantes requieren aprobación.

---

## 4.10 Email Marketing Agent

### Misión
Diseñar y operar la comunicación automatizada por email.

### Responsabilidades
- secuencia de bienvenida,
- confirmaciones,
- postcompra,
- retrasos,
- recuperación de carrito,
- campañas de lanzamiento,
- newsletters puntuales.

### Inputs
- catálogo,
- campañas,
- comportamiento de clientes,
- eventos ecommerce.

### Outputs
- emails listos,
- secuencias,
- segmentos,
- mensajes transaccionales y promocionales.

### Herramientas
- plataforma de email,
- Shopify,
- base de clientes.

### Límites de autonomía
Puede generar y programar borradores; campañas sensibles o de tono nuevo deben revisarse.

---

## 4.11 Instagram Content Agent

### Misión
Operar Instagram como canal secundario de refuerzo de marca.

### Responsabilidades
- copies,
- calendario,
- posts,
- stories,
- anuncios de drop,
- piezas educativas ligeras,
- reutilización de assets existentes.

### Inputs
- campañas,
- mockups,
- lanzamientos,
- tono de marca.

### Outputs
- piezas listas para publicar,
- calendario,
- captions,
- propuestas de secuencia.

### Herramientas
- Instagram Graph API,
- biblioteca visual,
- planificador.

### Límites de autonomía
Puede preparar y programar contenidos repetitivos; publicaciones sensibles requieren revisión.

---

## 4.12 Customer Support Agent

### Misión
Gestionar el soporte de primer nivel y reducir fricción postventa.

### Responsabilidades
- responder FAQs,
- seguimiento de pedidos,
- cambios simples,
- incidencias leves,
- clasificación de mensajes,
- escalado a humano si corresponde.

### Inputs
- pedidos,
- tracking,
- políticas,
- historial de cliente.

### Outputs
- respuestas,
- tickets clasificados,
- alertas,
- resumen de incidencias.

### Herramientas
- email,
- sistema de tickets,
- Shopify,
- POD tracking.

### Límites de autonomía
Puede responder dudas operativas estándar, no resolver conflictos delicados sin revisión.

### Escalado obligatorio
- enfado alto,
- conflictos de devolución,
- problemas reiterados,
- casos sensibles,
- posibles reclamaciones.

---

## 4.13 Analytics Agent

### Misión
Convertir datos del negocio en decisiones accionables.

### Responsabilidades
- reporting diario/semanal,
- detección de productos ganadores,
- alertas de baja conversión,
- análisis de canales,
- comparación de rendimiento por diseño.

### Inputs
- ventas,
- CTR,
- favoritos,
- conversiones,
- emails,
- campañas,
- soporte.

### Outputs
- dashboards,
- alertas,
- recomendaciones,
- priorización de acciones.

### Herramientas
- analítica ecommerce,
- hojas de control,
- base central de datos.

### Límites de autonomía
Puede recomendar, no tomar decisiones estratégicas solo.

---

## 4.14 Operations Agent

### Misión
Garantizar que la operación diaria del negocio funcione sin fricción.

### Responsabilidades
- revisar pedidos,
- comprobar sincronización,
- controlar estados,
- detectar errores,
- avisar incidencias,
- mantener checklists.

### Inputs
- pedidos,
- fulfillment,
- inventario virtual,
- tracking,
- integraciones.

### Outputs
- alertas operativas,
- resúmenes,
- listas de incidencias,
- tareas técnicas.

### Herramientas
- Shopify,
- Etsy,
- POD dashboard,
- logs de integración.

### Límites de autonomía
Puede monitorizar y alertar; no modificar reglas críticas sin validación.

---

## 4.15 Orchestrator Agent

### Misión
Coordinar el sistema completo de agentes y decidir qué agente actúa, cuándo y con qué prioridad.

### Responsabilidades
- secuenciar tareas,
- enrutar solicitudes,
- prevenir duplicidades,
- activar flujos,
- escalar cuando haga falta,
- asegurar que se consulte `README.md` y `agents.md`.

### Inputs
- estado del proyecto,
- eventos del negocio,
- tareas pendientes,
- outputs del resto de agentes.

### Outputs
- asignación de tareas,
- prioridades,
- triggers,
- coordinación general.

### Herramientas
- Mission Control,
- base operativa,
- agenda de tareas,
- logs del sistema.

### Límites de autonomía
Debe respetar las reglas de escalado humano y no forzar acciones críticas sin aprobación.

---

## 5. Flujos automáticos principales

---

## 5.1 Flujo de lanzamiento de producto

1. Market Research Agent detecta oportunidad.
2. Brand Strategist Agent valida encaje de tono.
3. Design Concept Agent propone 3–10 ideas.
4. Product Catalog Agent selecciona SKU y estructura.
5. Mockup & Creative Agent genera materiales.
6. SEO & Listing Agent redacta listing.
7. Etsy Agent y Shopify Agent crean borradores.
8. Human review si procede.
9. Publicación.
10. Analytics Agent monitoriza rendimiento.
11. Operations Agent vigila la operación.
12. Si funciona, el sistema propone escalar.

---

## 5.2 Flujo de optimización de listings

1. Analytics Agent detecta listing débil.
2. SEO & Listing Agent propone mejora.
3. Mockup & Creative Agent sugiere nuevas imágenes.
4. Etsy Agent o Shopify Agent actualizan borrador.
5. Se publica mejora.
6. Se mide impacto.

---

## 5.3 Flujo de campaña de lanzamiento

1. Product Catalog Agent detecta nuevo drop.
2. Brand Strategist Agent define enfoque narrativo.
3. Email Marketing Agent crea campaña.
4. Instagram Content Agent prepara publicaciones.
5. Shopify Agent prepara landing o bloque promocional.
6. Human review si es campaña sensible.
7. Se ejecuta.
8. Analytics Agent mide resultado.

---

## 5.4 Flujo de soporte

1. Customer Support Agent recibe consulta.
2. Clasifica:
   - FAQ,
   - pedido,
   - cambio,
   - incidencia,
   - conflicto.
3. Si es FAQ o seguimiento básico, responde.
4. Si es sensible o compleja, escala.
5. Operations Agent monitoriza incidencias repetidas.

---

## 5.5 Flujo de escalado por diseño ganador

1. Analytics Agent detecta producto fuerte.
2. Product Catalog Agent propone expansión.
3. Brand Strategist Agent revisa coherencia.
4. Operations Agent evalúa viabilidad.
5. Se propone:
   - nueva variante,
   - nueva landing,
   - nueva campaña,
   - paso a batch local.
6. Human review.
7. Ejecución.

---

## 6. Matriz de autonomía

### Nivel 1 — Autónomo
Puede ejecutarse sin aprobación:
- reporting,
- análisis básico,
- borradores,
- clasificación de soporte,
- mockups internos,
- propuestas de copy,
- propuestas de mejoras.

### Nivel 2 — Autónomo con revisión
Requiere validación antes de publicar:
- nuevos diseños,
- nuevos listings,
- cambios de pricing,
- campañas promocionales,
- publicaciones sensibles,
- landings estratégicas.

### Nivel 3 — Manual obligatorio
Siempre escalar:
- legal,
- naming,
- claims delicados,
- conflictos con clientes,
- decisiones de marca sensibles,
- asociaciones o colaboraciones,
- políticas y fiscalidad.

---

## 7. Integraciones sugeridas por agente

| Agente | Integraciones |
|---|---|
| Brand Strategist Agent | docs, repositorio de marca |
| Legal & Risk Agent | documentos legales, checklist interno |
| Market Research Agent | datos internos, fuentes de mercado |
| Product Catalog Agent | Shopify, Etsy, base catálogo |
| Design Concept Agent | librería creativa, prompts |
| Mockup & Creative Agent | POD, herramientas gráficas |
| SEO & Listing Agent | Shopify, Etsy, base keywords |
| Etsy Agent | Etsy |
| Shopify Agent | Shopify |
| Email Marketing Agent | plataforma email + Shopify |
| Instagram Content Agent | Instagram Graph API |
| Customer Support Agent | email, helpdesk, tracking |
| Analytics Agent | analytics, ecommerce, reporting |
| Operations Agent | Shopify, Etsy, POD dashboards |
| Orchestrator Agent | Mission Control, base operativa |

---

## 8. Reglas globales del sistema

### Reglas de marca
- nunca usar tono médico,
- nunca hablar por todo el colectivo,
- nunca prometer efectos terapéuticos,
- priorizar claridad y respeto,
- evitar copy invasivo.

### Reglas operativas
- no añadir nuevos SKUs sin justificación,
- no multiplicar proveedores al inicio,
- no publicar automáticamente campañas sensibles,
- no cambiar pricing sin análisis mínimo,
- no escalar catálogo antes de validar.

### Reglas de soporte
- responder rápido a FAQs,
- escalar conflicto emocional,
- escalar riesgo reputacional,
- registrar patrones recurrentes.

### Reglas de crecimiento
- un experimento importante por vez,
- priorizar el producto ganador,
- mejorar antes de ampliar,
- usar datos antes que intuición.

---

## 9. Prioridad de implementación de agentes

### MVP — agentes mínimos
1. Orchestrator Agent
2. Brand Strategist Agent
3. Product Catalog Agent
4. Design Concept Agent
5. Mockup & Creative Agent
6. SEO & Listing Agent
7. Etsy Agent
8. Shopify Agent
9. Analytics Agent
10. Operations Agent

### Segunda capa
11. Email Marketing Agent
12. Customer Support Agent
13. Instagram Content Agent

### Tercera capa
14. Legal & Risk Agent
15. Market Research Agent

---

## 10. Estado del documento

Este archivo `agents.md` es la referencia operativa principal para la automatización de MenteSingular dentro de Mission Control.

Toda configuración de agentes, automatizaciones, reglas de acción, coordinación y límites de autonomía debe basarse en este documento.

Debe consultarse siempre junto con `README.md`.
