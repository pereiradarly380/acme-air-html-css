# ACME AIR

## Descripción

**ACME AIR** es una aplicación web para una aerolínea, desarrollada como proyecto académico utilizando **HTML5 y CSS3**.

El proyecto permite simular diferentes procesos relacionados con los vuelos, como el registro de usuarios, inicio de sesión, búsqueda de vuelos, consulta de vuelos disponibles, check-in y consulta de vuelos reservados.

La interfaz fue diseñada para ser **responsive**, permitiendo visualizar correctamente el contenido en computadores, tablets y dispositivos móviles.

---

## Objetivo del proyecto

Desarrollar una interfaz web moderna, organizada y responsive para una aerolínea, aplicando conocimientos de:

* HTML5
* CSS3
* Diseño responsive
* Formularios
* Navegación entre páginas
* Estructura semántica
* Organización de archivos
* Diseño de interfaces de usuario

---

## Funcionalidades

El proyecto cuenta con las siguientes vistas:

### Inicio de sesión

Permite al usuario ingresar a la aplicación mediante:

* Usuario o correo electrónico
* Contraseña
* Acceso al menú principal
* Acceso al registro
* Recuperación de contraseña

**Archivo:** `index.html`

[Vista previa](img/cap.png)

---

### Registro

Permite registrar los datos básicos del usuario:

* Nombre completo
* Número de identificación
* E-mail
* Teléfono
* Ciudad

Al guardar la información, el usuario es dirigido a la creación de contraseña.

**Archivo:** `registro.html`

[Vista previa](img/cap.png)

---

### Crear contraseña

Permite establecer una contraseña para completar el proceso de registro.

**Archivo:** `crear-contraseña.html`

[Vista previa](img/cap.png)

---

### Menú principal

Es la pantalla principal de navegación de ACME AIR.

Desde esta vista el usuario puede acceder a:

* Buscar vuelos
* Check-in
* Mis vuelos
* Cerrar sesión

**Archivo:** `menu.html`

[Vista previa](img/cap.png)

---

### Buscar vuelos

Permite seleccionar:

* Ciudad de origen
* Ciudad de destino
* Fecha de salida
* Fecha de regreso
* Opción de solo ida

El formulario dirige a la pantalla de vuelos disponibles.

**Archivo:** `buscar-vuelos.html`

[Vista previa](img/cap.png)

---

### Vuelos disponibles

Muestra los vuelos disponibles para una ruta seleccionada, incluyendo información como:

* Código del vuelo
* Hora de salida
* Hora de llegada
* Duración
* Precio
* Opción para seleccionar el vuelo

La presentación de los vuelos se adapta al tamaño de pantalla:

* Computador y tablet: dos vuelos por fila.
* Celular: un vuelo por fila.

**Archivo:** `vuelos.html`

[Vista previa](img/cap.png)

---

### Check-in

Permite simular el proceso de check-in de un pasajero mediante un formulario.

**Archivo:** `checkin.html`

[Vista previa](img/cap.png)

---

### Mis vuelos

Permite consultar los vuelos reservados por el usuario.

Cada tarjeta muestra:

* Código del vuelo
* Estado
* Ciudad de origen
* Ciudad de destino
* Horarios
* Fecha
* Duración
* Precio

**Archivo:** `mis-vuelos.html`

[Vista previa](img/cap.png)

---

### Recuperar contraseña

Permite iniciar el proceso de recuperación de contraseña mediante el correo electrónico del usuario.

**Archivo:** `recuperar.html`

[Vista previa](img/cap.png)

---

## Diseño

El diseño de ACME AIR utiliza una combinación de colores basada principalmente en:

* `#d13cff`
* `#00b0ff`
* Blanco
* Tonos grises

Se utilizan tarjetas, botones, sombras, bordes redondeados y degradados para crear una interfaz moderna y sencilla.

---

## Diseño Responsive

El proyecto está diseñado para adaptarse a diferentes tamaños de pantalla.

Se consideran principalmente:

| Dispositivo | Tamaño |
| ----------- | ------ |
| Móvil       | 320px  |
| Tablet      | 768px  |
| Computador  | 1024px |

