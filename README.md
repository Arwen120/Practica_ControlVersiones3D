# Práctica: Control de versiones con Unity

## 1. Objetivo

Experimentar con el control de versiones en un proyecto de Unity utilizando Git. Aprender a registrar cambios, guardar diferentes versiones del proyecto y trabajar con ramas.

## 2. Creación del proyecto

Se creó un proyecto 3D básico en Unity llamado `Practica_ControlVersiones3D`.

Se inicializó un repositorio local mediante Git utilizando el comando:

```bash
git init
```

También se creó un archivo `.gitignore` para excluir archivos temporales y carpetas que Unity puede generar automáticamente.

## 3. Primer cambio: esfera roja y plano azul

Se añadieron dos objetos 3D a la escena:

- Una esfera con un material de color rojo.
- Un plano con un material de color azul.

Se guardó el proyecto y se registró la primera versión mediante un commit:

```bash
git commit -m "Primera version: esfera roja y plano azul"
```

## 4. Segundo cambio: cilindro verde

Posteriormente, se añadió un cilindro a la escena y se creó un material de color verde para aplicárselo.

Los cambios se guardaron en Git mediante:

```bash
git add .
git commit -m "Segundo cambio: añadir cilindro verde"
```

## 5. Creación de una nueva rama

Se creó una nueva rama llamada `rama-capsula` para trabajar en una modificación independiente:

```bash
git switch -c rama-capsula
```

## 6. Tercer cambio: cápsula con textura

Dentro de la nueva rama se añadió una cápsula a la escena.

Se creó un material llamado `MaterialCapsula` y se le aplicó una imagen como textura.

Finalmente, se registraron los cambios:

```bash
git add .
git commit -m "Añadir capsula con textura en nueva rama"
```

## 7. Comprobación del historial

Se comprobó el historial de versiones utilizando:

```bash
git log --oneline --all --graph
```

El resultado mostró los tres commits realizados y las dos ramas del proyecto:

- `master`
- `rama-capsula`

## 8. Conclusión

Con esta práctica se ha aprendido a utilizar Git para controlar las versiones de un proyecto de Unity, registrar modificaciones mediante commits y crear ramas para desarrollar cambios de forma independiente.