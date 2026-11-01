# Jaya Player — guía de uso

Jaya Player es un reproductor IPTV para Android TV, TV boxes y smartphones.
La aplicación **no ofrece canales de TV ni contenido**: solo reproduce las listas que añade el propio usuario.

---

## 1. Instalación

1. Descargue la aplicación: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (siempre la última versión) o desde la página [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest).
2. En un TV box es cómodo usar la app **Downloader** o una memoria USB.
3. En la primera instalación Android pedirá permitir instalar desde esta fuente — permítalo.
4. Se requiere Android 6.0 o superior.

Después, la aplicación descarga e instala las actualizaciones **por sí misma** (ver sección 10).

---

## 2. Primer inicio y lista

En el primer inicio se abren los **Ajustes**.

1. Pulse **Listas → Añadir**.
2. Elija el tipo:
   - **enlace M3U** — dirección de la lista de su proveedor;
   - **Xtream Codes** — dirección del servidor, usuario y contraseña;
   - **archivo** — lista `.m3u` del dispositivo o de una memoria USB.
3. **EPG** (guía de programación) — dirección XMLTV. Normalmente ya está incluida en la lista del proveedor y el campo puede quedar vacío. Si no aparece la guía, pida la dirección EPG a su proveedor y escríbala aquí.
4. **Actualizar cada … h** — con qué frecuencia actualizar la lista y la guía.
5. Pulse **Guardar**. La carga se hace en segundo plano — puede volver a ver la TV enseguida.

Puede añadir varias listas. Si una actualización falla (por ejemplo, sin internet), la aplicación la repite sola en el siguiente inicio.

---

## 3. Mando a distancia

| Botón | Acción |
|---|---|
| ▲ ▼ | canal anterior / siguiente |
| ◀ | lista de canales |
| ◀ ◀ (más a la izquierda) | lista de grupos |
| ▶ | Favoritos |
| ▶ ▶ (dos veces rápido) | estadísticas del flujo (sí/no) |
| OK | panel de información |
| OK otra vez | pausa |
| OK en pausa | continuar |
| OK largo | menú de acciones (audio, subtítulos, formato, ajustes) |
| números | ir al canal por número |
| 0 | canal anterior |
| Atrás dos veces | salir |

**En la lista de canales:**
- ▶ — guía del canal seleccionado;
- OK largo — modo de marcado: ◀ añadir/quitar de Favoritos, ▶ eliminar canal (los eliminados se recuperan en el grupo «Eliminados»).

**En el smartphone:** toque — pausa y panel de información; deslizar arriba — panel, abajo — ocultarlo; deslizar a la derecha en la mitad izquierda — lista de canales; a la izquierda en la mitad derecha — Favoritos; toque largo — ajustes.

---

## 4. Guía y archivo

- La guía se guarda **24 horas hacia atrás y 36 horas hacia adelante**.
- Pulse ▶ en la lista de canales para abrir la guía. Los programas pasados se pueden ver desde el **archivo** si su proveedor lo admite.
- En el archivo: **OK** — barra de avance, ◀ ▶ — paso (se acelera al mantener), **Atrás** — volver al directo.

---

## 5. Pausa del directo (Timeshift)

**Ajustes → Reproducción → Pausa en directo con grabación.**

- **Desactivada:** la pausa detiene la imagen; al continuar se vuelve al directo.
- **Activada:** tras la pausa se continúa **desde el mismo momento**. El retraso respecto al directo se ve abajo; **Atrás** — volver al directo.

**Almacenamiento de la pausa:**
- **Memoria interna** — la grabación empieza al pausar y se borra al cambiar de canal.
- **Disco externo (USB)** — se graba todo el tiempo mientras ve un canal, por eso **en pausa ◀ ▶ rebobinan** (hasta donde alcance el espacio). La aplicación crea la carpeta `Timeshift` en el disco y usa como máximo el 80 % del espacio libre; las grabaciones antiguas se borran solas.

