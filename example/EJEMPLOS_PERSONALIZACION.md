# 🎨 Ejemplos de Personalización

## 📌 Introducción

Este archivo muestra ejemplos prácticos de cómo modificar las plantillas para diferentes casos de uso.

---

## 1️⃣ Ejemplo: Cambiar a Español Latinoamericano

### reminder.html - Versión MX/AR

```html
<p class='client'>Estimado cliente de TuISP</p>
<p align="justify">
  <br>
  Te recordamos que los pagos del servicio de internet deben realizarse <strong>del 1 al 10 de cada mes</strong>.
  <br>
  Si no cuentas con tu factura, puedes descargarla desde tu panel de cliente.
  <br/>
</p>
<div class="message">
  Gracias por ser parte de nuestra familia.
  <br />
  <p class='client'>El equipo de TuISP</p>
</div>
```

---

## 2️⃣ Ejemplo: Versión Premium (Dark Mode)

### Modificar CSS para Dark Mode

```css
body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: linear-gradient(135deg, #1e1e1e 0%, #2d2d2d 100%);
}

.container {
  background: linear-gradient(135deg, #2d2d2d 0%, #1e1e1e 100%);
  padding: 40px;
  border-radius: 15px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.5);
  border: 1px solid #444;
  display: flex;
  flex-direction: column;
  align-items: center;
}

p {
  font-size: 16px;
  color: #e0e0e0;
}

h1 {
  color: #fec901;
  text-shadow: 0 0 20px rgba(254, 201, 1, 0.5);
}
```

---

## 3️⃣ Ejemplo: Agregar Logo de Empresa

### Modificar index.html

```html
<div class="container">
  <!-- NUEVO: Logo empresa -->
  <div class="logo">
    <img src="example/logo-empresa.png" alt="Logo de TuISP" />
  </div>
  
  <div class="icon">
    <!-- SVG icon -->
  </div>
  
  <!-- ... resto del contenido -->
</div>
```

### CSS para Logo

```css
.logo {
  margin-bottom: 20px;
  text-align: center;
}

.logo img {
  max-width: 120px;
  height: auto;
  border-radius: 10px;
}
```

---

## 4️⃣ Ejemplo: Información de Contacto

### Agregar datos de contacto

```html
<main>
  <p class='client'>Estimado cliente</p>
  <p align="justify">
    Tu servicio ha sido suspendido por falta de pago.
  </p>
  
  <!-- NUEVO: Información de contacto -->
  <div class="contact-info">
    <h3>¿Necesitas ayuda?</h3>
    <p>📞 <strong>Teléfono:</strong> +1 (555) 123-4567</p>
    <p>📧 <strong>Email:</strong> soporte@tuisp.com</p>
    <p>🌐 <strong>Web:</strong> www.tuisp.com</p>
    <p>💬 <strong>Chat:</strong> Sistema de chat disponible 24/7</p>
  </div>
</main>
```

### CSS para Contacto

```css
.contact-info {
  background-color: #f9f9f9;
  border-left: 4px solid #fec901;
  padding: 15px;
  margin: 20px 0;
  border-radius: 5px;
}

.contact-info h3 {
  color: #000;
  margin-top: 0;
}

.contact-info p {
  margin: 8px 0;
  font-size: 14px;
}
```

---

## 5️⃣ Ejemplo: Método de Pago

### Agregar opciones de pago

```html
<main>
  <p class='client'>Estimado cliente</p>
  <p align="justify">
    Realiza tu pago antes del 7 de cada mes a través de:
  </p>
  
  <!-- NUEVO: Métodos de pago -->
  <div class="payment-methods">
    <div class="method">
      <h4>💳 Tarjeta de Crédito/Débito</h4>
      <p>Panel de control: www.tuisp.com/pagar</p>
    </div>
    <div class="method">
      <h4>🏦 Transferencia Bancaria</h4>
      <p>Banco: Banco Nacional | Cuenta: 123456789</p>
    </div>
    <div class="method">
      <h4>💰 Efectivo</h4>
      <p>En nuestras oficinas: Calle Principal 123</p>
    </div>
  </div>
</main>
```

### CSS para Métodos de Pago

```css
.payment-methods {
  display: grid;
  grid-template-columns: 1fr;
  gap: 15px;
  margin: 20px 0;
}

.method {
  background: #f0f0f0;
  padding: 15px;
  border-radius: 8px;
  border-left: 4px solid #fec901;
}

.method h4 {
  margin: 0 0 10px 0;
  color: #000;
}

.method p {
  margin: 0;
  font-size: 14px;
}

@media (max-width: 760px) {
  .payment-methods {
    grid-template-columns: 1fr;
  }
}
```

---

## 6️⃣ Ejemplo: Con Cuenta Regresiva

### Agregar contador de días hasta suspensión

```html
<main>
  <p class='client'>Estimado cliente</p>
  <p align="justify">
    <strong>⚠️ CUENTA REGRESIVA:</strong> 
    Tu servicio será suspendido en <span class='countdown'>3 días</span>
  </p>
  <p align="justify">
    Por favor realiza tu pago antes de que venza el plazo.
  </p>
</main>
```

### CSS para Countdown

```css
.countdown {
  display: inline-block;
  background-color: #ff6b6b;
  color: white;
  padding: 5px 10px;
  border-radius: 5px;
  font-weight: bold;
  animation: pulse 1.5s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.7; }
}
```

---

