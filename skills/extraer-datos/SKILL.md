---
name: extraer-datos
description: Extrae información del negocio desde fotos, PDFs, capturas de pantalla o descripciones del usuario para preparar la generación de publicidad
user-invocable: true
---

# Skill: Extraer Datos del Negocio

Usa esta skill cuando el usuario suba una imagen, foto, PDF, captura de WhatsApp Business, volante, carta de menú, o describa su negocio con sus propias palabras.

## Cuándo activar esta skill

- El usuario sube una foto o imagen de su negocio
- El usuario sube un PDF (carta, menú, volante, ficha)
- El usuario dice "te paso mi carta", "mira mi volante", "te mando foto de mi local"
- El usuario describe su negocio sin estructura clara

## Qué extraer

Busca esta información en el archivo o descripción:

- Nombre: nombre del negocio, marca, logo, letrero
- Rubro: tipo de negocio (restaurante, ropa, servicios, etc.)
- Producto: qué vende o qué servicio ofrece
- Público: a quién va dirigido si se puede inferir
- Oferta: promociones, precios, descuentos mencionados
- Contacto: teléfono, WhatsApp, dirección, redes sociales
- Horario: si aparece el horario de atención

## Cómo entregar el resultado

✅ Datos extraídos de tu negocio:

- 🏪 Nombre: [nombre encontrado]
- 🏷 Rubro: [rubro]
- 📦 Producto/Servicio: [descripción]
- 👥 Público: [público objetivo]
- 🎯 Oferta: [promoción si hay]
- 📞 Contacto: [si aparece]

Luego pregunta:
"¿Están bien estos datos? ¿Quieres cambiar o agregar algo antes de generar tu publicidad?"

## Si falta información importante

Si no puedes extraer el nombre o el producto pregunta:
"Vi tu archivo pero necesito confirmar: ¿cuál es el nombre exacto de tu negocio y qué es lo que más quieres promocionar?"

## Después de confirmar los datos

Una vez que el usuario confirme, pregunta:
"¡Perfecto! ¿Para qué canales quieres los anuncios? (Facebook, Instagram, WhatsApp, TikTok, Email, Cartel) ¿Y qué tono prefieres: amigable, profesional, urgente o divertido?"

Luego activa la skill generar-copy con los datos confirmados.

## Reglas

- NUNCA inventes datos que no estén en el archivo o descripción
- Si un campo no aparece, déjalo en blanco y pregunta
- Siempre confirma con el usuario antes de generar publicidad
