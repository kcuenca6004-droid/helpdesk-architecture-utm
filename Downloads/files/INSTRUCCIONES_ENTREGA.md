# GUÍA DE ENTREGA - ACTIVIDAD #3: MAQUETACIÓN ESTRUCTURAL HTML5

## Resumen de la Actividad Realizada

Se han creado tres archivos HTML5 interconectados para un sistema de Help Desk con estructura semántica completa:

### 📄 Archivos Creados:

1. **index.html** - Dashboard Principal
   - Encabezado y navegación
   - Bienvenida y resumen del sistema
   - Estadísticas generales
   - Enlaces a las otras secciones

2. **reportar.html** - Formulario de Reporte
   - Formulario completo con validación HTML5
   - Campos de texto (título, email, teléfono)
   - Lista desplegable para categorías (Red, Hardware, Software)
   - Botones radio para prioridades (Alta, Media, Baja)
   - Área de texto para descripción
   - Instrucciones de uso
   - Botones de envío y limpieza

3. **tickets.html** - Listado de Tickets
   - Sección de filtros
   - Tabla estructurada con tickets registrados
   - Detalles individuales de cada ticket
   - Estadísticas del sistema

### ✅ Requisitos Cumplidos:

#### 1. Estructura y Navegación (3 pts)
- ✓ Tres archivos HTML interconectados
- ✓ Barra de navegación <nav> común en todas las páginas
- ✓ Enlaces funcionales entre todas las secciones

#### 2. Semántica HTML5 Obligatoria (3 pts)
Cada página utiliza correctamente:
- ✓ <header> - Encabezado con título y descripción
- ✓ <nav> - Menú de navegación
- ✓ <main> - Contenido principal exclusivo
- ✓ <section> - Bloques de información temáticos
- ✓ <article> - Contenidos independientes
- ✓ <footer> - Información de contacto y derechos
- ✓ Etiquetas semánticas adicionales: <form>, <table>, <dl>, <dt>, <dd>

#### 3. Componentes de Formulario y Datos (2 pts)
En reportar.html:
- ✓ Campo de texto: Título del incidente
- ✓ Campos de texto: Email y teléfono
- ✓ Lista desplegable <select>: Categorías
- ✓ Botones radio <input type="radio">: Niveles de prioridad
- ✓ Área de texto <textarea>: Descripción detallada
- ✓ Checkbox: Recursos adjuntos
- ✓ Botones: Enviar y Limpiar

En tickets.html:
- ✓ Tabla estructurada <table> con todos los tickets
- ✓ Listas de detalles con <dl>, <dt>, <dd>
- ✓ Lista de estadísticas con <ul> y <ol>

#### 4. Estándares, Calidad y Versiones (2 pts)
- ✓ Código HTML5 válido y bien estructurado
- ✓ Declaración DOCTYPE correcta
- ✓ Meta etiquetas apropiadas (charset, viewport, descripción)
- ✓ Atributos name en formularios

---

## 📋 PASOS PARA VALIDACIÓN EN W3C

### Paso 1: Validar en el Markup Validation Service
1. Ir a: https://validator.w3.org/
2. Seleccionar la pestaña "Upload File" o copiar el código en "Validate by Direct Input"
3. Para cada archivo (index.html, reportar.html, tickets.html):
   - Subir el archivo o copiar el contenido
   - Hacer clic en "Check"
   - Verificar que no haya errores (Warning son aceptables)
   - **Capturar pantalla del resultado** ✓ LIBRE DE ERRORES

### Paso 2: Puntos a Verificar
- Declaración DOCTYPE correcta
- Metaetiquetas obligatorias
- Estructura semántica correcta
- Atributos bien formados
- Formularios con validación

---

## 🔧 PASOS PARA GITHUB - GITFLOW

### Paso 1: Crear Repositorio (si no existe)
```bash
# En GitHub, crear un nuevo repositorio llamado:
# apellido-nombre-helpdesk
# o similar
```

### Paso 2: Clonar y Configurar Localmente
```bash
# Clonar el repositorio
git clone https://github.com/tuusuario/tu-repositorio.git
cd tu-repositorio

# Configurar usuario (si no está hecho)
git config user.name "Tu Nombre"
git config user.email "tu.email@example.com"
```

### Paso 3: Crear Estructura de Carpetas
```bash
# Crear carpetas para organizar
mkdir -p assets/img
mkdir -p assets/css  # Para futuros estilos

# Mover o copiar los archivos HTML
# index.html
# reportar.html
# tickets.html
# (en la raíz del proyecto)
```

### Paso 4: Crear Rama Feature
```bash
# Asegurarse en rama develop (o main)
git checkout develop

# Crear nueva rama feature
git checkout -b feature/maquetacion-html

# Verificar que estamos en la rama correcta
git branch
```

