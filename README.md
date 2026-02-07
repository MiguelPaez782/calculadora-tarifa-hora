# 💼 Calculadora de Tarifa por Hora

Una aplicación web moderna y gratuita que te ayuda a calcular cuánto debes cobrar por hora según tus gastos, objetivos de ingreso y jornada laboral. Perfecta para freelancers, profesionales independientes y cualquier persona que necesite establecer sus tarifas de manera profesional.

## ✨ Características

- 📊 **Cálculo preciso**: Considera ingresos objetivo, gastos personales y operativos
- 🕐 **Personalizable**: Configura tu jornada laboral (horas/día, días/semana)
- 📈 **Resultados detallados**: Tarifa por hora, tarifa semanal e ingreso mensual necesario
- 🎓 **Tutorial interactivo**: Guía paso a paso para nuevos usuarios
- 💾 **Sin base de datos**: No requiere registro ni almacena datos personales
- 🎨 **Diseño moderno**: Interfaz limpia con animaciones suaves
- 📱 **Responsive**: Funciona perfectamente en móviles, tablets y escritorio
- 🆓 **100% Gratuita**: De código abierto y libre para usar

## 🚀 Instalación

### Opción 1: Instalación local (para desarrollo)

1. **Clona o descarga el repositorio**
   ```bash
   git clone https://github.com/mjpb-projects/calculadora-tarifa-hora.git
   cd calculadora-tarifa-hora
   ```

2. **Abre el archivo en tu navegador**
   - Simplemente abre el archivo `index.html` en tu navegador web favorito
   - No requiere servidor web ni dependencias adicionales
   - **Navegadores compatibles**: Chrome, Firefox, Safari, Edge (versiones modernas)

### Opción 2: Instalación en hosting web

#### Hosting compartido (cPanel, DirectAdmin, etc.)

1. **Accede a tu panel de control**
   - Inicia sesión en tu hosting (cPanel, Plesk, etc.)

2. **Ubica el administrador de archivos**
   - Busca "File Manager" o "Administrador de archivos"
   - Navega a la carpeta `public_html` o `www`

3. **Sube el archivo**
   - Haz clic en "Upload" o "Subir"
   - Selecciona el archivo `index.html`
   - Espera a que termine la carga

4. **Accede a tu aplicación**
   - Visita: `http://tu-dominio.com/index.html`
   - O renombra el archivo a `index.html` en la raíz para acceder con: `http://tu-dominio.com`

#### Netlify (Gratuito y recomendado)

