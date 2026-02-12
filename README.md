# README DE web-template
Información básica de flujos de trabajo con web-template. Editar para customizar con cada proyecto.

##FLUJO DE BASE DE DATOS

Resumen del Flujo Correcto
Local: Haces cambios en el Studio (localhost:54323).

Generar: Ejecutas npx supabase db diff -f cambios_nuevos. (Se crea el archivo).

Git: Haces git add ., git commit y git push.

GitHub: El Action ve el archivo nuevo y lo aplica a Producción.
