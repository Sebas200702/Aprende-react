# Contribuyendo a Aprende React 🤝

¡Gracias por tu interés en contribuir! Esta guía te ayudará a empezar.

## 🎯 Cómo puedes contribuir

Hay muchas formas de contribuir a este proyecto:

- 📝 **Mejorar contenido**: Corregir errores, mejorar explicaciones, agregar ejemplos
- 🆕 **Nuevo contenido**: Agregar nuevas páginas o secciones
- 🐛 **Reportar errores**: Encontrar y reportar errores en el contenido
- 💡 **Sugerencias**: Proponer mejoras o nuevos temas
- 🌍 **Traducciones**: Ayudar a traducir a otros idiomas

## 🚀 Primeros pasos

### 1. Fork y Clone

```bash
# Fork el repositorio en GitHub
# Luego clona tu fork
git clone https://github.com/TU-USUARIO/Aprende-react.git
cd Aprende-react
```

### 2. Instalar Mintlify

```bash
npm install -g mintlify
```

### 3. Ejecutar localmente

```bash
mintlify dev
```

Esto abrirá la documentación en `http://localhost:3000`

## 📝 Guía de estilo

### Lenguaje

- **Usa lenguaje sencillo y claro**: Evita jerga técnica innecesaria
- **Analogías cotidianas**: Compara conceptos técnicos con situaciones de la vida real
- **Tono amigable**: Como si le explicaras a un amigo

### Estructura de contenido

Cada página debe tener:

1. **Título descriptivo**: Claro y conciso
2. **Descripción**: Breve resumen del contenido
3. **Introducción**: Con analogía o ejemplo cotidiano
4. **Explicación detallada**: Con código de ejemplo
5. **Ejemplos prácticos**: Casos de uso reales
6. **Buenas prácticas**: Tips y mejores prácticas
7. **Navegación**: Link a la siguiente página

### Código de ejemplo

```typescript
// ✅ BUENO: Código completo y funcional
interface Usuario {
  nombre: string;
  edad: number;
}

function MostrarUsuario({ usuario }: { usuario: Usuario }) {
  return (
    <div>
      <h2>{usuario.nombre}</h2>
      <p>Edad: {usuario.edad}</p>
    </div>
  );
}

// ❌ MALO: Código incompleto o confuso
function Algo({ data }) {
  return <div>{data}</div>;
}
```

### Componentes de Mintlify

Usa componentes de Mintlify para mejorar el contenido:

```mdx
<Tip>
  Consejos útiles para el lector
</Tip>

<Warning>
  Advertencias importantes
</Warning>

<Note>
  Notas adicionales o aclaraciones
</Note>

<Info>
  Información contextual
</Info>

<Card title="Título" icon="icon-name" href="/ruta">
  Descripción de la tarjeta
</Card>

<Accordion title="Pregunta">
  Respuesta expandible
</Accordion>
```

## 🔍 Proceso de revisión

1. **Crea una rama**: `git checkout -b feature/mi-mejora`
2. **Haz tus cambios**: Edita los archivos `.mdx`
3. **Prueba localmente**: `mintlify dev` para verificar
4. **Commit**: `git commit -m "Descripción clara del cambio"`
5. **Push**: `git push origin feature/mi-mejora`
6. **Pull Request**: Abre un PR en GitHub

### Checklist del PR

Antes de enviar tu PR, asegúrate de:

- [ ] El código de ejemplo funciona correctamente
- [ ] La ortografía y gramática son correctas
- [ ] Las imágenes (si hay) están optimizadas
- [ ] Los links funcionan correctamente
- [ ] El formato MDX es válido
- [ ] Has probado localmente con `mintlify dev`
- [ ] El contenido sigue la guía de estilo

## 📋 Tipos de contribuciones

### Corrección de errores

```markdown
Título: Fix: Corregir error de tipado en ejemplo de useState

Descripción:
- Corrijo el tipo incorrecto en el ejemplo
- Agrego nota explicativa sobre el tipo correcto
```

### Nuevo contenido

```markdown
Título: Feat: Agregar página sobre React Router

Descripción:
- Nueva página explicando React Router
- Incluye ejemplos prácticos
- Sigue la estructura y estilo del resto del sitio
```

### Mejora de contenido

```markdown
Título: Docs: Mejorar explicación de useEffect

Descripción:
- Agrego más ejemplos de casos de uso
- Mejoro la analogía inicial
- Incluyo diagrama explicativo
```

## 🎨 Agregar imágenes

1. Guarda las imágenes en carpeta `/images/`
2. Usa formato optimizado (PNG o WEBP)
3. Nombra descriptivamente: `ejemplo-usestate.png`
4. Referencia en MDX: `![Descripción](/images/ejemplo-usestate.png)`

## 🌍 Traducciones

Si quieres contribuir con traducciones:

1. Crea carpeta con código de idioma: `/es/`, `/en/`, etc.
2. Traduce los archivos `.mdx`
3. Actualiza `mint.json` con las rutas traducidas

## ❓ Preguntas

Si tienes preguntas:

- Abre un [issue en GitHub](https://github.com/Sebas200702/Aprende-react/issues)
- Revisa los [issues existentes](https://github.com/Sebas200702/Aprende-react/issues)

## 📜 Código de conducta

- Se respetuoso y profesional
- Acepta críticas constructivas
- Enfócate en lo mejor para el proyecto
- Ayuda a otros contribuidores

## 🙏 Agradecimientos

¡Gracias por contribuir a hacer que aprender React sea más fácil para todos!

---

**Happy coding!** 🚀
