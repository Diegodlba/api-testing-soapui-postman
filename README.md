# Pruebas de servicios SOAP y REST

Trabajo final del curso de testing de APIs. Probé dos servicios con dos herramientas distintas:

- **Servicio SOAP** del Banco Central del Uruguay (cotizaciones de monedas), con **SoapUI**.
- **Servicio REST** JSONPlaceholder (recurso `/comments`), con **Postman**.

En los dos casos armé casos de prueba válidos e inválidos y usé *assertions* para comparar el resultado esperado con el obtenido.

## Qué hay en el repositorio

- `soapui/`: proyecto de SoapUI con 11 casos de prueba.
- `postman/`: colección de Postman con 12 requests (GET, POST, PUT y DELETE).
- `docs/`: informe con el detalle de los casos, las assertions y los resultados.

## Errores encontrados

- En el servicio SOAP, enviar un código de moneda no numérico devuelve un error HTTP 500.
- En el servicio REST, hacer un PUT sobre un id que no existe también devuelve un error 500.

## Cómo abrirlo

- **SoapUI:** File → Import Project y elegir el archivo `.xml` de la carpeta `soapui`.
- **Postman:** Import y elegir el archivo `.json` de la carpeta `postman`.
