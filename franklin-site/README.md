# Franklin Zeas Real Estate — sitio web con blog editable

## Qué es esto
Tu página web (inicio, propiedades, financiamiento, sobre mí, contacto) + un
blog con URLs propias (franklinzeas.com/blog/tu-articulo/) que vas a poder
escribir tú mismo desde un panel privado, con subida de fotos incluida —
sin tocar código.

## Cómo publicarla (una sola vez, ~15 minutos)

**1. Crea una cuenta gratis en GitHub** (github.com) si no tienes una.

**2. Sube esta carpeta a un repositorio nuevo en GitHub.**
   - Más fácil: en github.com, "New repository" → arrastra todos estos
     archivos y carpetas a la web de GitHub (acepta arrastrar y soltar).

**3. Crea una cuenta gratis en Netlify** (netlify.com) y elige
   "Add new site" → "Import an existing project" → conecta tu cuenta de
   GitHub → selecciona el repositorio que acabas de subir.
   - Netlify va a detectar automáticamente el archivo `netlify.toml` y
     construir el sitio solo. En un par de minutos tendrás una URL como
     `algo-al-azar.netlify.app` ya funcionando.

**4. Activa el panel de blog (Netlify Identity + Git Gateway):**
   - Dentro de tu sitio en Netlify: pestaña **Identity** → "Enable Identity".
   - En Identity → **Settings and usage** → **Registration**: déjalo en
     "Invite only" (así solo tú puedes entrar).
   - Baja a **Services** → **Git Gateway** → "Enable Git Gateway".
   - En la pestaña Identity, botón **Invite users** → escribe tu correo.
     Te va a llegar un email para crear tu contraseña.

**5. (Opcional pero recomendado) Conecta tu dominio propio**, por ejemplo
   `franklinzeasrealestate.com`, desde Netlify → Domain settings. Si no
   tienes uno, lo compras en Namecheap o NIC.ec (~$12–15/año).

## Cómo escribir un blog nuevo (desde ese momento en adelante)
1. Ve a `tu-sitio.netlify.app/admin/` (o `tudominio.com/admin/`).
2. Inicia sesión con el correo que invitaste.
3. Clic en "Blog" → "New Blog" → escribe título, categoría, resumen,
   sube la foto de portada y escribe el contenido.
4. Clic en "Publish". En 1–2 minutos tu artículo ya está en línea en
   `tu-sitio.com/blog/tu-articulo/`.

Así de simple, cada vez — no necesitas volver a pedirme ayuda con código
para publicar, solo para cambios de diseño o secciones nuevas.

## Antes de publicar, revisa
- `src/index.njk`: al final tiene el arreglo `properties` — reemplázalo
  con tus propiedades reales cuando las tengas listas.
- El WhatsApp ya está puesto (0969851813).
- Instagram: `@franklinzeas.realtor` (cámbialo si es distinto).

## Desarrollo local (si algún día quieres ver cambios antes de publicar)
```
npm install
npm start
```
Abre `http://localhost:8080`.
