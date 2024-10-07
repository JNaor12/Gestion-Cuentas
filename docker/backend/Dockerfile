# Imagen base de Python
FROM python:3.12.3

# Establecer el directorio de trabajo
WORKDIR /app

# Copiar el archivo de requerimientos y luego instalarlos
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copiar el resto de la aplicación al contenedor
# COPY ../../backend .

# Exponer el puerto que Django utilizará (8000 por defecto)
EXPOSE 8000

# Comando por defecto para ejecutar Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
