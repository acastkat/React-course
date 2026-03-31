# Concepto 1 de 5: ¿Qué es React y cómo “piensa” (componentes + UI declarativa)

**Idea central:**
React te ayuda a construir interfaces a partir de **componentes** (piezas reutilizables) que devuelven “cómo debería verse” la UI según el estado actual.

**Declarativo vs. imperativo:**
En vez de “tocar el DOM” manualmente (imperativo), describís el resultado (“si ```isLoggedIn``` es true, mostrà X; si no, Y”) y React se encarga de actualizar la pantalla.

**Componente = función:**
En React moderno, un componente suele ser una **función** que retorna JSX (una sintaxis parecida a HTML dentro de JavaScript).

**JSX no es HTML:** 
Es sintaxis que se convierte a JavaScript. Por eso podés mezclar expresiones (```{...}```) y componer componentes como si fueran tags.

**Cómo se arma una app:**
Una pantalla es un árbol de componentes (App → Header → Nav, etc.). Pensar en “piezas” te simplifica mantenimiento y reutilización.

**Aplicación real:**
Cuando algo cambia (por ejemplo, una búsqueda, un toggle, datos que llegan de una API), lo expresás como **estado**; React vuelve a renderizar lo necesario para reflejarlo.

## Ejemplo práctico paso a paso (mínimo)

1. Definís un componente como función.
2. Le pasás datos por props.
3. Renderizás distinto según esos datos.
```
function Greeting({ name }) {
  return <h1>Hola, {name}</h1>;
}

export default function App() {
  return (
    <div>
      <Greeting name="Andrea" />
    </div>
  );
}
```
   Idea central: React te ayuda a construir interfaces a partir de componentes (piezas reutilizables) que devuelven “cómo debería verse” la UI según el estado actual.
Declarativo vs. imperativo: en vez de “tocar el DOM” manualmente (imperativo), describís el resultado (“si isLoggedIn es true, mostrà X; si no, Y”) y React se encarga de actualizar la pantalla.
Componente = función: en React moderno, un componente suele ser una función que retorna JSX (una sintaxis parecida a HTML dentro de JavaScript).
JSX no es HTML: es sintaxis que se convierte a JavaScript. Por eso podés mezclar expresiones ({...}) y componer componentes como si fueran tags.
Cómo se arma una app: una pantalla es un árbol de componentes (App → Header → Nav, etc.). Pensar en “piezas” te simplifica mantenimiento y reutilización.
Aplicación real: cuando algo cambia (por ejemplo, una búsqueda, un toggle, datos que llegan de una API), lo expresás como estado; React vuelve a renderizar lo necesario para reflejarlo.
Ejemplo práctico paso a paso (mínimo)

Definís un componente como función.
Le pasás datos por props.
Renderizás distinto según esos datos.
