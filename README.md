Cuayolo - db
==========

Estructura de la base de datos para el sitio de cuayolo en MongoDB.

```
  +--------+--------+
  |   Collection    |
  +--------+--------+
  |  key   | value  |
  +--------+--------+
  | name   | text   |
  | age    | number |
  | update | date   |
  | active | bolean |
  +--------+--------+
```

Implementación
----------
```
mongoimport --collection collection --file collection.json
```

Consultas.
----------

```js
   // Recuperar el dato donde 'last_name' == 'Smith':
   db.users.find ({'last_name': 'Smith'});
```

```js
   // Salta 20 registros y devuelve los siguientes 10
   db.users.find ().skip (20).limite (10);
```

####Enlaces utiles.
- [Consultas utiles](http://qbit.com.mx/blog/2013/10/09/mongodb-consultas-utiles/)
- [Generador de Tablas Ascii](http://www.sensefulsolutions.com/2010/10/format-text-as-table.html)
