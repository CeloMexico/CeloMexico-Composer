# Instalación y configuración de Celo Composer

## Objetivo de aprendizaje
Instalar Celo Composer y preparar el entorno de desarrollo para crear dApps en Celo.

## Prerrequisitos
- Node.js v20+ instalado
- Git v2.38+ instalado
- Cuenta en GitHub (opcional, para clonar repositorios)

## Instrucciones paso a paso
1. **Clona el repositorio de Celo Composer**
   ```bash
   git clone https://github.com/celo-org/celo-composer.git
   cd celo-composer
   ```
2. **Instala las dependencias**
   ```bash
   npm install
   # O, si usas yarn:
   # yarn install
   ```
3. **Verifica la instalación**
   ```bash
   node -v
   npm -v
   git --version
   ```
   Asegúrate de que las versiones cumplen los requisitos.
4. **Inicia el entorno de desarrollo**
   ```bash
   npm run dev
   ```
   Esto levantará la aplicación web en modo desarrollo.

## Código de ejemplo
```bash
# Ejemplo de clonación e instalación
 git clone https://github.com/celo-org/celo-composer.git
 cd celo-composer
 npm install
 npm run dev
```

## Ejercicios o preguntas de repaso
- ¿Qué comando usas para instalar las dependencias?
- ¿Cómo verificas la versión de Node.js instalada?

## Recursos adicionales
- [Guía oficial de instalación](https://github.com/celo-org/celo-composer#installation)
- [Descargar Node.js](https://nodejs.org/)
- [Descargar Git](https://git-scm.com/) 