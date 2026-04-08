# 🌐 Plantillas ISP - Notificaciones de Servicio

Conjunto profesional de plantillas HTML para **Proveedores de Internet (ISP)** que permite notificar a clientes sobre suspensiones de servicio y recordatorios de pago.

## ✨ Características

- 📱 **100% Responsivo** - Funciona perfectamente en cualquier dispositivo
- 🎨 **Fácil de personalizar** - Cambios simples sin necesidad de conocimientos avanzados
- 🚀 **Ligero y rápido** - Sin dependencias externas, solo HTML/CSS puro
- 🔐 **Seguro** - Sin scripts maliciosos, código limpio
- 📧 **Compatible con email** - Ideal para envíos masivos
- 🌍 **Multiidioma** - Ejemplos en español, inglés, portugués

## 📂 Contenido del Proyecto

```
uispdue/
├── 📄 index.html                 → Plantilla: Servicio Suspendido (rojo)
├── 📄 reminder.html              → Plantilla: Recordatorio de Pago (amarillo)
├── 🎨 EJEMPLOS_PERSONALIZACION.md → 10 ejemplos prácticos
├── 📖 INDICE.md                  → Navegación de documentación
├── 📋 README.md                  → Este archivo
└── 📁 example/                   → Imágenes y recursos de ejemplo
```

## 🚀 Inicio Rápido

### Opción 1: Ver en el navegador
```bash
1. Abre index.html en tu navegador
2. O abre reminder.html
3. ¡Listo! Verás la plantilla en acción
```

### Opción 2: Editar localmente
```bash
1. Abre cualquier archivo HTML con tu editor favorito (VS Code, Sublime, etc)
2. Realiza tus cambios
3. Guarda (Ctrl+S / Cmd+S)
4. Recarga el navegador (F5)
```

### Opción 3: Servir localmente
```bash
# Con Python
python -m http.server 8000

# Con Node.js
npx http-server
```


## 🎯 Plantillas Disponibles

### 1️⃣ Recordatorio de Pago (`reminder.html`)
- **Color:** Amarillo `#fec901`
- **Uso:** Recordar a clientes que deben pagar
- **Ícono:** Símbolo de riesgo/advertencia
- **Tono:** Amistoso pero formal

### 2️⃣ Servicio Suspendido (`index.html`)
- **Color:** Rojo
- **Uso:** Notificar suspensión de servicio
- **Ícono:** WiFi desconectado
- **Tono:** Urgente pero profesional

## 💡 Casos de Uso

✅ Notificaciones para clientes de ISP  
✅ Recordatorios de pago automáticos  
✅ Avisos de suspensión de servicio  
✅ Emails transaccionales  
✅ Portales de cliente  
✅ Sistemas de notificación web  
✅ Landing pages de ISP  

## 🎨 Personalización Básica

### Cambiar el título
```html
<!-- Busca esta línea -->
<h1>SERVICIO SUSPENDIDO</h1>

<!-- Cámbiala por esto -->
<h1>TU TITULO AQUI</h1>
```

### Cambiar el color del título
```css
/* Busca esta sección en <style> */
h1 {
  color: red;  /* Rojo para index.html */
  /* o */
  color: #fec901;  /* Amarillo para reminder.html */
}

/* Cámbialo por tu color preferido */
h1 {
  color: #0066cc;  /* Azul por ejemplo */
}
```

### Cambiar el mensaje
```html
<!-- Busca este párrafo -->
<p align="justify">
  Te recordamos que los pagos del servicio de internet son de 1 al 7 de cada mes.
</p>

<!-- Cámbialo por tu mensaje -->
<p align="justify">
  Tu mensaje personalizado aquí...
</p>
```

## 📱 Responsividad

Las plantillas se adaptan automáticamente a:
- 📱 Móviles (320px - 480px)
- 📱 Tablets (481px - 760px)
- 💻 Escritorio (760px+)

Prueba en tu navegador:
1. Abre DevTools (F12)
2. Haz clic en el ícono de dispositivo móvil
3. Selecciona diferentes tamaños

## 🔧 Personalización Avanzada

- 🎨 [EJEMPLOS_PERSONALIZACION.md](/example/EJEMPLOS_PERSONALIZACION.md/) → 10 ejemplos completos

Ejemplos incluyen:
- Dark mode premium
- Con logo de empresa
- Con información de contacto
- Con métodos de pago
- Versión multiidioma
- Con código QR
- Versión corporativa profesional
- Y más...

## 🌐 Integración con Servidores

### Backend (Node.js)
```javascript
const fs = require('fs');
let html = fs.readFileSync('reminder.html', 'utf-8');
// Personalizar con datos dinámicos
html = html.replace('{{cliente}}', 'Juan Pérez');
res.send(html);
```

### Backend (PHP)
```php
$html = file_get_contents('reminder.html');
$html = str_replace('{{cliente}}', 'Juan Pérez', $html);
echo $html;
```

Más detalles en [DOCUMENTACION.md](DOCUMENTACION.md) → "Integración con Servidores"

## 📧 Envío por Email

Las plantillas son 100% compatibles con email HTML:
1. Cambia rutas de imágenes a URLs absolutas
2. Usa atributos `style` inline si es necesario
3. Test en [Litmus](https://litmus.com) o [Email on Acid](https://www.emailonacid.com)

## 🎓 Ejemplos Rápidos

Tenemos 10 ejemplos listos para copiar y pegar en [EJEMPLOS_PERSONALIZACION.md](/example/EJEMPLOS_PERSONALIZACION.md):

1. ✅ Español Latinoamericano
2. ✅ Dark Mode Premium
3. ✅ Con Logo de Empresa
4. ✅ Con Información de Contacto
5. ✅ Con Métodos de Pago
6. ✅ Con Cuenta Regresiva
7. ✅ Versión Multiidioma
8. ✅ Con Código QR
9. ✅ Versión Corporativa
10. ✅ Con Historial de Pagos



## 📝 Historial de Cambios

- **v1.0** (2026-04-08) - Versión inicial con documentación completa

## 📄 Licencia

Libre para usar, modificar y distribuir en proyectos personales y comerciales.

## 🤝 Contribuciones

¿Tienes mejoras o sugerencias? Estamos abiertos a feedback.
