# Lección 5: Corrección de errores comunes en monorepos

## Objetivo
Ajustar los nombres de los workspaces y scripts en el `package.json` raíz para que el proyecto funcione correctamente.

## Pasos detallados

1. Abre el archivo `package.json` en la raíz del proyecto.
2. Busca la sección `"scripts"`. Borra cualquier script que haga referencia a un workspace incorrecto (por ejemplo, `@celo-composer-minipay-template/react-app` o cualquier otro que no coincida con el nombre real del workspace).
3. Copia y pega este bloque en la sección `"scripts"` de tu `package.json` raíz (ajusta el nombre del workspace si es necesario):

   ```json
   "scripts": {
     "react-app:dev": "yarn workspace @examples/react-app dev",
     "react-app:build": "yarn workspace @examples/react-app build",
     "react-app:start": "yarn workspace @examples/react-app start",
     "react-app:lint": "yarn workspace @examples/react-app lint"
   }
   ```

4. Verifica que el nombre del workspace (`@examples/react-app`) coincida exactamente con el campo `"name"` en `packages/react-app/package.json`.

5. (Opcional) Agrega un script raíz para mayor facilidad. Esto te permitirá iniciar el servidor de desarrollo simplemente con `yarn dev` desde la raíz del proyecto. Agrega esta línea dentro del bloque `"scripts"`:

   ```json
   "dev": "yarn react-app:dev"
   ```

6. Ejemplo final de la sección `"scripts"`:

   ```json
   "scripts": {
     "react-app:dev": "yarn workspace @examples/react-app dev",
     "react-app:build": "yarn workspace @examples/react-app build",
     "react-app:start": "yarn workspace @examples/react-app start",
     "react-app:lint": "yarn workspace @examples/react-app lint",
     "dev": "yarn react-app:dev"
   }
   ```

---
[← Lección anterior](04-preparar-el-entorno.md) | [Siguiente lección →](06-iniciar-tu-aplicacion.md) 