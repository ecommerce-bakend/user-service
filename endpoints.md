Obtener todos los usuarios

GET `/user-service/api/users` Check

Obtener un usuario por id

GET `/user-service/api/users/{userId}` Check

Crear un usuario

POST `/user-service/api/users` 

Errores:

- Recibe al userId como parámetro, lo cual rompe cuando el id ya es de otro usuarios

- Cuando se crea un usuario con el objeto Credentials, como la relación es de tipo fetch lazy, cuando se hace el fetch esa relación no esta en el contexto de hibernate
```
{
    "userId": "{{$randomInt}}",
    "firstName": "Alejandro",
    "lastName": "Cordoba",
    "imageUrl": "{{$randomUrl}}",
    "email": "{{$randomEmail}}",
    "addressDtos": [
        {
            "fullAddress": "123 Main St",
            "postalCode": "12345",
            "city": "New York"
        }
    ],
    "credential": {
        "username": "johndoe",
        "password": "securePassword123",
        "roleBasedAuthority": "ROLE_USER",
        "isEnabled": true,
        "isAccountNonExpired": true,
        "isAccountNonLocked": true,
        "isCredentialsNonExpired": true
    }
}
```

Lo crea pero no se encuentra

Actualizar un usuario

PUT `/user-service/api/users` Check


```

```