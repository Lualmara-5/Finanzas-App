# Aprendizaje for me jaja

---

## SRC

```bash
src/
├── index.html
├── main.ts
└── styles.css
```

1. `index.html`

Tú no tocas este archivo casi nunca, salvo si:

* Quieres cambiar el título del sitio (<title>).
* Agregar meta etiquetas (SEO, icono, etc).
* O incluir scripts globales externos (raro en apps Angular).

2. `main.ts`

No necesitas modificarlo, salvo que quieras:

* Agregar algo global (por ejemplo, un provideHttpClient()).
* Cambiar el componente raíz (rara vez).
  
3. `styles.css`

Usualmente se usa para:

* Definir fuentes, colores globales, variables CSS, etc.
* Resetear márgenes y estilos del navegador.

---

## APP

1. `app.config.ts`

Es como el “panel de control” que conecta Angular con tus rutas y servicios globales.
Normalmente solo se modifica una vez, al agregar nuevas rutas o providers.

2. `app.css`

Archivo de estilos solo del componente raíz (App).

No afecta a otros componentes (por ejemplo, sidebar.css o dashboard.css son independientes).

Se usa para dar estructura visual a la app: espacio para el menú, márgenes, colores de fondo, etc.

3. `app.html`

Este archivo define la estructura principal (layout) de tu aplicación.

Aquí se renderiza el `Sidebar` y el contenido que cambia según la ruta.

Es como el esqueleto del sitio: a la izquierda el menú, a la derecha el contenido dinámico.
  
4. `app.routers.ts`

Define todas las rutas de navegación de tu aplicación.

Cada ruta indica:
* Qué componente se muestra.
* En qué URL se muestra.

Es el “mapa” de la aplicación.

Cada `path` = una página, cada `component` = su contenido.
  
5. `app.spec.ts`

Archivo de **tests automáticos** (pruebas unitarias). Angular lo crea por defecto, pero si no estás haciendo testing, puedes ignorarlo.

Sirve para comprobar que tu app funcione correctamente de forma automática.

6. `app.ts`

Es el componente raíz de la app, también conocido como root component.

Aquí se importan:

* El `Sidebar` (menú lateral).
* El `RouterOutlet` (para mostrar las páginas según la ruta).
* Otros componentes globales.

Es la “carcasa” donde se muestra todo lo demás. Aquí se conectan los componentes principales.
