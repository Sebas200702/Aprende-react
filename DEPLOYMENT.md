# Guía de Despliegue / Deployment Guide

## 🚀 Opciones de Despliegue

### Opción 1: Mintlify Cloud (Recomendado)

La forma más fácil de publicar tu documentación es usar Mintlify Cloud:

1. **Crear cuenta en Mintlify**
   - Ve a [https://mintlify.com](https://mintlify.com)
   - Crea una cuenta gratuita

2. **Conectar con GitHub**
   - En el dashboard de Mintlify, haz clic en "New Project"
   - Conecta tu repositorio `Sebas200702/Aprende-react`
   - Mintlify detectará automáticamente el archivo `mint.json`

3. **Deploy automático**
   - Cada push a tu repositorio actualizará la documentación automáticamente
   - Tu documentación estará disponible en `aprende-react.mintlify.app` (o tu dominio personalizado)

### Opción 2: Desarrollo Local

Para previsualizar la documentación localmente:

```bash
# Instalar Mintlify CLI
npm install -g mintlify

# Navegar al directorio del proyecto
cd Aprende-react

# Iniciar servidor de desarrollo
mintlify dev
```

La documentación estará disponible en `http://localhost:3000`

### Opción 3: Despliegue en Vercel/Netlify

También puedes desplegar usando otros servicios:

#### Vercel:
```bash
# Instalar Vercel CLI
npm install -g vercel

# Deploy
vercel
```

#### Netlify:
```bash
# Instalar Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy
```

## 🔧 Configuración

### Dominio personalizado

Para usar un dominio personalizado en Mintlify Cloud:

1. Ve a Project Settings en tu dashboard de Mintlify
2. Agrega tu dominio personalizado
3. Configura los DNS según las instrucciones

### Variables de entorno

Si necesitas variables de entorno, créalas en:
- Mintlify Cloud: Project Settings > Environment Variables
- Vercel/Netlify: Settings > Environment Variables

## 📝 Actualizar contenido

1. Edita los archivos `.mdx` en tu repositorio
2. Haz commit y push de los cambios
3. La documentación se actualizará automáticamente

## 🐛 Solución de problemas

### La documentación no se actualiza

- Verifica que el `mint.json` sea válido JSON
- Revisa los logs de deploy en tu plataforma
- Asegúrate de que todos los archivos `.mdx` estén listados en `navigation`

### Errores de sintaxis MDX

- Verifica que todas las etiquetas JSX estén cerradas
- Asegúrate de que los bloques de código tengan la sintaxis correcta
- Usa el validador MDX: [https://mdxjs.com/playground/](https://mdxjs.com/playground/)

### Imágenes no cargan

- Las imágenes deben estar en la carpeta raíz o en subcarpetas
- Usa rutas relativas: `/images/foto.jpg`
- Formatos soportados: PNG, JPG, SVG, GIF

## 📚 Recursos adicionales

- [Documentación de Mintlify](https://mintlify.com/docs)
- [MDX Documentation](https://mdxjs.com/)
- [React Documentation](https://react.dev/)

## ✨ Tips

- Usa imágenes optimizadas para mejor rendimiento
- Mantén los archivos MDX organizados y bien nombrados
- Usa componentes de Mintlify (`<Tip>`, `<Warning>`, `<Card>`) para contenido rico
- Revisa la documentación en móvil - Mintlify es responsive por defecto

---

¿Necesitas ayuda? Abre un issue en el [repositorio de GitHub](https://github.com/Sebas200702/Aprende-react/issues)