Memoria USB: FAT32 o exFAT (NTFS si su dispositivo lo admite).
No se admiten flujos DASH, flujos cifrados ni flujos con pista de audio separada — en ellos la pausa funciona de forma normal.

---

## 6. Grupos ocultos (control parental)

1. Abra la lista de grupos (◀ ◀), elija un grupo y **mantenga OK** — se activa la selección de grupos.
2. Marque los grupos con OK y pulse **Atrás**.
3. Introduzca la contraseña con las flechas y pulse OK. La contraseña predeterminada es **▶ ▶ ▶ ▶**.
4. Tras la primera ocultación, la aplicación le propondrá crear su propia contraseña de flechas (p. ej. ▲ ▲ ◀ ▶) — recuérdela.

Para volver a mostrar los grupos ocultos, en la lista de grupos **pulse ◀ tres veces rápido** e introduzca la contraseña. Al minimizar la aplicación los grupos se ocultan de nuevo.

---

## 7. Imagen en imagen y segundo plano (smartphone)

- **Imagen en imagen:** al ir a la pantalla de inicio, el vídeo sigue en una ventana pequeña.
- **Audio en segundo plano:** el audio sigue con la pantalla bloqueada; se controla desde la barra de notificaciones.

---

## 8. Ajustes

- **Pantalla:** frecuencia de imagen automática, 120 Hz, duración del panel de información, desplazamiento de listas, **pantalla OLED** (protección contra quemado: desplazamiento de elementos, reloj oculto, salvapantallas en pausa, atenuación de menús).
- **Reloj:** posición en pantalla.
- **Reproducción:** imagen en imagen, audio en segundo plano, nivelación de volumen, estadísticas, pausa del directo, precarga de canales vecinos, búfer, User-Agent.
- **Temas** (botón aparte «Temas» en los ajustes): temas listos (Clásico, Negro OLED, Océano, Cálido, Cristal) o colores propios de paneles, selección, texto, panel de información, reloj y transparencia.
- **Administración:** contraseña y bloqueo de opciones (las opciones bloqueadas se ocultan).

**User-Agent** es cómo el reproductor se «presenta» ante el servidor del proveedor. Si la lista carga pero los canales no se abren, pruebe **VLC**.

---

## 9. Copia de seguridad

**Ajustes → Acerca de → Exportar** guarda listas, Favoritos, grupos ocultos y ajustes en un archivo. **Importar** los restaura — por ejemplo, en un dispositivo nuevo.

---

## 10. Actualizaciones

- La aplicación busca, descarga e instala las actualizaciones sola (se puede desactivar en **Acerca de**).
- Antes de instalar se comprueba la firma — no se puede falsificar una actualización.
- Si la aplicación no pudo buscar actualizaciones durante **90 días**, se activa un modo restringido (sin guía ni archivo, 5 canales en Favoritos). Basta con conectarse a internet — todo vuelve.

---

## 11. Versión Pro

Ahora todas las funciones son **gratuitas**. Cuando llegue Pro, todos tendrán **3 meses** más de acceso completo.

| | Gratis | Pro |
|---|---|---|
| Calidad | hasta 1080p (4K/HDR — 3 minutos) | 4K, HDR |
| Favoritos | 20 canales | sin límite |
| Grupos ocultos | 1 | sin límite |
| Archivo | últimas 3 horas | lo que ofrezca el proveedor |
| Nivelación de volumen, frecuencia automática, 120 Hz, AC3/DTS al receptor | — | ✓ |
| Pausa en directo con grabación, temas | — | ✓ |
| Imagen en imagen y audio en segundo plano (smartphone) | — | ✓ |

---

## 12. Solución de problemas

- **Un canal no se abre** — cambie el User-Agent (VLC); pruebe la lista en otro dispositivo.
- **No hay guía** — revise la dirección EPG de la lista; abra **Listas** — allí se ve el error de carga.
- **Audio con chasquidos en el smartphone con nivelación** — desactive la nivelación.
- **4K va a saltos en un TV box débil** — elija el búfer «Grande» o vea en HD.

---

© 2026 Ruslan G. Todos los derechos reservados.