En dispositivos móviles los elementos se organizan verticalmente para facilitar la navegación.

En tablets y computadores se aprovecha el espacio disponible para mostrar los elementos de forma más amplia.

---

## Estructura del proyecto

```text
acme-air-app/
│
├── index.html
├── menu.html
├── registro.html
├── crear-contraseña.html
├── buscar-vuelos.html
├── vuelos.html
├── checkin.html
├── mis-vuelos.html
├── recuperar.html
│
├── css/
│   ├── style.css
│   ├── forms.css
│   ├── layout.css
│   └── responsive.css
│
└── img/
    ├── logo.png
    ├── logo_menu.jpg
    ├── icono.jpg
    │
    └── icons/
        ├── icon-perfil.jpg
        └── icon-viajes.jpg
```

---

## Archivos CSS

### style.css

Contiene los estilos generales de la aplicación:

* Tipografía
* Colores
* Fondos
* Botones
* Estilos generales

### layout.css

Contiene la estructura y distribución de los elementos:

* Contenedores
* Tarjetas
* Organización de secciones
* Alineación de elementos

### forms.css

Contiene los estilos relacionados con:

* Formularios
* Inputs
* Selects
* Botones
* Tarjetas de vuelos
* Información de vuelos

### responsive.css

Contiene las reglas necesarias para adaptar la aplicación a diferentes tamaños de pantalla.

---

## Navegación

La navegación principal del proyecto funciona mediante enlaces y formularios HTML.

```text
                    LOGIN
                 index.html
                      |
          +-----------+-----------+
          |           |           |
          v           v           v
      Registro    Recuperar     Menú
          |           |           |
          v           v           +-- Buscar vuelos
   Crear contraseña              +-- Check-in
          |                      +-- Mis vuelos
          +----------+           |
                     |           +-- Cerrar sesión
                     v                    |
                    Menú                  v
                                    index.html
```

---

## Tecnologías utilizadas

### HTML5

Utilizado para construir la estructura y contenido de las páginas.

### CSS3

Utilizado para:

* Diseño visual
* Colores
* Animaciones
* Transiciones
* Responsive Design
* Grid
* Flexbox

### Git y GitHub

Utilizados para el control de versiones y almacenamiento del proyecto.

---

## JavaScript

Este proyecto fue desarrollado **sin JavaScript**, de acuerdo con los requerimientos de la actividad.

La navegación entre las diferentes vistas se realiza mediante:

* Enlaces `<a>`
* Formularios `<form>`
* Botones `<button>`
* Atributos `action`
* Método `GET`

---

## Cómo ejecutar el proyecto

### 1. Descargar o clonar el proyecto

Si el proyecto se encuentra en GitHub:

```bash
git clone URL_DEL_REPOSITORIO
```

### 2. Abrir la carpeta

Ingresar a la carpeta del proyecto:

```bash
cd acme-air-app
```

### 3. Abrir el proyecto

Abrir el archivo:

```text
index.html
```

También se puede utilizar **Visual Studio Code** y abrir el proyecto con un servidor local como Live Server.

---

## Flujo principal de la aplicación

El flujo principal del usuario es:

1. Ingresar al sistema.
2. Iniciar sesión.
3. Acceder al menú principal.
4. Seleccionar una opción.
5. Buscar o consultar vuelos.
6. Visualizar la información.
7. Regresar al menú.
8. Cerrar sesión.

---

## Consideraciones de accesibilidad

Se aplicaron algunas prácticas básicas de accesibilidad:

* Uso de etiquetas semánticas de HTML5.
* Uso de `alt` en imágenes.
* Asociación de campos de formulario con sus respectivos identificadores.
* Uso de elementos HTML adecuados para cada función.
* Diseño adaptable a diferentes dispositivos.

---

## Autores

**Proyecto académico - ACME AIR**

Desarrollado como parte del proceso de formación en desarrollo web.

---

## Estado del proyecto

**Proyecto funcional**

El proyecto cuenta con las diferentes vistas solicitadas y navegación simulada entre ellas mediante HTML y CSS.

---

## Licencia

Este proyecto fue desarrollado con fines **académicos y educativos**.
