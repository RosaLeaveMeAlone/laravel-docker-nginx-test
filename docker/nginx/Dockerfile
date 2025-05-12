# Usa una imagen liviana de NGINX
FROM nginx:alpine

# Crea el directorio del proyecto (por si no existe)
RUN mkdir -p /var/www/html

# Copia el código de tu proyecto al contenedor (opcional si solo sirve archivos estáticos)
COPY . /var/www/html

# Copia tu configuración personalizada de NGINX (si tienes una)
# Asegúrate de tener un archivo como ./docker/nginx/default.conf
COPY ./docker/nginx/default.conf /etc/nginx/conf.d/default.conf
