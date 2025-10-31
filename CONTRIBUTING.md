# Convensiones de PlayMatch

## Motivos de su aplicación

- Facilidad en su uso.
- Facilidad de comprensión para cualquier nuevo colaborador o consultor.
- Orden en el desarrollo del proyecto.

## Mensajes de Confirmación

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]

```

### Ejemplo

```
docs (Develop): se realiza ejemplo para mensaje de confirmacion.

Por medio de este mensaje describo que este va a ser un ejemplo para mensaje de confirmación para asi realizar cualquier commit describiendo toda actividad que realice aqui.

(Se cierra requerimiento #0001)
```

## Asunto del mensaje

Primera linea de poca longitud con menos de 70 caracteres, segunda linea siempre en blanco, demas lineas ajustadas a 80 caracteres. El tipo y alcance siempre en minúsculas.

### ``<type>``

Es el tipo de suceso que se esta realizando con la confirmacion, siendo de diversos tipos acorde al cambio realizado.

## Valores permitidos de ``<type>``

- feat (Caracteristicas nuevas para usuario, no caracteristica nueva para script de compilación).

- fix (corrección de errores para usuario, no correccion de script de compilación).

- docs (cambios en la documentación).

- style (formateo, puntos y comas que faltan,etc. sin cambio de codigo de producción).

- refactor (codigo de producción de refactorización, por ejemplo, cambio de nombre de una variable).

- test (agregando pruebas faltantes, pruebas de refactorización, sin cambio codigo de producción).

- chore (actualización de tareas, sin cambio en codigo de producción).

- merge (fusion de ramas, cambio en codigo de produccion).

- release (creacion de una nueva version de proyecto).

## scope

Representa el modulo sobre el que se esta realizando el cambio. Puede llegar a estar vacio, siempre y cuando el cambio sea de manera global o cuando es dificil determinar un modulo o si los cambios son para mas de un modulo.

## Cuerpo del mensaje

Descripción breve y concisa con información de utilidad que ayude a determinar de que trata el cambio para no dejar lugar a dudas. Por lo general, describir como se resolvio sin entrar en detalles tecnicos.

## Footer

Los **Issues** cerrados deben ir enumerados en una linea separada del pie de pagina con la palabra clave **Closed**. Adicionalmente en caso de ser necesario agregar un co-autor se debera agregar en el footer.

### Ejemplo

````
co-authored-by: Name <correo@gmail.co>.

Closed #0003, #0010, #0030.
````

## Semantica de versionamiento

Se utilizará Versionamiento Semantico 2.0.0-rc.2

### Motivos para su aplicación

Sistema de versionado de baja complejidad.

Facilidad de entendimiento para nuevos colaboradores o consultores.
Llevar orden en el desarrollo del proyecto permitiendo un control sobre el estado del mismo.

### Versionamiento

Se han de aplicar las siguientes restricciones y normas al versionado del proyecto:

- se usara los digitos en orden X.Y.Z donde estos son enteros (no negativos).
- X es el digito"mayor", siendo cambios significativos en el proyecto, tales como: cambios o borrado de multiples de funcionalidades.

> [!NOTE]
> Por lo general estos cambios pueden resultar en incompatibilidad con algunas funciones de sus versiones anteriores.

- Y es el digito "menor", siendo cambios de nuevas funcionacionalidades con compatibilidad con versiones anteriores.

- Z es el digito "patch", siendo correccion de fallas, se utiliza para correcion de funcionalidades o cambios esteticos.

### Ejemplo

PlayMatch 1.2.3

