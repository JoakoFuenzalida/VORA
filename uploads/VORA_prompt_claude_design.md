# PROMPT PARA CLAUDE DESIGN — Sitio web VORA

> **Cómo usar este prompt:** copiar y pegar el bloque completo desde "Contexto del proyecto" hasta el final. El logo se sube por separado como archivo adjunto en Claude Design (`Logo_vora_3.png`).

---

## Contexto del proyecto

Necesito construir el sitio web corporativo de **VORA**, una empresa chilena de servicios profesionales de tecnología fundada en 2016 y con sede en Santiago. El sitio se presenta como parte de una licitación pública para un proyecto de plataforma hotelera, por lo que debe transmitir seriedad, madurez técnica y solidez institucional. La comisión evaluadora va a verificar el sitio para validar información institucional, experiencia, equipo y capacidades técnicas.

**Formato:** **single page** con navegación por anclas (los botones del header hacen scroll suave a cada sección).
**Deploy:** Vercel (dominio `vora.vercel.app`).
**Stack:** Next.js (App Router) + Tailwind CSS + componentes accesibles (shadcn/ui o Radix UI).

---

## Identidad de marca

- **Nombre:** VORA
- **Significado del acrónimo:** Vision, Operations, Results & Advancement (usar solo como frase secundaria, no como título principal)
- **Bajada / tagline:** "Plataformas digitales de misión crítica para operaciones que no pueden detenerse"
- **Logo:** una rana estilizada azul-petróleo con el texto "VORA" debajo. La rana simboliza la conexión con la sostenibilidad ambiental (bio-indicador). Adjunto la imagen aparte.

### Paleta de colores

- **Primario (azul-petróleo del logo):** aproximadamente `#3B7A8B` — usar para acentos, botones primarios, enlaces destacados, iconografía
- **Primario oscuro (hover / énfasis):** `#2A5A68`
- **Fondo:** blanco `#FFFFFF` (secciones alternas con gris muy claro `#F7F8F9`)
- **Texto principal:** gris casi negro `#1A1F24`
- **Texto secundario:** gris medio `#5A6470`
- **Bordes y separadores:** `#E5E7EA`

Máximo cinco colores en total, sin acentos fluor ni gradientes llamativos.

### Tipografía

- **Sans-serif limpia y corporativa** tipo Inter, Söhne o similar
- Dos familias como máximo (una para todo el sitio está bien)
- Jerarquía clara: H1 grande y contundente, H2 seccional, cuerpo cómodo de leer (16-18px)

### Tono visual

**Corporativo sobrio, consultora tech seria.** Aire generoso, tipografía protagonista, mínimo ornamento. Nada de ilustraciones cartoon, gradientes coloridos, glassmorphism ni "web startup 2020". Referencias mentales: sitios de consultoras de arquitectura de software o de ingeniería industrial, no de agencias creativas.

---

## Estructura del sitio (single page con anclas)

Header sticky con el logo a la izquierda y navegación a la derecha. Los items del menú son:

`Inicio` · `Nosotros` · `Experiencia` · `Equipo` · `Capacidades` · `Recursos` · `Contacto`

Cada uno hace scroll suave (`scroll-behavior: smooth`) hasta su sección. Al hacer scroll, la sección visible se resalta en el nav.

---

## Sección 1 — HERO (`#inicio`)