### Paso 5: Agregar y Confirmar Cambios
```bash
# Agregar todos los archivos
git add .

# Verificar los cambios
git status

# Hacer commit con mensaje descriptivo
git commit -m "feat: implementar maquetación estructural HTML5 del Help Desk

- Crear index.html con dashboard principal
- Crear reportar.html con formulario de incidentes
- Crear tickets.html con listado de tickets
- Implementar navegación común en todas las páginas
- Usar etiquetas semánticas HTML5 correctamente
- Validado en W3C sin errores"
```

### Paso 6: Push a GitHub
```bash
# Subir la rama feature a GitHub
git push -u origin feature/maquetacion-html
```

### Paso 7: Hacer Merge a Develop
```bash
# Opción A: Pull Request en GitHub (Recomendado)
# 1. En GitHub, ir al repositorio
# 2. Hacer clic en "Pull requests"
# 3. Clic en "New pull request"
# 4. Seleccionar:
#    - Base: develop
#    - Compare: feature/maquetacion-html
# 5. Crear el PR con descripción
# 6. Hacer Merge

# Opción B: Merge local
git checkout develop
git merge feature/maquetacion-html
git push origin develop
```

---

## 📑 ESTRUCTURA DE CARPETAS RECOMENDADA

```
tu-repositorio/
├── index.html
├── reportar.html
├── tickets.html
├── README.md
├── assets/
│   ├── img/
│   │   └── logo.png (opcional)
│   └── css/
│       └── styles.css (para unidad 3)
└── .gitignore
```

---

## 📝 README.md - Ejemplo

Crea un archivo README.md en la raíz del proyecto:

```markdown
# Sistema de Help Desk - HTML5

## Descripción
Sistema de gestión de incidentes (Help Desk) implementado en HTML5 con estructura semántica.

## Archivos
- **index.html**: Dashboard principal
- **reportar.html**: Formulario de reporte de incidentes
- **tickets.html**: Listado y detalles de tickets

## Requisitos
- Navegador web moderno
- Validación W3C: ✓ Libre de errores

## Validación
Código validado en: https://validator.w3.org/

## Autor
[Tu nombre] - Estudiante de Desarrollo de Sistemas Informáticos

## Fecha
Junio 2026
```

---

## 📸 CAPTURAS PARA EL PDF DE ENTREGA

Debe incluir:

1. **Captura del repositorio GitHub**
   - URL pública del repositorio
   - Estructura de archivos
   - Historial de commits

2. **Capturas del código HTML**
   - index.html (fragmentos principales)
   - reportar.html (formulario)
   - tickets.html (tabla y detalles)

3. **Capturas de validación W3C**
   - Resultado de validación para cada archivo
   - Mensaje: "Document checking completed. No errors or warnings to show."

4. **Capturas de navegación en navegador**
   - index.html renderizado
   - reportar.html con formulario
   - tickets.html con tabla y detalles
   - Enlaces de navegación funcionando

---

## 📄 DOCUMENTO PDF DE ENTREGA

Nombre del archivo: **apellido_nombre_actividad3.pdf**

Contenido sugerido:
1. Portada (conforme a formato universitario)
2. Índice
3. Introducción
4. Descripción de la solución
5. Estructura del proyecto
6. Archivos creados (con código)
7. Capturas de validación W3C
8. Capturas de funcionamiento en navegador
9. Capturas del repositorio GitHub
10. Conclusiones
11. Enlaces públicos (URL del repositorio)

---

## ✨ CHECKLIST FINAL

Antes de entregar:

- [ ] Los 3 archivos HTML creados y funcionando
- [ ] Navegación común en todas las páginas
- [ ] Etiquetas semánticas correctas (<header>, <nav>, <main>, <section>, <article>, <footer>)
- [ ] Formulario con todos los campos requeridos
- [ ] Tabla de tickets con datos de ejemplo
- [ ] Validación W3C sin errores (para cada archivo)
- [ ] Código subido a GitHub en rama feature/maquetacion-html
- [ ] Merge realizado a rama develop
- [ ] README.md creado
- [ ] Capturas de pantalla de todo lo anterior
- [ ] PDF de entrega generado con formato universitario
- [ ] Archivo nombrado correctamente: apellido_nombre_actividad3.pdf

---

## 🔗 LINKS IMPORTANTES

- **Validador W3C**: https://validator.w3.org/
- **HTML5 Semántico**: https://developer.mozilla.org/es/docs/Web/HTML/Element
- **GitHub**: https://github.com
- **Git Cheat Sheet**: https://education.github.com/git-cheat-sheet-education.pdf

---

## 📞 SOPORTE TÉCNICO

Si encuentras problemas:

1. **Validación W3C rechaza el código**
   - Revisar DOCTYPE
   - Verificar cierre correcto de etiquetas
   - Asegurarse que los atributos estén bien formados

2. **Git no funciona**
   - Instalar Git desde: https://git-scm.com/
   - Configurar usuario: `git config --global user.name "Tu Nombre"`

3. **Problemas con GitHub**
   - Crear cuenta en: https://github.com
   - Generar token de acceso (Personal Access Token)
   - Usar token como contraseña en push

---

**Última actualización**: Junio 2026
**Versión**: 1.0
