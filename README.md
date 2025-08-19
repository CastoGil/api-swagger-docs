# api-swagger-docs

Documentación interactiva de una API (Products & Carts) usando **OpenAPI/Swagger** sobre Node.js/Express.

## 📚 Características
- Definición OpenAPI centralizada (`swagger.yaml`).
- Swagger UI servido en `/api/docs`.
- Esquemas de modelos (`Product`, `Cart`), parámetros, respuestas y ejemplos.
- Soporte para auth (Bearer) listo para ampliar.

## 🥐 Stack
- Node.js, Express
- swagger-ui-express
- YAML (OpenAPI 3)

## 🚀 Inicio rápido
    npm ci
    npm run dev
    # abre http://localhost:3000/api/docs

## 💂 Estructura
    /src
      /routes
      /middlewares
    swagger.yaml

## 📎 Cómo está organizada la documentación
- `swagger.yaml` define los endpoints de `products` y `carts`, los esquemas de modelos y componentes comunes.
- En tu servidor Express se monta Swagger UI en `/api/docs` mediante `swagger-ui-express`.
- Para añadir más rutas o recursos, edita `swagger.yaml` y reinicia la aplicación.

## ✍️ Edición de la spec
Puedes usar el editor web [Swagger Editor](https://editor.swagger.io/) para crear y validar la especificación.
1. Copia el contenido de `swagger.yaml` en Swagger Editor.
2. Realiza los cambios necesarios (endpoints, esquemas, ejemplos, parámetros).
3. Valida que la spec no tenga errores.
4. Copia el YAML actualizado de vuelta a `swagger.yaml` en tu proyecto y haz commit.

## 📄 Licencia
MIT