1. **Crea una cuenta en Netlify**
   - Visita [netlify.com](https://www.netlify.com)
   - Regístrate gratis con GitHub, GitLab o email

2. **Sube tu proyecto**
   - Arrastra la carpeta del proyecto a Netlify
   - O conecta tu repositorio de GitHub

3. **¡Listo!**
   - Netlify generará una URL automáticamente
   - Ejemplo: `https://tu-app.netlify.app`

#### Vercel (Gratuito)

1. **Crea una cuenta en Vercel**
   - Visita [vercel.com](https://vercel.com)
   - Regístrate con GitHub, GitLab o Bitbucket

2. **Importa el proyecto**
   ```bash
   npm i -g vercel
   vercel
   ```

3. **Sigue las instrucciones**
   - Vercel detectará automáticamente la configuración
   - Tu app estará disponible en una URL de Vercel

#### GitHub Pages (Gratuito)

1. **Sube tu proyecto a GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/tu-usuario.github.io.git
   git push -u origin main
   ```

2. **Activa GitHub Pages**
   - Ve a Settings → Pages
   - En "Source" selecciona "main branch"
   - Guarda los cambios

3. **Accede a tu aplicación**
   - Tu app estará en: `https://tu-usuario.github.io/calculadora-tarifa-hora/`

### Opción 3: Servidor local con Python (para pruebas)

```bash
# Python 3
python -m http.server 8000

# Luego abre en tu navegador
# http://localhost:8000
```

### Opción 4: Servidor local con Node.js

```bash
# Instala http-server globalmente
npm install -g http-server

# Ejecuta el servidor
http-server

# Abre en tu navegador
# http://localhost:8080
```

## 📖 Cómo usar la aplicación

### Primer uso: Tutorial interactivo

La primera vez que abras la aplicación, verás un tutorial interactivo que te guiará a través de las funcionalidades principales.

**Ver captura:** [tutorial/screenshots/01-tutorial-bienvenida.png](tutorial/screenshots/01-tutorial-bienvenida.png)
- *Muestra el modal de bienvenida con los 4 pasos del tutorial*

Si necesitas volver a ver el tutorial, simplemente haz clic en el botón de ayuda (ícono de interrogación) en la esquina inferior derecha.

### Paso 1: Define tu ingreso objetivo

Ingresa la información financiera básica:

1. **Ingreso objetivo mensual**: Cuánto deseas ganar al mes (neto)
2. **Gastos personales mensuales**: Tus gastos de vida (renta, comida, servicios, etc.)

**Ver captura:** [tutorial/screenshots/02-ingresos-gastos-personales.png](tutorial/screenshots/02-ingresos-gastos-personales.png)
- *Muestra la sección "Ingresos y Gastos Personales" con los campos completados*
- *Ejemplo: Ingreso objetivo: $5,000 | Gastos personales: $2,000*

### Paso 2: Agrega tus gastos operativos

Especifica los costos relacionados con tu trabajo:

1. **¿Trabajas desde casa?**
   - Marca esta casilla si trabajas remotamente
   - Si está marcada, el campo de transporte se ocultará automáticamente

2. **Gasto mensual en transporte**
   - Solo visible si NO trabajas desde casa
   - Incluye gasolina, transporte público, estacionamiento, etc.

3. **Herramientas y equipos**
   - Depreciación de equipo, reparaciones, reemplazos
   - Ejemplo: computadora, cámara, micrófono, etc.

4. **Software y suscripciones**
   - Licencias, SaaS, herramientas en línea
   - Ejemplo: Adobe, Microsoft 365, Canva Pro, etc.

5. **Internet y servicios**
   - Conexión a internet, telefonía, hosting, etc.

6. **Otros gastos operativos**
   - Cualquier otro gasto relacionado con tu trabajo
   - Ejemplo: coworking, electricidad adicional, café, etc.

**Ver captura:** [tutorial/screenshots/03-gastos-operativos.png](tutorial/screenshots/03-gastos-operativos.png)
- *Muestra la sección "Gastos Operativos" completa*
- *Muestra el checkbox "Trabajo desde casa" activado (campo de transporte oculto)*
- *Ejemplo de valores en: Herramientas: $150, Software: $100, Internet: $50, Otros: $100*

**Ver captura alternativa:** [tutorial/screenshots/03b-gastos-operativos-transporte.png](tutorial/screenshots/03b-gastos-operativos-transporte.png)
- *Muestra la misma sección pero con "Trabajo desde casa" desactivado*
- *Campo de transporte visible con ejemplo: $300*

### Paso 3: Configura tu jornada laboral

Define cuánto tiempo trabajarás:

1. **Horas de trabajo al día**
   - Ejemplo: 8 horas (jornada completa)
   - Acepta decimales: 6.5, 7.5, etc.

2. **Días de trabajo a la semana**
   - Ejemplo: 5 días (lunes a viernes)
   - Rango: 1-7 días

**Ver captura:** [tutorial/screenshots/04-jornada-laboral.png](tutorial/screenshots/04-jornada-laboral.png)
- *Muestra la sección "Jornada Laboral"*
- *Ejemplo: 8 horas/día, 5 días/semana*
- *Muestra el botón "Calcular mi tarifa" destacado*

### Paso 4: Obtén tus resultados

Haz clic en el botón **"Calcular mi tarifa"** y obtendrás:

#### Resultados principales (tarjetas destacadas)

1. **Tarifa por hora** 💰
   - Cuánto debes cobrar por cada hora de trabajo
   - Incluye todos tus gastos e ingreso objetivo

2. **Tarifa semanal** 📅
   - Tus ingresos semanales esperados
   - Basado en tu jornada laboral configurada

3. **Ingreso mensual necesario** 📊
   - Total que necesitas ganar al mes
   - Suma de ingreso objetivo + todos los gastos

**Ver captura:** [tutorial/screenshots/05-resultados-principales.png](tutorial/screenshots/05-resultados-principales.png)
- *Muestra las 3 tarjetas de resultados principales con valores calculados*
- *Ejemplo: Tarifa por hora: $43.29 | Tarifa semanal: $1,731.79 | Ingreso mensual: $7,500*

#### Desglose detallado

Una tabla con el desglose completo de todos tus gastos:
- Cada concepto con su monto
- Total requerido mensual
- Resumen de tu jornada laboral (horas/semana y horas/mes)

**Ver captura:** [tutorial/screenshots/06-desglose-detallado.png](tutorial/screenshots/06-desglose-detallado.png)
- *Muestra la tabla "Desglose de gastos" completa*
- *Incluye todos los conceptos y el total resaltado*
- *Muestra el cálculo de horas al final de la tabla*

### Funciones adicionales

#### Recalcular
- Simplemente modifica cualquier valor y haz clic en "Calcular mi tarifa" nuevamente
- Los resultados se actualizarán instantáneamente

#### Ver tutorial nuevamente
- Haz clic en el botón de ayuda (❓) en la esquina inferior derecha
- Se abrirá el tutorial completo

**Ver captura:** [tutorial/screenshots/07-boton-ayuda.png](tutorial/screenshots/07-boton-ayuda.png)
- *Muestra el botón flotante de ayuda en la esquina inferior derecha*

### Validaciones automáticas

La aplicación valida automáticamente:
- ✅ Que hayas ingresado horas por día válidas (> 0)
- ✅ Que hayas ingresado días por semana válidos (> 0)
- ✅ Que hayas ingresado un ingreso objetivo (> 0)

Si falta algún dato importante, recibirás una alerta indicándote qué necesitas completar.

**Ver captura:** [tutorial/screenshots/08-validacion-error.png](tutorial/screenshots/08-validacion-error.png)
- *Muestra una alerta de validación pidiendo completar campos requeridos*

### Responsive Design

La aplicación se adapta perfectamente a cualquier dispositivo:
- 💻 **Desktop**: Vista completa con grid de 2 columnas
- 📱 **Móvil**: Vista de 1 columna optimizada para pantallas pequeñas
- 📱 **Tablet**: Vista adaptativa según orientación

**Ver capturas:** 
- [tutorial/screenshots/09-responsive-desktop.png](tutorial/screenshots/09-responsive-desktop.png) - *Vista en desktop*
- [tutorial/screenshots/10-responsive-mobile.png](tutorial/screenshots/10-responsive-mobile.png) - *Vista en móvil*

## 🎯 Casos de uso

### Freelancer diseñador gráfico
```
Ingreso objetivo: $3,000
Gastos personales: $1,500
Trabajo desde casa: ✓
Software (Adobe): $60
Internet: $40
Otros (electricidad): $30
Jornada: 6 horas/día, 5 días/semana
→ Tarifa: $36.15/hora
```

### Desarrollador web independiente
```
Ingreso objetivo: $5,000
Gastos personales: $2,000
Transporte: $200
Coworking: $150
Software (GitHub, hosting): $100
Internet: $50
Equipo: $100
Jornada: 8 horas/día, 5 días/semana
→ Tarifa: $43.29/hora
```

### Consultor de marketing
```
Ingreso objetivo: $4,000
Gastos personales: $1,800
Transporte: $300
Software (Semrush, Canva): $150
Internet y móvil: $80
Materiales: $70
Jornada: 7 horas/día, 4 días/semana
→ Tarifa: $52.32/hora
```

## 🛠️ Tecnologías utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Diseño moderno con animaciones
- **JavaScript (Vanilla)**: Lógica de cálculo y interactividad
- **Google Fonts**: Tipografía Google Sans
- **Material Icons**: Iconografía de Google
- **LocalStorage**: Para recordar si el usuario ya vio el tutorial

## 🎨 Personalización

### Cambiar colores

Edita las variables CSS en el archivo `index.html` (líneas 19-32):

```css
:root {
    --primary: #6497F7;        /* Color principal */
    --primary-dark: #4a7de8;   /* Variante oscura */
    --primary-light: #e8f0fe;  /* Variante clara */
    /* ... más colores ... */
}
```

### Cambiar tipografía

1. Busca otra fuente en [Google Fonts](https://fonts.google.com)
2. Reemplaza el enlace de Google Sans (línea 11)
3. Actualiza la familia de fuentes en CSS (línea 47)

### Modificar el logo

Cambia el ícono del logo editando la línea 492:
```html
<span class="material-icons-round">payments</span>
```

Busca otros íconos en: [Google Material Icons](https://fonts.google.com/icons)

## 📂 Estructura del proyecto

```
calculadora-tarifa-hora/
│
├── index.html              # Aplicación completa (HTML + CSS + JS)
├── README.md              # Este archivo
│
└── tutorial/
    └── screenshots/       # Capturas de pantalla para documentación
        ├── 01-tutorial-bienvenida.png
        ├── 02-ingresos-gastos-personales.png
        ├── 03-gastos-operativos.png
        ├── 03b-gastos-operativos-transporte.png
        ├── 04-jornada-laboral.png
        ├── 05-resultados-principales.png
        ├── 06-desglose-detallado.png
        ├── 07-boton-ayuda.png
        ├── 08-validacion-error.png
        ├── 09-responsive-desktop.png
        └── 10-responsive-mobile.png
```

## ❓ FAQ (Preguntas Frecuentes)

### ¿Por qué mi tarifa parece alta?
La calculadora incluye TODOS tus gastos (personales + operativos) más tu ingreso objetivo. Esto asegura que cubras todos tus costos y ahorres.

### ¿Puedo usar esta tarifa directamente con mis clientes?
Sí, pero considera factores adicionales como:
- Competencia en tu mercado
- Nivel de experiencia
- Valor que aportas al cliente
- Urgencia del proyecto

### ¿Los datos se guardan en algún lugar?
No. La aplicación NO guarda datos personales ni financieros. Solo guarda en LocalStorage si ya viste el tutorial.

### ¿Puedo modificar el código?
¡Por supuesto! Es código abierto. Siéntete libre de personalizar, mejorar y compartir.

### ¿Funciona offline?
Sí, una vez cargada la página. Solo necesita internet inicialmente para cargar las fuentes e íconos de Google.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar esta herramienta:

1. Haz fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

Eres libre de:
- ✅ Usar comercialmente
- ✅ Modificar
- ✅ Distribuir
- ✅ Uso privado

Solo se requiere:
- 📄 Incluir la licencia y copyright original

## 📧 Soporte

Si encuentras algún bug o tienes sugerencias:
- Abre un issue en GitHub
- Envía un pull request
- Comparte tu feedback

## 🌟 Créditos

**Desarrollado por:** Miguel Páez.

**Tecnologías y recursos utilizados:**
- [Google Fonts](https://fonts.google.com) - Tipografía Google Sans
- [Google Material Icons](https://fonts.google.com/icons) - Iconografía
- Diseñado con atención al detalle para freelancers y profesionales independientes

**Inspiración:**
- Comunidad de freelancers y trabajadores independientes
- Necesidad de herramientas gratuitas y accesibles para establecer precios justos

---

💼 **¿Te resultó útil?** Dale una ⭐ al proyecto y compártelo con otros profesionales independientes.

📢 **Comparte en redes sociales** usando el hashtag #CalculadoraTarifaPorHora

🚀 **Desarrollado con cariño para la comunidad freelance**
