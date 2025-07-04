# Lección 4: Preparar el entorno (.env y dependencias)

## Objetivo
Configurar tu entorno para que la app funcione correctamente.

## Pasos

Antes de iniciar tu proyecto, sigue estos pasos:

- Renombra `.env.template` a `.env` en `packages/react-app/`.
- Agrega tu WalletConnect Project ID desde [WalletConnect Cloud](https://cloud.walletconnect.com/).

1. Renombra el archivo:

   ```bash
   packages/react-app/.env.template → packages/react-app/.env
   ```

2. Abre el archivo `.env` y completa las variables necesarias (por ejemplo: claves API, direcciones de contrato, etc.).

3. Instala dependencias:

   ```bash
   yarn install
   ```

---
[← Lección anterior](03-tu-primer-proyecto.md) | [Siguiente lección →](05-corrección-de-errores-comunes.md) 