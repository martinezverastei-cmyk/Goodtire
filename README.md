# Good Tire · Ubicación de almacenes (Angular)

Aplicación web que resuelve el caso Good Tire, Inc. (problema de transporte + decisión de qué
almacenes abrir). Todos los datos son editables y los resultados, tablas y conclusiones se
recalculan automáticamente.

## Ejecutar
    npm install
    npx ng serve        # abre http://localhost:4200
    npx ng build        # versión de producción en dist/

## Estructura (src/app)
- core/models.ts        Tipos de datos
- core/solver.ts        Algoritmo: enumera combinaciones + flujo de costo mínimo (problema de transporte)
- core/good-tire.ts     Datos del caso (Tablas 9.23 y 9.24) — valores iniciales
- core/case-store.ts    Estado reactivo (signals): al cambiar un dato se recalcula todo
- core/conclusions.ts   Conclusiones automáticas en español
- data-editor/          Pestaña 1: edición de datos
- results/              Pestaña 2: conclusiones y todas las tablas de resultados
- explanation/          Pestaña 3: «¿De dónde sale cada valor o resultado?»
- styles.css            Bordes, botones, transiciones y animaciones
