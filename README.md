# crear-repositorio-de-rpms
Como crear un servidor repositorio de rpms

Primero creamos la estructura:

```bash
mkdir -p repo/rhel6/{i386,x86_64}
```

luego inicializamos los repositorios

```bash
createrepo repo/rhel6/i386
createrepo repo/rhel6/x86_64
```

Después de cada cambio debemos actualizar los datos de cada repositorio:

```bash
createrepo --update repo/rhel6/i386
createrepo --update repo/rhel6/x86_64
```

No olvidar dejar accesibles las carpetas por nuestro servidor web de preferencia


