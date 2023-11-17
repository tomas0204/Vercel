# Django + Vercel + Tailwind = ❤️

**Es una base lista para ser clonada!**

- Ya te reconoce los staticsfiles
- Te permite trabajar con Tailwind
- Usas Vercel
- Usas Django

*Que mas puedes pedir?*

Solo te falta el dominio para tu grandiosa app/web, pero ese no te lo puedo dar yo...

## A tomar en cuenta

Antes de entrar a produccion te recomiendo checar estos detalles

```py
#vercel_app/settings.py
Debug = False
```

Haz las migraciones!

```sh
python manage.py makemigrations && python manage.py migrate
```

Tambien puedes poner las migraciones "automaticas" en el archivo `vercel_build_staticfiles.sh` **descomentando** la linea que viene abajo de `Automatic Migrations` esto hara que las migraciones se hagan cada que se recopilen los staticsfiles

Tienes Super usuario?

```sh
python manage.py createsuperuser
```
