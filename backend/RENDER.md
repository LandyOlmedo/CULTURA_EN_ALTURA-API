# Despliegue en Render.com

Este backend FastAPI está listo para desplegarse en Render. Sigue estos pasos:

1. **Sube todo el contenido de la carpeta `backend/` al repositorio.**
2. **Variables de entorno:**
   - Asegúrate de definir `SUPABASE_URL` y `SUPABASE_SERVICE_KEY` en el panel de Render (no subas tu .env con claves reales).
3. **Procfile:**
   - Ya existe un archivo `Procfile` con el comando correcto:  
     `web: uvicorn main:app --host 0.0.0.0 --port $PORT`
4. **Requisitos:**
   - Render instalará automáticamente las dependencias desde `requirements.txt`.
5. **Comando de inicio:**
   - Render detectará el comando del `Procfile`.

**¡Listo! Solo haz push a tu repo y crea un nuevo servicio web en Render apuntando a la carpeta `backend/`.**
