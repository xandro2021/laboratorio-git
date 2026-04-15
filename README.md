# Comandos usados en el proyecto

## Iniciar Git

```bash
git init
```

## Cambiar el nombre de la rama main

```bash
git branch -m main
```

## Hacer primer commit

```bash
git add .
git commit -m "Estuructura inicial del proyecto"
```

## Verificar el historial de commits de forma resumida en una sola línea por commit

```bash
git log --graph --decorate --all --oneline
```

## Crear nueva rama llamada “desarrollo” y pasarse a trabajar en ella

```bash
git checkout -b desarrollo
```

## Realizar un nuevo commit llamado "Agrega contenido en index"

```bash
git add index.html
git commit -m "Agrega contenido en index"
```

## Unir ramas main y desarrollo

```bash
git checkout main
git merge desarrollo
```

## Crear un commit llamado "Cambio temporal"

```bash
git add styles.css
git commit -m "Cambio temporal"
git diff styles.css
```

## Eliminar el último commit y sus cambios

```bash
git reset --hard HEAD~1
```

## Recuperar el último commit

```bash
git reflog
git reset --hard 874a4f5
```

## Crear commit para agregar `.gitignore`

```bash
echo -e "*.log\n.env\n.vscode" > .gitignore
git add .gitignore
git commit -m "Agrega gitignore"
```

## Vincular proyecto a repositorio

Uso SSH en vez de agregarlo por HTTP

```bash
git remote add origin git@github.com:xandro2021/laboratorio-git.git
```

## Subir proyecto a GitHub

```bash
git push -u origin main
```

## Crear una rama nueva llamada login

```bash
git checkout -b login
```

## Hacer otro commit llamado "Agrega login"

```bash
# Se crea el archivo login para poder hacer el commit
git add login.html
git commit -m "Agrega login"
```

## Subir la rama al repositorio

```bash
git push --set-upstream origin login
```
