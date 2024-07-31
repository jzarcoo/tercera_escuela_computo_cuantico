# Actualizar fork

1. Agregar la referencia al repositorio remoto original, al cual llamaremos «upstream»
```sh
git remote add upstream
```

2. Traernos todas las ramas de dicho repositorio remoto
```sh
git fetch upstream
```

3. Irnos a la rama que queremos actualizar
```sh
git checkout main
```

4. Reescribir nuestra rama con los commits nuevos de la rama del repositorio original
```sh
git rebase upstream/master
```

5. Finalmente si queremos actualizar nuestro fork remoto
```sh
git push main
```
