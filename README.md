# Proyecto final: Entrega 3 - Rombolá Julián.

## Cambios
### Login
Para acceder a las funcionalidades existen 2 tipos de usuarios.
1. **Común:** Sólo puede ver el listado de alumnos, sin posibilidad de hacer cambios.
2. **Admin:** Puede hacer cambios sobre los alumnos (ABM).

La pass para ambos tipos de usuarios es: **1234**.
- Para acceder como Administrador, el nombre de usuario es "Admin".
- Para acceder como usuario común, el nombre de usuario es indiferente (Sólo valida la pass).

### ABM
La modificación de datos se hace directamente sobre la REST API. Es decir, al dar de alta un alumno se hace un POST, al eliminar se hace un DELETE, al consultar se hace un GET.

Todo esto se hace desde el servicio: **AlumnosService**.

### Guards
El acceso a las distintas rutas se hace validando el logueo/tipo de usuario.

### Tests
Se agregaron test para:
- Servicio Auth: _auth.service.spec_
- Listado de Alumnos: _listado-alumnos.component.spec_
