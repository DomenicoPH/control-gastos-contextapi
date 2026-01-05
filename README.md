# Control de Gastos con React Context API
▶️[demo site](https://gno-budget-control.netlify.app/)

Una aplicación completa para gestionar gastos personales construida con React, TypeScript y Context API para un manejo eficiente del estado global.

## Características principales

- **Gestión de presupuesto**: Define un presupuesto inicial y haz seguimiento en tiempo real
- **Registro de gastos**: Añade gastos con nombre, cantidad, categoría y fecha
- **Categorías predefinidas**: 7 categorías organizadas (Ahorro, Comida, Casa, Gastos Varios, Ocio, Salud, Suscripciones)
- **Filtrado por categoría**: Visualiza gastos específicos por categoría
- **Edición y eliminación**: Modifica o elimina gastos existentes
- **Persistencia local**: Los datos se guardan automáticamente en localStorage
- **Interfaz responsive**: Diseño moderno con Tailwind CSS
- **Modal interactivo**: Formulario en modal para agregar/editar gastos
- **Estadísticas visuales**: Progreso circular del presupuesto vs gastos

## Tecnologías utilizadas

- **React 19** + **TypeScript** - Desarrollo frontend con tipado estático
- **Vite** - Build tool y entorno de desarrollo ultrarrápido
- **Tailwind CSS 4** - Framework de estilos utility-first
- **Context API** - Gestión de estado global nativa de React
- **Headless UI** - Componentes UI accesibles
- **Heroicons** - Biblioteca de iconos SVG
- **UUID** - Generación de IDs únicos para gastos
- **React Date Picker** - Selector de fecha

## Estructura del proyecto

src/  
├── App.tsx                    # Componente principal  
├── main.tsx                   # Punto de entrada  
├── index.css                  # Estilos globales  
├── context/  
│   └── BudgetContext.tsx      # Contexto para estado global  
├── reducers/  
│   └── budget-reducer.ts      # Reducer para estado global  
├── hooks/  
│   └── useBudget.ts           # Custom hook para acceder al contexto  
├── helpers/  
│   └── index.ts               # Helpers para formato de divisa y fecha  
|  
├── components/  
│   ├── AmountDisplay.tsx     # Componente que muestra el monto  
│   ├── BudgetForm.tsx        # Formulario de presupuesto inicial  
│   ├── BudgetTracker.tsx     # Seguimiento visual del presupuesto  
│   ├── ExpenseModal.tsx      # Modal para agregar/editar gastos  
│   ├── ExpenseForm.tsx       # Formulario de gastos  
│   ├── ExpenseList.tsx       # Lista de gastos  
│   ├── ExpenseDetail.tsx     # Item individual de gasto  
│   └── FilterByCategory.tsx  # Selector de filtro por categoría  
|  
├── data/  
│   └── categories.ts         # Datos de categorías y funciones helpers  
└── types/  
    └── index.ts              # Definiciones TypeScript  

## ▶ Ejecutar el proyecto localmente

Clona el repositorio e instala las dependencias:

```bash
npm install
```

Inicia el servidor de desarrollo:

```bash
npm run dev
```

Compilar para producción:

```bash
npm run build
```

Previsualizar build:

```bash
npm run preview
```

---

## Objetivo del proyecto

Este proyecto forma parte de un **portfolio frontend**, con el objetivo de demostrar:

- Manejo de estado complejo con useReducer
- Manejo de estado global con contextApi
- Arquitectura limpia y mantenible
- Tipado sólido con TypeScript
- Diseño de UI con Tailwind CSS moderno
- Buenas prácticas en React

---

## Licencia

Este proyecto es de uso libre con fines educativos y demostrativos.

---

**Domenico Pagano <dpaganoh@gmail.com>**  

Desarrollado como proyecto de práctica y portfolio frontend.  
💼 [Domenico Pagano Portafolio](https://portfolio-gnomono.vercel.app/)

---

## DevDep  

    npm i @headlessui/react  
    npm i @heroicons/react  
    npm i uuid  
    npm i --save-dev @types/uuid  
    npm i react-swipeable-list
    npm i prop-types
    npm i react-circular-progressbar


## npm docs

  uuid: 
  https://www.npmjs.com/package/uuid

  rect-swipeable-list:
  https://www.npmjs.com/package/react-swipeable-list

  react-circular-progressbar:
  https://www.npmjs.com/package/react-circular-progressbar