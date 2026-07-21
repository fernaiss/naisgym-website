# Borrador de inventario para Data Safety (revisar contra el AAB final)

Este documento NO se sube como política. Es una guía para completar Play Console.

Datos probablemente recopilados:
- Dirección de correo electrónico: funcionalidad de cuenta, asociado al usuario.
- Identificador de usuario: funcionalidad y seguridad, asociado al usuario.
- Datos de fitness: rutinas, entrenamientos, series, repeticiones, peso utilizado.
- Información de salud/bienestar introducida por el usuario: peso y medidas corporales.
- Fotografías: fotos de progreso opcionales.
- Compras: estado del producto/beneficio y datos técnicos de validación; el pago lo procesa Google Play.
- Preferencias de la app.

Finalidades:
- Funcionalidad de la app.
- Gestión de cuenta.
- Personalización.
- Prevención de fraude/seguridad.
- Soporte y diagnóstico, solo si realmente se recopila.

Seguridad:
- Datos cifrados en tránsito: marcar Sí solo después de verificar HTTPS/TLS en todos los servicios.
- Eliminación disponible: Sí.
- Solicitud web: URL /delete-account/.

Compartición:
- No marcar “no se comparte” automáticamente sin revisar la definición de Google y cada SDK.
- Revisar Supabase, Google Play Billing y cualquier SDK de analítica, crash reporting, notificaciones o publicidad.
- Si Firebase Analytics, Crashlytics, AdMob u otro SDK existe en el AAB final, actualizar la declaración.

Importante:
La declaración debe coincidir con el comportamiento real del AAB publicado, no solo con la intención del proyecto.
