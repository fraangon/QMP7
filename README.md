# QMP7

### Como usuarie de QueMePongo quiero ver todas las prendas que tengo en mi guardarropas desde el navegador para poder administrarlas

GET https://macowins-server.herokuapp.com/prendas
 
```Json
Rta:

[
  {
    "id": 1,
    "tipo": "pantalon",
    "talle": 35
  },
  {
    "id": 2,
    "tipo": "pantalon",
    "talle": 36
  },
  {
    "id": 3,
    "tipo": "pantalon",
    "talle": 37
  },
  {
    "id": 4,
    "tipo": "pantalon",
    "talle": 38
  },
  {
    "id": 5,
    "tipo": "pantalon",
    "talle": 39
  },
  {
    "id": 6,
    "tipo": "pantalon",
    "talle": 40
  },
  etc...
]
```

### Como usuario de QueMePongo, quiero crear una prenda desde el navegador

POST 'https://macowins-server.herokuapp.com/prendas/'
```Json
{
  "id": 30,
  "tipo": "pantalon",
  "talle": "XXL"
}
```

### Como usuarie de QueMePongo quiero ver una prenda en particular que tengo en mi guardarropas para poder editarla

GET https://macowins-server.herokuapp.com/prendas?id=200

```Json 
Rta:
  [
  {
    "id": 30,
    "tipo": "pantalon",
    "talle": "XXL"
  }
]
```

### Como usuarie de QueMePongo, quiero poder eliminar una prenda de mi guardarropas

DELETE https://macowins-server.herokuapp.com/prendas?id=200

### Como usuarie de QueMePongo, quiero poder ver mis eventos para administrarlos

GET https://macowins-server.herokuapp.com/eventos

### Como usuarie de QueMePongo, quiero poder abrir las sugerencias de prendas para un evento  en mi navegador

GET https://macowins-server.herokuapp.com/sugerencias
```Json
{
  "id_evento": 300
}
```
