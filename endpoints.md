Obtener todos los usuarios

GET `/user-service/api/users` Check

Obtener un usuario por id

GET `/user-service/api/users/{userId}` Check

Crear un usuario

POST `/user-service/api/users` 

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