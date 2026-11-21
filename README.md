# recetas

Web app personal de recetas, pensada para el iPhone (GitHub Pages).

- `index.html` — la app (home con una lista de recetas → detalle con ingredientes y pasos desplegables).
- `recetas/indice.json` — listado de recetas que aparece en la home.
- `recetas/<slug>.json` — una receta por archivo.

## Formato de receta

```json
{
  "titulo": "…",
  "categoria": "…",
  "tiempo": "30 min",
  "dificultad": "Fácil",
  "raciones": 4,
  "descripcion": "…",
  "ingredientes": [
    { "grupo": "Para la salsa" },
    { "nombre": "Harina", "cantidad": 200, "unidad": "g", "nota": "opcional" },
    { "nombre": "Sal", "cantidad": null, "unidad": "", "nota": "al gusto" }
  ],
  "pasos": [ { "texto": "…", "consejo": "opcional" } ],
  "consejos": [ "opcional" ]
}
```

Unidades: siempre sistema métrico (`g`, `ml`) o `cda`/`cdta` (cucharada/cucharadita) o vacío para unidades sueltas.
