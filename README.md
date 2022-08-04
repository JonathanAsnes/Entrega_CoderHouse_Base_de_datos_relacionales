# Bases de datos relacionales con NODE
### Asnes Jonathan

## Correr el proyecto localmente
Para correr el proyecto localmente iniciar un servicio de nodemon desde la carpeta source.
`cd .\src\` y `nodemon .\app.js`
Para inicializar las bases de datos se debe correr el comando node `.\src\services\database\migrations\start.js`

## Rutas disponibles:

### Productos
- `/api/productos` GET: Devuelve todos los productos.
- `/api/productos/:idProduct` GET: Devuelve un producto según su id. 
- `/api/productos` POST: Recibe y agrega un producto, y lo devuelve con su id asignando (Solo para admins). Campos requeridos: title, price, thumbnail (archivo de foto), description, code y stock
- `/api/productos/:idProduct` PUT: Recibe y actualiza un producto según su id (Solo para admins).
- `/api/productos/:idProduct` DELETE: Elimina un producto según su id (Solo para admins).