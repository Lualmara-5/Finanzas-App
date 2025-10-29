# Finanzas-App

Aplicación web creada con Angular 17+ y TypeScript para gestionar finanzas personales: controlar transacciones, presupuestos y metas financieras, con un diseño tipo dashboard moderno.

---

## 🚀 Tecnologías utilizadas

* Angular 17+ (standalone components)
* TypeScript
* HTML5 / CSS3
* Angular Router
* Signals (para manejo reactivo del estado)

---

## 📂 Estructura del proyecto

```
src/
└── app/
    ├── components/
    │   ├── sidebar/        → Menú lateral de navegación
    │   │   ├── sidebar.ts
    │   │   ├── sidebar.html
    │   │   └── sidebar.css
    │   ├── dashboard/      → Panel principal (standalone)
    │   │   └── ...
    │   ├── transactions/   → Transacciones (standalone)
    │   │   └── ...
    │   ├── budgets/        → Presupuestos (standalone)
    │   │   └── ...
    │   └── goals/          → Metas financieras (standalone)
    │       └── ...
    │
    ├── app.html            → Layout principal con <app-sidebar> y <router-outlet>
    ├── app.ts              → Componente raíz (standalone)
    ├── app.css
    ├── app.spec.ts
    ├── app.config.ts       → Configs de la app (env, constantes — opcional)
    └── app.routes.ts       → Configuración de rutas (exporta rutas para bootstrap)
src/
├── index.html
├── main.ts                 → punto de entrada + bootstrapApplication
└── styles.css              → estilos globales
```

## ⚙️ Instalación y ejecución
1. Clonar el repositorio
```bash
git clone https://github.com/tuusuario/finanzas-app.git
cd finanzas-app
```

2. Instalar dependencias
```bash
npm install
```

3. Ejecutar la aplicación
```bash
ng serve
```

4. Abrir en el navegador
```bash
http://localhost:4200
```

---

## 🧠 Próximos pasos

 * Implementar autenticación de usuario
 * Agregar gráficos con datos reales (chart.js o ngx-charts)
 * Integrar almacenamiento (Firebase / Supabase)
 * Crear versión móvil con menú colapsable
 * Agregar modo oscuro/ligero automático

---

## 👨‍💻 Autor

Luis Alejandro Martínez Ramírez (Lualmara)

Proyecto creado con el propósito de aprender Angular y desarrollo frontend práctico, combinando diseño y lógica para construir un sistema de finanzas personales funcional.

---

Made with ❤️ by **Alejo (DevByLualmara)**
