Un preset es una “plantilla de tirada” que guarda tu configuración para usarla en 1 clic más tarde.

Qué guarda exactamente

Los dados y cantidades (p. ej., 2×D6, 1×D20…)

El modificador actual (p. ej., +2 / −1)

El modo: Normal, Ventaja o Desventaja (aplica al D20)

Para qué sirve

Evitas reconfigurar cada vez tiradas típicas como “Ataque” o “Iniciativa”.

En tu próxima tirada, eliges el preset y lo aplicas, y ya puedes Lanzar.

Cómo se usa

Configura los dados, el modificador y (si quieres) ventaja/desventaja.

Escribe un nombre en “Guardar como…” y pulsa Guardar → se crea/actualiza el preset.

Para reutilizarlo, selecciónalo en el desplegable y pulsa Aplicar (no lanza; solo carga la configuración).

Dónde se guarda

En tu navegador (localStorage).

Persiste entre sesiones en el mismo dispositivo y navegador.

No se sincroniza entre móviles/PCs.

Notas

Si guardas con el mismo nombre, se sobrescribe.

Trae dos ejemplos por defecto (Ataque, Iniciativa), que puedes modificar o reemplazar.
-----------------------------------------------------------------------------------------------------------

Repetir N veces

Qué hace: repite la misma tirada varias veces seguidas.

Cómo se ve: la primera se anima (traqueteo); las siguientes se calculan rápido y se listan en el modal como “Tirada 2, 3…”.

Stats (si activas “Mostrar estadísticas”): calcula mín/medio/máx y un histograma de los totales de la serie (el total ya incluye el modificador).

Tip: ideal para estimar medias y rangos de tu build/ataque.

Umbral de éxitos (≥ / ≤ objetivo)

Qué hace: cuenta cuántos dados individuales son “éxitos” según un objetivo.

Modos:

≥ objetivo: éxito si el valor del dado es mayor o igual al objetivo.

≤ objetivo: éxito si es menor o igual (útil para sistemas “roll under”).

Detalles:

Se cuenta dado a dado, no sobre la suma.

Con ventaja/desventaja en D20, se usa el valor elegido (máx/mín) para ese dado.

El modificador (+/−) no afecta al conteo de éxitos (solo al total).

Ejemplo: 4×D6 con objetivo ≥5 → tirada [6,4,5,2] da 2 éxitos (6 y 5).

Re-roll reglas

Re-roll 1s (1 vez): si un dado saca 1, se vuelve a tirar una sola vez y se sustituye el 1 por el nuevo resultado.

Exploding en máximo: si un dado saca su valor máximo (ej. 6 en D6), tiras otro y lo sumas al mismo dado; si vuelve a salir máximo, sigues encadenando.

Orden aplicado en la app: primero Re-roll 1s, luego Exploding.

Aplicación: se aplica a todos los dados, incluido D20 con ventaja/desventaja (cada valor del par se calcula con estas reglas antes de elegir).

Dado personalizado

Qué hace: creas un dado de N caras (D7, D30, lo que quieras) y aparece su card en la cuadrícula.

Visual: si no hay sprite, usa un icono genérico (fallback) — funciona igual.

Presets: si guardas un preset con dados personalizados, se guardan las cantidades.

Nota: ahora mismo los tipos personalizados se crean para la sesión actual. Si recargas, tendrías que añadirlos de nuevo (el preset guardó “2×D7”, pero para editarlos cómodamente conviene recrear su card).

Si quieres, lo hago persistente: guardo la lista de dados personalizados en localStorage y los reconstruyo al cargar.
