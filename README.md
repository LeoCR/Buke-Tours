# Buke Tours
E-commerce de venta de Tours Vacacionales

### Como Instalar el Proyecto
1. Instalar XAMPP. Para ello ir a [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html) Descargarlo e Instalalrlo.
2. En la Carpeta htdocs del xampp clonar este Repositorio: [https://github.com/LeoCR/Buke-Tours.git](https://github.com/LeoCR/Buke-Tours.git)
3.Abrir el Mysql del Xampp o cualquier otra instancia local de Mysql como por ejemplo Workbench y crear una nueva base de datos llamada: `buke_tours_db`
4. Luego ejecutar en Mysql el Script que viene en la carpeta `/sql/ddl.sql` de este repositorio.
5. Cambiar el password de la configuracion en el archivo que viene en la carpeta `/php/config/db.php` en la Linea 15, cambiarlo por su password de la Base datos
6. Si todo salio bien deberias poder abrir en tu navegador estas URL's: [http://localhost/Buke-Tours/admin/auth/login/](http://localhost/Buke-Tours/admin/auth/login/) y [http://localhost/Buke-Tours/](http://localhost/Buke-Tours/)
7. El usuario administrador es: 
Usuario Admin: juan.perez@example.com
Password Admin: AeiB#12$34!u

## 🔍 Funcionalidades principales
### 🧭 Búsqueda de tours

Permite filtrar tours según título, ubicación o descripción.

Utiliza la función normalizeString() para buscar sin acentos ni mayúsculas.

Los resultados se renderizan dinámicamente en el contenedor #search-result o #search-tours-results.

### 🛒 Carrito de compras

Administrado desde cart.module.js.

El usuario puede agregar tours desde cualquier vista (index o tours).

Se almacena en localStorage para mantener persistencia entre páginas.

### 💳 Checkout

Validación de formulario con alertas visuales usando Bootstrap.

Cálculo del subtotal y total dinámicamente según los ítems seleccionados.


### 💡 Tecnologías utilizadas

HTML5 / Bootstrap 5.3 / JavaScript (ES6+) /SweetAlert2 / Fetch API 
