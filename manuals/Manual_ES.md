# Zoom MultiStomp — Community Effect Pack (8 Custom Effects)
### Manual de Usuario y Referencia Rápida
**Modelos soportados:** Zoom MS-70CDR / MS-50G (Firmware v2.10)  
**Categoría en el pedal:** Todos los efectos aparecen bajo la categoría **Delay**  
**Distribución:** Comunidad Reddit `r/zoommultistomp` & Facebook Groups  

---

## Índice
1. [Guía de Instalación y Primeros Pasos](#1-guía-de-instalación-y-primeros-pasos)
2. [Matriz Rápida / Cheat Sheet de Controles](#2-matriz-rápida--cheat-sheet-de-controles)
3. [Manuales Detallados por Efecto](#3-manuales-detallados-por-efecto)
   - [1. SilverSt — Amplificador Limpio Americano + Cab 2×12](#1-silverst--amplificador-limpio-americano--cab-212)
   - [2. 424mkI — Preamp / Saturador Cassette Vintage](#2-424mki--preamp--saturador-cassette-vintage)
   - [3. Dustbox — Fuzz Motosierra + Sub-Octava Sintética](#3-dustbox--fuzz-motosierra--sub-octava-sintética)
   - [4. Nimbus — Nube Granular Ambiental](#4-nimbus--nube-granular-ambiental)
   - [5. Dustfall — Reverb y Eco de Capas Sucias con Drive y Sag](#5-dustfall--reverb-y-eco-de-capas-sucias-con-drive-y-sag)
   - [6. Shields — Multitap Reverse Early Reflections (Glide Guitar)](#6-shields--multitap-reverse-early-reflections-glide-guitar)
   - [7. Ouroboros (mono) — Eco de Cinta de 3 Cabezas + Reverb de Resorte](#7-ouroboros-mono--eco-de-cinta-de-3-cabezas--reverb-de-resorte)
   - [8. Gatsby — Saturador de Cinta & Through-Zero Doubletracker](#8-gatsby--saturador-de-cinta--through-zero-doubletracker)
4. [Recetas de Cadenas Recomendadas](#4-recetas-de-cadenas-recomendadas)

---

## 1. Guía de Instalación y Primeros Pasos

### ⚠️ Regla de Oro antes de flashear:
**Haz un respaldo completo de tus presets y efectos actuales** antes de instalar cualquier archivo `.ZDL`. Puedes usar herramientas de la comunidad como *Zoom Effect Manager (ZEM)* o *Zoom Firmware Editor*.

### ¿Por qué están todos en la categoría Delay?
En la arquitectura del firmware Zoom ZDL, la categoría **Delay** (Group ID 8) ofrece la mayor estabilidad de memoria para efectos con buffers dedicados y potenciómetros extendidos (knobs 4 al 9). Aunque un efecto sea un amplificador (`SilverSt`), un previo/fuzz (`424mkI`, `Dustbox`) o una reverb (`Dustfall`), **siempre los encontrarás en la lista del pedal dentro del grupo DELAY**.

### Lista de archivos binarios incluidos:
1. `SilverSt.ZDL` &mdash; Amplificador limpio americano + caja 2×12 estéreo.
2. `424mkI.ZDL` &mdash; Preamplificador y distorsión de casetera analógica vintage.
3. `Dustbox.ZDL` &mdash; Fuzz motosierra con sub-octava cuadrada sintética a -2 octavas.
4. `Nimbus.ZDL` &mdash; Nube granular ambiental de 6 voces con escaneo y congelamiento.
5. `Dustfall.ZDL` &mdash; Reverb estéreo de capas sucias con saturación (Drive) y corte de voltaje (Sag).
6. `Shields.ZDL` &mdash; Multitap reverse de 19 reflexiones tempranas invertidas para shoegaze.
7. `Uroboros.ZDL` &mdash; Eco de cinta clásico de 3 cabezas con inercia de motor y reverb de resorte.
8. `Gatsby.ZDL` &mdash; Saturador de cinta y doubletracker through-zero flanger.

---

## 2. Matriz Rápida / Cheat Sheet de Controles

| Efecto | Inspiración Sonora | Rol en la Cadena | Knobs en Pantalla | Carácter de Salida |
|---|---|---|---|---|
| **SilverSt** | Fender Silverface + 2×12 | Amp Limpio + Cab | `Gain`, `Width`, `Level`, `Bass`, `Middl`, `Trebl`, `Reson`, `Prese`, `Mic` | Estéreo / Cab activo |
| **424mkI** | Tascam Portastudio 424 | Cassette Preamp / Fuzz | `Trim`, `Chan`, `Mstr`, `Bass`, `Trebl`, `Level` | Saturación analógica |
| **Dustbox** | DOD FX33 Buzz Box | Fuzz Caótico + Sub-Octava | `Dust`, `Motor`, `Filter`, `Power` | Sub-octava a -2 octavas |
| **Nimbus** | Granular Cloud Synthesis | Colchón Ambiental / Drones | `Size`, `Pitch`, `Dens`, `Mix`, `Freeze`, `Tone`, `Speed`, `Wah` | Búfer ~3s / 6 voces |
| **Dustfall** | Dirty Ambient Reverb | Reverb Rota / Colas Sucias | `Mode`, `Decay`, `Level`, `Drive`, `Sag`, `Mix`, `Amp`, `Volume` | Capa base + Drive/Sag |
| **Shields** | Yamaha SPX90 (Reverse Gate) | Glide Guitar / Shoegaze | `Size`, `Live`, `PreDly`, `Tone`, `Mix` | ¡Usar ANTES del drive! |
| **Ouroboros** | Roland RE-201 Space Echo | Eco de Cinta Multi-Cabeza | `Mode` (1-12), `Repeat`, `Intens`, `EchoVol`, `RevVol`, `Bass`, `Treble`, `Sat`, `Mix` | Inercia de motor real |
| **Gatsby** | Strymon Deco V2 | Saturador + Doubletracker | `Sat`, `Voice`, `Tone`, `Level`, `Lag`, `Blend`, `Wobble`, `Type`, `Mix` | Through-Zero (−0.3 ms) |

---

## 3. Manuales Detallados por Efecto

---

### 1. SilverSt — Amplificador Limpio Americano + Cab 2×12

#### Concepto y Carácter Sonoro
Inspirado en el clásico amplificador americano de sonido limpio a válvulas (estilo Fender Silverface Twin/Deluxe) combinado con una pantalla acústica abierta 2×12. Su sonido destaca por unos graves sólidos y con cuerpo, un corte natural en medios y un brillo campaneante (*chime*) en frecuencias altas. Incorpora emulación de dos posiciones de microfonía acústica: **Center** (definido y brillante) y **Edge** (cálido y fuera de eje).

> **Ubicación recomendada:** Colócalo al **final de tu cadena** en el pedal y envía las salidas L/R directamente a tu interfaz de grabación, consola de sonido o monitor FRFR. Su simulación de pantalla está siempre activa.

#### Controles
- **Gain (0–100):** Desde limpio de gran techo dinámico hasta una saturación sutil en el punto de ruptura (*edge-of-breakup*).
- **Bass, Middl, Trebl (0–100):** Ecualización tonal activa de 3 bandas.
- **Reson (0–100):** Regula la amortiguación de baja frecuencia entre la etapa de potencia y el cono (respuesta de pegada en graves).
- **Prese (0–100):** Ataque de medios-altos previo a la pantalla.
- **Mic (0–100):** Posición del micrófono (0 = centro del cono, brillante; 100 = borde/fuera de eje, cálido y redondo).
- **Width (0–100):** Desfase estéreo entre los dos micrófonos virtuales, conservando una suma a mono perfecta.
- **Level (0–100):** Volumen máster de salida.

#### Presets Recomendados
| Preset | Gain | Width | Level | Bass | Middl | Trebl | Reson | Prese | Mic |
|---|---|---|---|---|---|---|---|---|---|
| **Pedal Platform** | 25 | 30 | 60 | 50 | 50 | 50 | 45 | 50 | 35 |
| **Glass Clean** | 12 | 20 | 62 | 42 | 43 | 64 | 30 | 65 | 18 |
| **Warm Edge of Breakup**| 72 | 22 | 48 | 58 | 58 | 38 | 62 | 38 | 72 |
| **Big Studio Clean** | 35 | 40 | 56 | 62 | 38 | 54 | 68 | 55 | 32 |

---

### 2. 424mkI — Preamp / Saturador Cassette Vintage

#### Concepto y Carácter Sonoro
Inspirado en la sección de preamplificación y saturación analógica de las legendarias caseteras multipista Tascam Portastudio de los años 80 y 90. En ajustes moderados proporciona el grano, calidez y compresión musical de una cinta analógica; al llevarlo a ajustes extremos satura progresivamente hasta convertirse en un fuzz de consola lo-fi crujiente y agresivo.

#### Controles
- **Trim (0–100):** Ganancia de entrada analógica.
- **Chan (0–100):** Nivel del canal. Subirlo engrosa el tono y eleva la saturación armónica.
- **Mstr (0–100):** Nivel máster previo a las etapas de recorte de salida.
- **Bass & Trebl (0–100):** Ecualización tonal de la consola (50 = posición neutra).
- **Level (0–100):** Volumen de salida post-recorte.

#### Presets Recomendados
| Preset | Trim | Chan | Mstr | Bass | Trebl | Level |
|---|---|---|---|---|---|---|
| **Calor de Cinta (Default)** | 50 | 85 | 85 | 50 | 50 | 35 |
| **Fuzz de Consola al Límite** | 100 | 100 | 100 | 50 | 50 | 25 |
| **Preamp Limpio Cálido** | 20 | 85 | 85 | 50 | 50 | 35 |
| **Crunch Indie Rock** | 80 | 90 | 90 | 50 | 50 | 25 |

---

### 3. Dustbox — Fuzz Motosierra + Sub-Octava Sintética

#### Concepto y Carácter Sonoro
Inspirado en el mítico pedal de culto DOD FX33 Buzz Box. Fusiona una distorsión abrasiva y motosierra con un divisor de sub-octava cuadrada sintética a **-2 octavas**. El resultado es una pared sónica destructiva y caótica ideal para sludge, grunge y riffs graves experimentales.

> **Controles (Temática de aspiradora industrial):** Dust (mezcla de octava), Motor (ganancia de distorsión), Filter (tono) y Power (volumen máster).

#### Controles
- **Dust (0–100):** Mezcla entre la distorsión pura (0) y la sub-octava cuadrada a -2 octavas (100). En 0 no hay sub-octava.
- **Motor (0–100):** Ganancia de la distorsión. Al aumentarlo, el divisor de octava se vuelve más reactivo e inestable.
- **Filter (0–100):** Control de tono de la distorsión (0 = oscuro/opaco, 50 = plano, 100 = brillante/cortante). No filtra la sub-octava.
- **Power (0–100):** Volumen de salida general.

#### Presets Recomendados
| Preset | Dust | Motor | Filter | Power |
|---|---|---|---|---|
| **Classic Buzz Box Sludge** | 50 | 60 | 50 | 25 |
| **Pure Chainsaw Fuzz** (Sin Octava) | 0 | 75 | 65 | 25 |
| **Sub-Bass Glitch Drone** | 90 | 40 | 30 | 30 |

---

### 4. Nimbus — Nube Granular Ambiental

#### Concepto y Carácter Sonoro
Inspirado en la síntesis granular ambiental (arquetipo Mutable Instruments Clouds / Chase Bliss Mood). Nimbus graba continuamente tu señal en un búfer circular de ~3 segundos. Hasta **6 voces granulares simultáneas** leen fragmentos aleatorios con envolventes parabólicas suaves, pasándolos por filtros resonantes y una red de difusión estéreo para crear desde sutiles texturas hasta colchones orquestales etéreos.

#### Controles
- **Size (0–100):** Duración de los granos (~40 ms para texturas glitch/stutter hasta ~400 ms para un mar ambiental continuo).
- **Pitch (0–100):** Tono de los granos (0 = -1 octava, 50 = unísono, 100 = +1 octava shimmer).
- **Dens (0–100):** Cantidad de voces activas (1 a 6) y densidad de disparo temporal.
- **Mix (0–100):** Balance dry/wet (prueba con valores de 60 a 80 para evaluar cambios tímbricos en la nube).
- **Freeze (0–100):** Valores ≥50 congelan el búfer actual (~2.97 s) de forma infinita, permitiéndote solear o tocar en seco por encima.
- **Tone (0–100):** Filtro tonal por voz (~180 Hz a 5 kHz).
- **Speed (0–100):** Velocidad del cabezal de escaneo (75 = 1.0x normal, 50 = estático, <50 = reversa).
- **Wah (0–100):** Macro interactivo que conecta resonancia y seguidor de envolvente (auto-wah orgánico reactivo al ataque de la púa).

#### Presets Recomendados
| Preset | Size | Pitch | Dens | Mix | Freeze | Tone | Speed | Wah |
|---|---|---|---|---|---|---|---|---|
| **Ambient Dream Cloud** | 55 | 50 | 60 | 60 | 0 | 75 | 75 | 0 |
| **Shimmer Wash (+1 Oct)** | 70 | 100 | 75 | 50 | 0 | 65 | 75 | 15 |
| **Sub-Atmosphere Drone** | 85 | 0 | 80 | 70 | 55 | 45 | 50 | 0 |
| **Reverse Glitch Scatter** | 25 | 50 | 50 | 50 | 0 | 80 | 25 | 40 |

---

### 5. Dustfall — Reverb y Eco de Capas Sucias con Drive y Sag

#### Concepto y Carácter Sonoro
Dustfall es un procesador de ambiente diseñado para crear muros sonoros shoegaze, colas que se desmoronan y niebla lo-fi. Su arquitectura divide la señal en dos capas paralelas: una señal base con reverb larga y una segunda capa que puede saturarse (**Drive**) y quedarse sin alimentación de corriente (**Sag**), pasando finalmente por un previo de salida (**Amp**).

> **La fórmula de Dustfall:** `Level` crea el material base; `Drive` y `Sag` lo rompen; `Mix` regula cuánta rotura escuchas; `Amp` colorea el resultado final.

#### Controles
- **Mode:** Familia de ambiente: **Hall** (0–32, amplio y oscuro), **Spring** (33–66, metálico y resonante) o **BBD** (67–100, eco analógico lo-fi).
- **Decay (0–100):** Longitud de la cola o repeticiones del eco.
- **Level (0–100):** Mezcla seco/ambiente de la capa base.
- **Drive (0–100):** Ganancia y saturación de la capa paralela.
- **Sag (0–100):** Efecto de batería agotada (*voltage starvation*) que corta la cola en fragmentos crujientes.
- **Mix (0–100):** Mezcla entre la capa base limpia y la capa saturada/rota.
- **Amp:** Selector de previo: **Neutral** (limpio), **Murk** (oscuro y con cuerpo) u **Open** (brillante y agresivo).
- **Volume (0–100):** Volumen máster de salida.

#### Presets Recomendados
| Preset | Mode | Decay | Level | Drive | Sag | Mix | Amp | Volume |
|---|---|---|---|---|---|---|---|---|
| **Niebla Shoegaze** | Hall | 65 | 50 | 40 | 35 | 60 | Murk | 35 |
| **Broken Spring** | Spring | 70 | 60 | 65 | 55 | 50 | Open | 30 |
| **Cinta Degradada** | BBD | 50 | 50 | 30 | 20 | 45 | Neutral | 50 |

---

### 6. Shields — Multitap Reverse Early Reflections (Glide Guitar)

#### Concepto y Carácter Sonoro
Inspirado en el célebre algoritmo Early Reflections ER2 "Reverse Gate" del procesador de rack Yamaha SPX90. Es el pilar fundamental detrás del sonido de guitarra elástica (*glide guitar*) de Kevin Shields en el legendario álbum *Loveless* de My Bloody Valentine.

No es una reverb tradicional con cola infinita: es un patrón de **19 reflexiones tempranas invertidas con ganancia ascendente** que imita el efecto de una cinta reproduciéndose al revés.

> **⚠️ POSICIÓN CRÍTICA EN LA CADENA:** Shields **DEBE colocarse ANTES de tus pedales de distorsión, fuzz o previo saturado**. Al golpear una etapa de ganancia con esta envolvente ascendente, se genera el clásico muro envolvente y elástico de MBV.

#### Controles
- **Size (0–100):** Expande o contrae la separación temporal entre las 19 reflexiones (de 30 ms a 420 ms). En 100 proporciona la duración extendida clásica de MBV.
- **Live (0–10):** Regula la absorción y presencia de las reflexiones posteriores (5 = preset original de fábrica; 7 = curva optimizada MBV; 10 = mayor densidad).
- **PreDly (0–100 ms):** Retardo previo al inicio de las reflexiones (0 ms para que el efecto arranque inmediatamente con la púa).
- **Tone (0–100):** Filtro pasabajos tonal (100 = conserva el filtrado natural de 12 kHz de los convertidores de rack clásicos).
- **Mix (0–100):** Balance dry/wet (100% wet por defecto para alimentar directamente las etapas de ganancia).

#### Presets Recomendados
| Preset | Size | Live | PreDly | Tone | Mix | Cadena recomendada |
|---|---|---|---|---|---|---|
| **MBV Loveless (Default)** | 100 | 7 | 0 | 100 | 100 | `Shields` &rarr; Fuzz/Distorsión &rarr; Amp |
| **SPX90 Factory Preset 17** | 16 | 5 | 25 | 100 | 100 | `Shields` &rarr; Overdrive suave |
| **Subtle Glide Layer** | 70 | 6 | 10 | 60 | 50 | Textura paralela en limpio |

---

### 7. Ouroboros (mono) — Eco de Cinta de 3 Cabezas + Reverb de Resorte

#### Concepto y Carácter Sonoro
Inspirado en el mítico Roland RE-201 Space Echo (1974). En la pantalla del pedal aparece con el nombre **`Uroboros`**.

Ouroboros emula la física de una **cinta analógica en bucle sin fin** pasando por tres cabezas de reproducción simultáneas a distancias fijas, impulsada por un motor electromecánico de velocidad variable. Mover la perilla `Repeat` altera la velocidad del motor, produciendo el auténtico arrastre de tono (*glissando*) con inercia física, saturación de cinta y una reverberación de resortes integrada en paralelo.

#### Controles
- **Mode (1–12):** Selector de los 12 modos clásicos:
  - *Modos 1 a 4:* Solo eco de cinta (cabeza 1, 2, 3 o combinaciones).
  - *Modos 5 a 11:* Combinaciones rítmicas de cabezas + tanque de reverb de resorte.
  - *Modo 12:* Solo reverb de resortes (Spring).
- **Repeat (0–100):** Velocidad del motor (cambia el tiempo arrastrando el tono con inercia física real).
- **Intens (0–100):** Realimentación / Feedback (subir para autooscilación infinita musical).
- **EchoVol (0–100):** Nivel del eco de cinta.
- **RevVol (0–100):** Nivel del tanque de resortes.
- **Bass & Treble (0–100):** Ecualización de las repeticiones (50 = plano).
- **Sat (0–100):** Saturación del previo de grabación de cinta.
- **Mix (0–100):** Mezcla general entre señal seca y efecto.

#### Presets Recomendados
| Preset | Mode | Repeat | Intens | EchoVol | RevVol | Sat | Mix |
|---|---|---|---|---|---|---|---|
| **Dub Chamber (King Tubby)** | 7 (Cabezas 2+3 + Rev) | 45 | 70 | 65 | 40 | 40 | 50 |
| **Rockabilly Slapback** | 1 (Cabeza 1 sola) | 85 | 15 | 55 | 0 | 25 | 40 |
| **Infinite Space Oscillation** | 2 o 4 | 30 | 85 | 75 | 20 | 60 | 50 |

---

### 8. Gatsby — Saturador de Cinta & Through-Zero Doubletracker

#### Concepto y Carácter Sonoro
Inspirado en los efectos de estudio clásicos de saturación de cinta y doubletracker (estilo Strymon Deco). Gatsby reúne la calidez y compresión de un previo de cinta con dos reproductores (*Reference Deck* y *Lag Deck*). Su tiempo de desfase arranca en **-0.3 ms**, permitiendo el auténtico **Through-Zero Flanging (TZF)**: el retardo cruza el punto cero absoluto produciendo la cancelación nula total y el clásico sonido de "chorro de avión" (*jet sweep*) de cinta.

#### Controles
- **Sat (0–100):** Ganancia del saturador de cinta (de calidez armónica transparente a compresión marcada).
- **Voice:** Tipo de cinta: **Classic** (0–49, carrete abierto de estudio) o **Cassette** (50–100, compresión de casete con pegada en graves).
- **Tone (0–100):** Tonalidad del bloque saturador (50 = neutro).
- **Level (0–100):** Compensación de volumen de salida del saturador (50 = ganancia unitaria).
- **Lag (0–100):** Desfase temporal entre reproductores (-0.3 ms a 500 ms).
- **Blend (0–100):** Balance entre la toma original y la toma desfasada (50 = mezcla 50/50, óptima para cancelaciones TZF).
- **Wobble (0–100):** Modulación de cinta (wow & flutter aleatorio).
- **Type:** Interacción de fase: **Sum** (0–25), **Invert** (26–50), **Bounce** (51–75, ping-pong estéreo) y **Auto-Sweep** (76–100).
- **Mix (0–100):** Mezcla dry/wet global.

#### Presets Recomendados
| Preset | Sat | Voice | Tone | Lag | Blend | Wobble | Type | Mix |
|---|---|---|---|---|---|---|---|---|
| **Through-Zero Jet Flange** | 35 | Classic | 50 | 15 | 50 | 20 | Sum | 100 |
| **Stereo Doubler (Dimension)** | 25 | Classic | 50 | 45 | 50 | 35 | Bounce | 100 |
| **Cassette Preamp Warmth** | 65 | Cassette | 45 | 0 | 0 | 0 | Sum | 100 |
| **Slapback de Cinta Vintage** | 40 | Classic | 50 | 75 | 50 | 15 | Sum | 100 |

---

## 4. Recetas de Cadenas Recomendadas

¡Aprovecha los 6 slots simultáneos del Zoom MultiStomp combinando estos efectos!

### Receta 1: El Sonido Definitivo Shoegaze / Dream Pop
```
[Guitarra] ──► Shields (100% Wet) ──► 424mkI (Fuzz/Preamp) ──► Nimbus (Granular Cloud) ──► SilverSt (Amp + Cab) ──► [Salida Estéreo]
```
*Las reflexiones tempranas invertidas de Shields golpean el previo 424mkI, mientras Nimbus sostiene una bruma detrás y SilverSt da el timbre y caja final.*

### Receta 2: Dub & Ambient Lo-Fi
```
[Guitarra/Sintetizador] ──► Gatsby (Saturador de Cinta) ──► Uroboros (RE-201) ──► Dustfall (Reverb Sucia) ──► [Salida Estéreo]
```
*El doubletracker añade ensanchamiento analógico, Ouroboros entrega ecos con inercia física y Dustfall envuelve las repeticiones en una cola rota.*

### Receta 3: Sludge / Glitch Caótico
```
[Bajo o Guitarra] ──► Dustbox (Buzz Box Fuzz) ──► Nimbus (Freeze activado ≥ 60) ──► SilverSt (Amp Limpio) ──► [Salida]
```
*Riffs con motosierra y sub-graves de -2 octavas congelados en nubes granulares vivas.*

---
*Manual preparado con cariño para la comunidad de Zoom MultiStomp.*
