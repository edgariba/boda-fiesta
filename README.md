# Boda Fiesta: invitación digital de boda informal (demo)

Invitación web de una sola página con estilo **juvenil y relajado**: paleta cálida y suave (crema, terracota, durazno, rosa palo, salvia y verde olivo), con letra a mano, stickers discretos, tarjetas tipo polaroid y sombras suaves. La paleta está en las variables de `:root` al inicio de `index.html`. Todos los datos son ficticios (novios "Mariana & Leo", Rancho La Tortuga, Valle de Bravo, 15 de mayo de 2027).

## Qué incluye

- Pantalla de inicio con foto a pantalla completa, nombres y botón "Abrir invitación": al tocarla sube como cortina, cae confeti y empieza la música
- Portada con foto tipo polaroid, sello giratorio "al fin" y botones a confirmar y al plan
- Cinta animada (marquesina) con nombres, fecha y lugar
- Mensaje informal de los novios y papás de cada uno
- **Rasca la fecha**: tarjeta para rascar con el dedo o el mouse que revela el día (con opción para revelarla sin rascar)
- Cuenta regresiva en vivo y botón "Agendar en mi calendario" (.ics)
- Nuestra historia "en números" con contadores animados
- El plan: ceremonia y fiesta con botón "Cómo llegar" (Google Maps)
- Itinerario divertido (boda, taquiza, brindis, pista, chilaquiles…)
- Banner con frase sobre foto (efecto parallax)
- Menú de taquiza
- Código de vestimenta "arreglado pero cómodo" (tenis permitidos) con colores sugeridos
- Galería tipo polaroid con visor a pantalla completa (deslizar en celular, flechas en escritorio)
- Preguntas frecuentes desplegables (acompañantes, niños, mascota, estacionamiento, hospedaje, lluvia)
- Regalos: fondo de luna de miel con barra de avance y CLABE para copiar, y mesa de regalos
- "Pide tu canción" por WhatsApp
- Pase personalizado y **confirmación por WhatsApp** (asistencia, número de personas, restricción alimentaria y mensaje)
- Hashtag para copiar
- Música alegre tipo ukulele generada en el navegador (sin archivos de audio)

## Personalizar para un cliente

1. Edita el objeto `CONFIG` al final de `index.html`: novios, fecha, número de WhatsApp, pases por defecto y `avanceLunaDeMiel` (porcentaje de la barra).
2. Cambia los textos de cada sección directamente en el HTML (mensaje, papás, historia y números, lugares, itinerario, menú, preguntas, regalos, hashtag).
3. La fecha de "Rasca la fecha" está en el HTML (`.scratch-under`) y en el aviso que aparece al rascar (función `finish` en el módulo `Scratch`).
4. Reemplaza las fotos en `img/` usando los mismos nombres:
   - `portada.jpg`: foto vertical para la polaroid de la portada
   - `historia.jpg`: foto cuadrada para "Nuestra historia"
   - `ceremonia.jpg`, `fiesta.jpg`: encabezados de las tarjetas de "El plan"
   - `banner.jpg`: foto horizontal para la frase
   - `taquiza.jpg`: foto vertical del menú
   - `tenis.jpg`: foto vertical para el código de vestimenta
   - `galeria-1.jpg` … `galeria-6.jpg`
   - `intro.jpg`: foto de la pantalla de inicio (mejor horizontal y grande, con los novios al centro)
   - `og.jpg`: vista previa al compartir en WhatsApp. Al publicar, pon la URL completa en `og:image`.

## Pases personalizados por invitado

Agrega parámetros al enlace:

```
https://tu-dominio.com/?invitado=Familia%20Pérez&pases=3
```

## Usar una canción real

Pon `musica: false` en `CONFIG` y agrega un `<audio>` con tu archivo MP3, o cambia el módulo `Music` para reproducirlo.

## Créditos de las fotos (demo)

Todas las fotos son de [Pexels](https://www.pexels.com/), bajo la [Licencia de Pexels](https://www.pexels.com/license/). Son solo para el demo: en cada invitación vendida, cámbialas por las fotos del cliente.

| Archivo | Foto en Pexels |
|---|---|
| portada.jpg | https://www.pexels.com/photo/18657552/ |
| intro.jpg, og.jpg, galeria-4.jpg | https://www.pexels.com/photo/5085332/ |
| historia.jpg | https://www.pexels.com/photo/7945026/ |
| tenis.jpg | https://www.pexels.com/photo/15587773/ |
| banner.jpg | https://www.pexels.com/photo/6119578/ |
| ceremonia.jpg | https://www.pexels.com/photo/26975888/ |
| fiesta.jpg | https://www.pexels.com/photo/10994595/ |
| taquiza.jpg | https://www.pexels.com/photo/15434318/ |
| galeria-1.jpg | https://www.pexels.com/photo/10360898/ |
| galeria-2.jpg | https://www.pexels.com/photo/15964957/ |
| galeria-3.jpg | https://www.pexels.com/photo/13722217/ |
| galeria-5.jpg | https://www.pexels.com/photo/2735683/ |
| galeria-6.jpg | https://www.pexels.com/photo/15964967/ |