- **Título grande:** Plataformas digitales de misión crítica para operaciones que no pueden detenerse.
- **Subtítulo:** Diseñamos, construimos y operamos sistemas transaccionales de alta exigencia para retail, hotelería, logística y servicios financieros. 10 años, más de 30 proyectos y 168 personas.
- **Dos botones CTA:** "Conocer nuestra experiencia" (ancla a #experiencia) · "Hablemos" (ancla a #contacto, botón secundario/outline)
- **Fondo:** blanco o gris muy claro. Opcionalmente, un patrón geométrico sutil o líneas muy tenues. No usar imagen de stock corporativa (mujer con laptop sonriendo, etc.).
- **Franja inferior con 4 números:** `10 años` de trayectoria · `168` personas · `30+` proyectos · `15` plataformas en operación 24/7

---

## Sección 2 — NOSOTROS (`#nosotros`)

### 2.1 Quiénes somos
Párrafo introductorio:

> VORA es una empresa chilena de servicios profesionales de tecnología fundada en 2016. Nos especializamos en el diseño, desarrollo, implantación y operación de plataformas de misión crítica para industrias con operación distribuida y alta exposición al cliente final: retail, hotelería, logística y transporte, servicios financieros. A diez años de nuestra fundación, hemos ejecutado más de 30 proyectos de este tipo, de los cuales 15 continúan en operación bajo contratos de servicio vigentes.

### 2.2 Misión · Visión · Valores (3 tarjetas en fila, valores en lista después)

**Misión.** Diseñar, construir y operar plataformas digitales de misión crítica para industrias con operación distribuida y alta exposición al cliente final, con foco en continuidad operacional, seguridad y coherencia entre arquitectura y costo.

**Visión.** Ser el socio tecnológico chileno de referencia para operaciones que no pueden detenerse, reconocido por la calidad de sus soluciones a medida, la continuidad de sus equipos y la disciplina de su ingeniería.

**Valores** (bloque debajo, con 5 items, cada uno con un ícono simple tipo lucide-react):

1. **Continuidad.** Cuidamos la continuidad de nuestros equipos y la de la operación de nuestros clientes por igual. 62% de la dotación técnica supera los 5 años en la compañía.
2. **Coherencia técnica.** La arquitectura, el costo y el plan de trabajo deben decir la misma verdad.
3. **Ingeniería honesta.** No imponemos modelos de referencia genéricos a industrias con particularidades operacionales.
4. **Seguridad como práctica.** La seguridad se decide al comienzo, no al cierre.
5. **Sostenibilidad operacional.** Dimensionamos a la demanda real y elegimos regiones de menor intensidad de carbono cuando es viable.

### 2.3 Nuestras oficinas (2 tarjetas)

**Casa matriz — Santiago**
Av. Apoquindo 4700, piso 14, Las Condes, Región Metropolitana
+56 2 2450 8000 · contacto@vora.cl
1.100 m² · 145 puestos · Laboratorio de integración de hardware

**Oficina Concepción**
Av. Chacabuco 726, oficina 802, Concepción, Región del Biobío
+56 41 2245 300
220 m² · 32 puestos

### 2.4 Certificaciones (fila de badges/tarjetas con nombre y año)

- ISO 9001:2015 — Gestión de Calidad (vigente desde 2018)
- ISO/IEC 27001:2022 — Seguridad de la Información (vigente desde 2020)
- ISO/IEC 20000-1:2018 — Gestión de Servicios de TI (vigente desde 2022)
- CMMI for Development, Nivel 3 (evaluación vigente desde 2021)

---

## Sección 3 — EXPERIENCIA (`#experiencia`)

### 3.1 Industrias atendidas (chips o iconos en fila)
Retail · Hotelería · Logística y transporte · Servicios financieros

### 3.2 Volumen operado (4 números grandes en fila)

- **+8,4 M** transacciones mensuales
- **+3.500** usuarios operacionales activos
- **99,7 %** disponibilidad promedio 2025
- **+52** integraciones activas

### 3.3 Casos destacados (3 tarjetas grandes en columna o grid 3x1)

**Proyecto 1 — Plataforma de Gestión Hotelera Multi-Propiedad**
Cadena de 6 hoteles urbanos chilenos con problemática de inventario perecible, múltiples canales de distribución y propiedades con conectividad no garantizada. Desarrollamos una arquitectura híbrida con componente on-premise autónomo.
Métricas:
- 6 propiedades · 520 habitaciones
- 99,8 % de disponibilidad
- 0 incidentes de sobreventa desde el paso a producción
- ~120.000 reservas al año · 8 canales integrados
- −38 % en tiempo de check-in

**Proyecto 2 — Trazabilidad y Distribución Retail**
Cadena de retail de 45 puntos de venta con requerimiento de sincronización de inventario y precios en tiempo real hacia distintos canales.
Métricas:
- 45 puntos de venta sincronizados en tiempo real
- +2,3 M de SKU sincronizados diariamente
- 99,9 % de disponibilidad en peaks (cumplimiento SLA)
- −64 % en tiempo de propagación de cambios de precio

**Proyecto 3 — Gestión de Activos con Operación Remota**
Operador logístico con sitios remotos conectados por enlace satelital. Diseño de sistema con operación autónoma ante desconexión y sincronización posterior sin pérdida.
Métricas:
- 17 sitios remotos con enlace satelital
- Autonomía comprobada de 96 horas ante desconexión
- 0 pérdidas de información en 30 meses
- 99,5 % de disponibilidad del componente en sitio

### 3.4 Testimonios (3 tarjetas con quote grande, nombre y cargo)

> "Trabajamos con VORA la plataforma que integra la reserva, la operación diaria y la conciliación de nuestras propiedades. Entendieron desde el primer día que un hotel no se apaga: el componente que corre en cada propiedad sigue vendiendo incluso cuando el enlace con la nube se cae, y después se sincroniza sin que nadie tenga que digitar dos veces."
> **Verónica Alcaíno** · Gerente de Operaciones, Cadena Hotelera Urbana

> "Nos entregaron más de lo que prometieron. La sincronización de precios e inventario hacia los canales de venta funciona mejor que la que teníamos antes, con la mitad de incidencias y sin sorpresas en las temporadas altas."
> **Cristián Bahamondes** · Gerente de Tecnología, Cadena de Retail (45 puntos de venta)

> "Nuestros sitios remotos están conectados por enlace satelital y antes vivíamos con miedo a las caídas. La solución de VORA los deja operar solos durante días si es necesario, y cuando el enlace vuelve, todo se pone al día sin pérdidas. Es la primera vez que dormimos tranquilos."
> **Álvaro Reveco** · Director de Operaciones, Operador Logístico Regional

---

## Sección 4 — EQUIPO (`#equipo`)

### 4.1 Estructura (introducción breve)

> Operamos bajo una estructura de "práctica": cada proyecto se conforma con especialistas asignados desde seis unidades funcionales permanentes. 168 personas en dotación total, 121 técnicas.

### 4.2 Directorio y socios fundadores (3 tarjetas)

**Ricardo Fuenzalida Larraín** — CEO y socio fundador
Ingeniero Civil Industrial (Universidad de Chile) · MBA (UAI) · 22 años en tecnología para operaciones distribuidas.

**Camila Vergara Ossandón** — Directora de Arquitectura y Nube · socia fundadora
Ingeniera Civil en Computación (USM) · AWS Solutions Architect Professional · Azure Solutions Architect Expert · 18 años.

**Sebastián Toro Meneses** — Director de Ingeniería de Software · socio fundador
Ingeniero Civil en Computación (PUC) · CMMI Associate · 20 años en desarrollo para industrias críticas.

### 4.3 Gerencias (4 tarjetas más pequeñas)

**María José Pinto Villablanca** — Directora de Ciberseguridad
CISSP · CISM · Lead Auditor ISO/IEC 27001 · 15 años, foco PCI DSS e ISO 27001.

**Andrés Lagos Herrera** — Director de Operación y Soporte
ITIL 4 Managing Professional · 16 años en gestión de servicios de TI y SLA.

**Francisca Muñoz Aravena** — Directora de Datos e Integración
Magíster en Ciencia de Datos · 13 años en integración de sistemas y plataformas de datos.

**Rodrigo Espinoza Fernández** — Director de Calidad y Aseguramiento
CMMI Associate · Lead Auditor ISO 9001 · 17 años en aseguramiento de calidad.

### 4.4 Organigrama (diagrama simple SVG)

Directorio → CEO → 6 direcciones en paralelo (Arquitectura y Nube, Ingeniería de Software, Datos e Integración, Ciberseguridad, Calidad y Aseguramiento, Operación y Soporte) + 3 gerencias transversales al pie (Administración, Comercial, Personas). Diagrama sobrio, cajas con bordes finos, sin colores llamativos.

---

## Sección 5 — CAPACIDADES (`#capacidades`)

### 5.1 Líneas de negocio (4 tarjetas en grid)

**Plataformas a medida.** Diseño y construcción de sistemas transaccionales y de gestión operacional, con arquitecturas nativas de nube, on-premise o híbridas.

**Datos e integración.** Consolidación de fuentes dispersas, migración de sistemas legados, analítica operacional e integración con canales externos.

**Operación y soporte.** Gestión de niveles de servicio, mantención evolutiva y preventiva, y operación de plataformas bajo SLA.

**Ciberseguridad aplicada.** Segmentación de redes, gestión de identidades y accesos, cifrado y cumplimiento normativo sectorial.

### 5.2 Alianzas tecnológicas (grid con nombre y descripción breve)

- **AWS** — Partner de nivel avanzado, equipos certificados en arquitectura, datos y seguridad
- **Microsoft Azure** — Partner de nivel avanzado
- **SiteMinder** — Gestores de canales de distribución hotelera
- **SISAP** — QSA para cumplimiento PCI DSS
- **ASSA ABLOY Hospitality** — Convenio marco de hardware hotelero
- **Dormakaba** — Convenio marco de hardware hotelero
- **Transbank** — Integración de terminales y cumplimiento PCI DSS

### 5.3 Metodologías (lista agrupada)

**Ingeniería y calidad:** CMMI Nivel 3 · ISO 9001:2015 · OWASP SAMM
**Seguridad:** ISO/IEC 27001:2022 · NIST CSF 2.0 · OWASP ASVS 4.0 · CIS Benchmarks · SLSA 3
**Operación:** ISO/IEC 20000-1:2018 · ITIL 4
**Proyectos:** PMBOK 7 · Scrum · Kanban · SAFe

### 5.4 Infraestructura y capacidad

- **Nube pública:** AWS (us-east-1 principal, sa-east-1 DR) · Azure (Brazil South principal, East US failover)
- **SOC 24/7/365** operado desde casa matriz Santiago
- **Laboratorio de integración** con hardware hotelero (ASSA ABLOY VingCard, Dormakaba Saflok), retail y terminales Transbank
- **Ambiente permanente de entrenamiento** con datos ficticios
- **121 personas técnicas** · 4 equipos scrum activos en simultáneo · ambientes DEV/QA/PREPROD/PROD por cliente

---

## Sección 6 — RECURSOS (`#recursos`)

Grid de 3 o 4 tarjetas de artículos/recursos. Es un placeholder aspiracional (deseable en la licitación).

- **Artículo** — "Cómo diseñar operación autónoma para propiedades con conectividad no garantizada"
- **Artículo** — "PCI DSS 4.0 en integraciones de terminales Transbank: qué cambió"
- **Artículo** — "Trazabilidad multi-canal sin sobreventa: patrones y trampas"
- **Webinar** — "Arquitectura híbrida nube-borde para hotelería" (30 min)

Cada tarjeta con un tag (Artículo / Webinar), título y una línea de descripción. Los enlaces pueden ser placeholders (`#`) por ahora.

---

## Sección 7 — CONTACTO (`#contacto`)

Dos columnas:

**Izquierda: formulario simple**
- Nombre
- Empresa
- Email
- Teléfono (opcional)
- Mensaje
- Botón "Enviar" (no necesita backend por ahora, puede mostrar mensaje de éxito falso)

**Derecha: datos de las dos oficinas**
Repetir las dos direcciones con teléfono y email de la sección Nosotros.

---

## Footer

- Logo VORA (versión chica) a la izquierda
- Copyright: © 2026 VORA. Todos los derechos reservados.
- Enlaces a Términos y Política de Privacidad (pueden ser `#` placeholder)
- Redes sociales: LinkedIn (ícono, placeholder)

---

## Requisitos de accesibilidad WCAG 2.2 AA (obligatorios)

- Contraste de texto mínimo **4.5:1** para texto normal y **3:1** para texto grande
- **Navegación completa por teclado** (todos los links, botones y campos accesibles con Tab)
- **Textos alternativos** en todas las imágenes, incluyendo el logo (`alt="VORA - logo corporativo"`)
- **Objetivos táctiles** de al menos **44×44 px** en móvil
- **Etiquetas** (`label`) en todos los campos del formulario
- **Landmarks HTML5 semánticos**: `<header>`, `<nav>`, `<main>`, `<section>` con `aria-labelledby`, `<footer>`
- **Skip link** al inicio ("Saltar al contenido principal")
- **Focus visible** en todos los elementos interactivos
- **Estructura de headings correcta**: un solo H1, luego H2 por sección, H3 dentro
- `lang="es"` en el `<html>`
- Metadatos: `<title>` descriptivo, `<meta description>`, Open Graph tags

## Responsive

- **Desktop 1920×1080** y **1366×768**
- **Tablet 768×1024** (ambas orientaciones)
- **Móvil 375×812**

En móvil el menú se colapsa a hamburguesa. Todas las grids pasan a una columna.

## Interacciones

- Scroll suave al hacer click en los links del nav
- Sección activa se resalta en el nav mientras se hace scroll (`IntersectionObserver`)
- Header con leve sombra al hacer scroll
- Hover states sutiles en tarjetas y botones (no animaciones exageradas)
- Sin loaders innecesarios ni animaciones de entrada llamativas

## Lo que NO quiero

- Imágenes de stock de personas sonriendo con laptops
- Gradientes coloridos ni glassmorphism
- Iconos con estilo cartoon
- Animaciones "wow" tipo parallax pesado o partículas flotantes
- Chatbot ni pop-ups
- Cookies banner intrusivo (si es necesario, uno mínimo en la esquina)

---

**Entregable final:** proyecto Next.js listo para hacer `vercel deploy`, con todo el código en un solo repo, imports de shadcn/ui donde apliquen, y el logo en `/public/logo-vora.png`.
