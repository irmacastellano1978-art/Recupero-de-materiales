# Recupero de Materiales — versión técnicos

Esta versión está preparada para Netlify y funciona como PWA.

## Incluye
- Login de técnico/administrador (modo demo).
- Alta de recuperos.
- Foto desde cámara del teléfono.
- GPS.
- Cálculo de comisión.
- Estado y devolución a depósito.
- Búsqueda y filtros.
- Dashboard administrativo.
- Exportación CSV compatible con Excel.
- Trabajo local/offline y sincronización cuando vuelve la conexión.
- Netlify Function + Netlify Blobs como almacenamiento.

## Demo
- tecnico / 1234
- admin / 1234

## Publicación
1. Subir el proyecto a un repositorio GitHub.
2. Crear un nuevo sitio en Netlify desde ese repositorio.
3. Netlify detectará `netlify.toml`.
4. La Function usa Netlify Blobs; una vez desplegado, la función guarda los registros en el store `recupero-materiales`.

## Importante antes de producción
Los usuarios/PIN del demo están dentro del frontend y NO deben usarse como seguridad real. Para producción conviene integrar autenticación real (por ejemplo Netlify Identity/JWT o un proveedor externo) y proteger la Function.
