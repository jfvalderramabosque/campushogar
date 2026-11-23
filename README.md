 CampusHogar

Prototipo funcional de una aplicación móvil que conecta a estudiantes de la Universidad El Bosque que llegan de otras ciudades con arrendadores cercanos al campus en Bogotá. Reemplaza el codeudor con finca raíz por un score de confianza basado en verificaciones.

Prototipo en línea: https://jfvalderramabosque.github.io/campushogar/

> Proyecto de Innovación Tecnológica · Gestión de Tecnología e Innovación · Universidad El Bosque · 2026-2

 Equipo

- Caren Sofia Bustamante Castellanos
- Alejandra Valenttina Ramírez Chacón
- Juan Felipe Valderrama Peñaloza

Docente: Carlos Hernan Medina Ayala

 Qué hace

Estudiante
- Registro con correo institucional y verificación de identidad (correo, carné por foto o NFC, selfie, acudiente).
- Explorar inmuebles en lista o mapa, con filtros de precio, distancia, tipo, alcobas, baños, amoblado, servicios, comodidades, contrato mínimo, disponibilidad, verificación y score del arrendador.
- Detalle del inmueble: galería, costos, compatibilidad con el arrendador, reseñas y enlaces a Google Maps.
- Chat con el arrendador (los datos de contacto se ocultan hasta aceptar el arriendo).
- Agendar visitas con check-in por NFC.
- Solicitud, decisión del arrendador, codeudor o acudiente, firma del contrato, registro del acuerdo, finalización y calificación mutua.

Arrendador
- Publicar inmuebles con asistente de 3 pasos.
- Verificar la ubicación con foto geolocalizada: hasta 50 m queda verificada, de 51 a 150 m va a revisión manual y más de 150 m se rechaza.
- Activar etiqueta NFC en la puerta, definir su umbral de confianza, atender solicitudes y visitas, firmar contratos y calificar.

 Score de confianza

| Rol | Componente | Puntos |
|---|---|---|
| Estudiante | Correo institucional | 15 |
| | Carné estudiantil | 20 |
| | Selfie frente al documento | 25 |
| | Acudiente verificado | 15 |
| | Reseñas de arriendos | 25 |
| Arrendador | Cédula | 20 |
| | Selfie frente a la cédula | 20 |
| | Documento del inmueble | 15 |
| | Inmueble verificado por GPS | 25 |
| | Reseñas de arriendos | 20 |

 Cómo probarlo

1. Abre el enlace del prototipo (funciona en el navegador, mejor en el celular).
2. Usa Acceso rápido para entrar como estudiante o arrendador, o crea una cuenta.
3. Recorrido sugerido: explorar y filtrar, abrir un inmueble, escribir, agendar visita, solicitar, firmar el contrato y calificar. Luego entra como arrendador y publica un inmueble: prueba la verificación de ubicación con 20, 100 y 200 m.

Para ejecutarlo localmente basta abrir `index.html` en el navegador. No requiere instalación ni servidor.

 Alcance y limitaciones

Es un prototipo de validación de concepto, sin backend:

- Los datos viven solo en el navegador (`localStorage`); no se comparten entre dispositivos.
- Son simulados: OCR, biometría, lectura NFC, el GPS (opcional del equipo), los mapas esquemáticos, las fotos de los inmuebles (ilustraciones generadas), las respuestas de arrendadores y estudiantes, la firma del contrato y los pagos.
- Los inmuebles, arrendadores, direcciones y reseñas son datos sintéticos.
- La contraseña usa un hash simple de demostración; una versión real requiere servidor y bcrypt o similar.
- El contrato es una plantilla que deja trazabilidad; no equivale a una firma electrónica con plena validez legal.

 Tecnología

HTML, CSS y JavaScript sin dependencias, en un solo archivo (`index.html`). Tipografía Plus Jakarta Sans de Google Fonts.

 Declaración de uso de IA generativa

Se usó Claude (Anthropic) como apoyo para desarrollar el prototipo. El equipo definió el concepto, los requisitos y las reglas de negocio, y revisó y probó el resultado.
