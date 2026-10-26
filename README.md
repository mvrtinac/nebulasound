# NebulaSound

Reproductor retro (estética Winamp / Matrix con robots bailarines) que controla tu música de Spotify desde el iPhone.

La música suena en la app de Spotify; NebulaSound es el control remoto con skin.

## Archivos
- `index.html` — toda la app
- `manifest.webmanifest` — nombre e ícono para la pantalla de inicio
- `icon-180.png`, `icon-192.png`, `icon-512.png` — íconos

## Instalación (una sola vez)
1. **GitHub**: crea el repo `nebulasound` y sube estos archivos (Add file → Upload files).
2. **Vercel**: vercel.com → Add New → Project → importa `nebulasound` → Framework: *Other* → Deploy. Anota la dirección (ej. `https://nebulasound.vercel.app/`).
3. **Spotify**: developer.spotify.com/dashboard → Create app
   - Redirect URI: la dirección de Vercel **con la barra final** (la app te la muestra para copiarla)
   - API: marca **Web API**
   - Guarda y copia el **Client ID**
   - Si al conectar aparece un error de usuario, agrega tu correo en *User Management*.
4. Abre la dirección de Vercel en Safari del iPhone → Compartir → **Agregar a inicio**.
5. Abre NebulaSound desde el ícono, pega el Client ID, toca **Conectar Spotify**.

## Requisitos
- Spotify Premium (exigido por Spotify para controlar la reproducción).
- Solo se muestran playlists tuyas o colaborativas (Spotify no entrega el contenido de playlists ajenas).
- Spotify debe estar abierto o usado hace poco en el iPhone para recibir las órdenes.

## Datos que guarda (solo en tu celular)
- `ns_tok`: sesión de Spotify
- `ns_cfg`: colores, velocidad del baile y última playlist
- `ns_client_id`: tu Client ID