## 7️⃣ Ejemplo: Versión Multiidioma

### Crear variantes de idioma

```html
<!-- ÍNDICE DE IDIOMAS -->
<!-- 
  - Spanish: reminder.html
  - English: reminder-en.html
  - Portuguese: reminder-pt.html
-->

<!-- reminder-en.html -->
<h1>PAYMENT REMINDER</h1>
<p class='client'>Dear Valued Customer</p>
<p align="justify">
  We remind you that internet service payments must be made between the 1st and 7th of each month.
</p>

<!-- reminder-pt.html -->
<h1>LEMBRETE DE PAGAMENTO</h1>
<p class='client'>Estimado Cliente</p>
<p align="justify">
  Lembramos que os pagamentos do serviço de internet devem ser realizados entre os dias 1 e 7 de cada mês.
</p>
```

---

## 8️⃣ Ejemplo: Con QR para Pago

### Agregar código QR

```html
<main>
  <p class='client'>Estimado cliente</p>
  <p align="justify">
    Escanea este código QR para realizar tu pago:
  </p>
  
  <!-- NUEVO: QR Code -->
  <div class="qr-container">
    <img src="example/qr-pago.png" alt="QR para pago" class="qr-code" />
    <p class="qr-text">Escanea con tu celular</p>
  </div>
</main>
```

### CSS para QR

```css
.qr-container {
  margin: 20px 0;
  text-align: center;
}

.qr-code {
  width: 150px;
  height: 150px;
  padding: 10px;
  background-color: #f9f9f9;
  border: 2px solid #ddd;
  border-radius: 8px;
}

.qr-text {
  font-size: 12px;
  color: #666;
  margin-top: 10px;
}
```

---

## 9️⃣ Ejemplo: Versión Corporativa

### Plantilla profesional con franja corporativa

```html
<!DOCTYPE HTML>
<html>
<head>
  <meta charset="UTF-8" />
  <title>Notificación - TuISP</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 20px;
      background: linear-gradient(to right, #2c3e50, #3498db);
      min-height: 100vh;
    }

    .header-bar {
      background: linear-gradient(to right, #e74c3c, #c0392b);
      color: white;
      padding: 20px;
      text-align: center;
      border-radius: 8px 8px 0 0;
      font-size: 18px;
      font-weight: bold;
    }

    .container {
      background-color: #fff;
      max-width: 600px;
      margin: 0 auto;
      border-radius: 8px;
      box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
      overflow: hidden;
    }

    .content {
      padding: 30px;
    }

    .footer-bar {
      background: #34495e;
      color: white;
      padding: 15px;
      text-align: center;
      font-size: 12px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header-bar">⚠️ SERVICIO SUSPENDIDO</div>
    <div class="content">
      <h2 style="color: #e74c3c;">Estimado cliente</h2>
      <p>Tu servicio ha sido suspendido por falta de pago.</p>
      <!-- contenido -->
    </div>
    <div class="footer-bar">© 2026 TuISP - Todos los derechos reservados</div>
  </div>
</body>
</html>
```

---

## 🔟 Ejemplo: Con Historial de Pagos

### Mostrar historial reciente

```html
<main>
  <p class='client'>Estimado cliente</p>
  
  <!-- NUEVO: Historial de pagos -->
  <div class="payment-history">
    <h3>📋 Historial de Pagos Recientes</h3>
    <table style="width: 100%; border-collapse: collapse;">
      <tr>
        <th style="border-bottom: 1px solid #ddd; padding: 8px;">Mes</th>
        <th style="border-bottom: 1px solid #ddd; padding: 8px;">Estado</th>
      </tr>
      <tr>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">Marzo 2026</td>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">✅ Pagado</td>
      </tr>
      <tr>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">Abril 2026</td>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">❌ Pendiente</td>
      </tr>
      <tr>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">Mayo 2026</td>
        <td style="border-bottom: 1px solid #ddd; padding: 8px;">⏳ Por vencer</td>
      </tr>
    </table>
  </div>
</main>
```

---

## 🎯 Resumen de Ejemplos

| Ejemplo | Caso de Uso | Dificultad |
|---------|-----------|-----------|
| 1. Español LAT | Localización | ⭐ Fácil |
| 2. Dark Mode | Estética moderna | ⭐⭐ Media |
| 3. Logo empresa | Branding | ⭐ Fácil |
| 4. Contacto | Soporte cliente | ⭐⭐ Media |
| 5. Métodos pago | E-commerce | ⭐⭐ Media |
| 6. Countdown | Urgencia | ⭐⭐ Media |
| 7. Multiidioma | Internacional | ⭐⭐⭐ Avanzado |
| 8. QR Code | Mobile-first | ⭐ Fácil |
| 9. Corporativo | Profional | ⭐⭐ Media |
| 10. Historial | Analytics | ⭐⭐⭐ Avanzado |

---

## 💡 Tips de Combinación

Puedes combinar múltiples ejemplos:

```html
<!-- Combinar: Logo + Dark Mode + QR + Contacto -->
<body style="background: linear-gradient(135deg, #1e1e1e, #2d2d2d);">
  <div class="container" style="background: #2d2d2d; color: #e0e0e0;">
    <!-- Logo pequeño aquí -->
    <!-- Dark mode styling -->
    <!-- QR code -->
    <!-- Contacto info -->
  </div>
</body>
```

---

**¡Elige tus ejemplos favoritos y personaliza!** 🎨
