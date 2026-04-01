## Concepto 2 de 5: Estado (state) y eventos — hacer la UI “interactiva”

### Props vs. state:

Props = datos que entran desde el “padre” (solo lectura).
State = datos que vive dentro del componente y cambia con la interacción o con datos que llegan.
Hook clave: useState: te permite guardar un valor y actualizarlo; al actualizarlo, React re-renderiza el componente.
Eventos: la UI cambia reaccionando a eventos (onClick, onChange). En React, pasás funciones como manejadores.
Actualizaciones asíncronas: setState no “cambia ya y listo”; React puede agrupar cambios. Por eso a veces conviene usar la forma funcional: setCount(c => c + 1).
Patrón típico front-end: input controlado → guardás lo que tipea el usuario en state → renderizás resultados filtrados/validados.
Aplicación real para entrevistas: te van a mirar si podés construir un componente con estado, manejar formularios básicos y mantener la UI consistente.
Ejemplo práctico (contador + botón)
