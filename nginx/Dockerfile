# Usamos la imagen oficial de Nginx como base
FROM nginx:latest

#Creamos un directorio de trabajo
WORKDIR /var/www/html

# Copiamos el archivo principal de HTML al directorio de contenido estático de Nginx
COPY IPN/Proyecto_web /usr/share/nginx/html/

#Copiamos el archivo de configuración de nginx
COPY nginx.conf /etc/nginx/nginx.conf

# Puerto en el que Nginx escuchará
EXPOSE 80

# Comando para iniciar Nginx en primer plano
CMD ["nginx", "-g", "daemon off;"]

