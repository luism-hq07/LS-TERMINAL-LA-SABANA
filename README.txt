TERMINAL DE TRANSPORTE LA SABANA - VERSION MEJORADA
===================================================

ARCHIVOS
- index.html: estructura de la aplicación.
- styles.css: diseño adaptable para computador, tableta y celular.
- app.js: lógica de inicio de sesión, registro, rutas, reservas, despachos, incidencias y administración.
- supabase_schema.sql: plantilla de base de datos para una futura versión multiusuario.

COMO PROBAR LOCALMENTE
1. Descomprime el ZIP.
2. Abre index.html en Chrome o Edge.
3. Acceso administrador: usuario admin / contraseña admin123.
4. Acceso pasajero de demostración: usuario pasajero / contraseña pasajero123.
5. También puedes crear una cuenta desde "Regístrate como pasajero".

FUNCIONES INCLUIDAS
- Inicio de sesión y cierre de sesión.
- Registro de pasajeros con validación de usuario/correo duplicado.
- Roles de pasajero y administrador.
- Consulta de recorridos entre Sincelejo, Corozal, Betulia y Sincé, en ambos sentidos.
- Tarifas y horarios ilustrativos.
- Reservas simuladas y sección "Mis reservas".
- Gestión de despachos, bahías, conductor, placa, fecha y hora.
- Validación para evitar asignar la misma bahía en el mismo horario.
- Registro y seguimiento de incidencias.
- Panel administrativo con usuarios, reservas, incidencias y actividad.
- Activación/desactivación de cuentas registradas.
- Exportación de respaldo JSON y usuarios CSV.
- Registro de actividad.
- Diseño adaptable a móviles.

LIMITACIONES IMPORTANTES
Esta es una versión académica de demostración que funciona con localStorage del navegador.
Por eso:
- Los usuarios, reservas, despachos e incidencias se guardan solo en el navegador y dispositivo donde se crean.
- No existe sincronización entre distintos computadores.
- Las contraseñas se guardan localmente para la demostración; NO se deben usar credenciales reales.
- Los pagos no se procesan, no se emiten tiquetes reales ni códigos QR.
- No hay integración con empresas transportadoras.
- Las tarifas, horarios, disponibilidad y duración son datos ilustrativos que deben validarse.
- No debe utilizarse para operación comercial real ni para almacenar datos personales reales.

PARA PUBLICAR EN GITHUB PAGES
1. En el repositorio, sube index.html, styles.css y app.js a la raíz (o reemplaza los archivos anteriores).
2. Mantén los tres archivos juntos en la misma carpeta.
3. En Settings > Pages, selecciona Deploy from a branch, rama principal y carpeta /(root).
4. Guarda y espera a que GitHub Pages publique el sitio.
5. Recarga el enlace con Ctrl + F5.

BASE DE DATOS CENTRALIZADA
Se incluye supabase_schema.sql como punto de partida para diseñar una futura base de datos.
El archivo SQL NO está conectado a esta versión del frontend. Para que el administrador vea usuarios registrados desde otros dispositivos se necesita:
- Crear un proyecto de Supabase u otro backend.
- Ejecutar y revisar el esquema SQL.
- Configurar autenticación real y políticas de acceso.
- Conectar app.js mediante un cliente seguro y variables públicas del proyecto.
- No guardar contraseñas en tablas propias ni exponer claves secretas en GitHub.

ACCESOS DE DEMOSTRACION
Administrador: admin / admin123
Pasajero de ejemplo: pasajero / pasajero123

Proyecto académico - Terminal de Transporte La Sábana, Sincelejo.
