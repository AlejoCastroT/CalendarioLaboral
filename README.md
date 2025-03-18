📌 Historias de Usuario  
🏷 HU01 - Consultar Festivos por País y Fecha  
Como usuario de la API  
Quiero ingresar un ID de país, mes y día  
Para saber si en esa fecha es festivo en ese país  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta GET a /festivos/{idPais}/{mes}/{dia}  
✔️ Si la fecha es festivo, la API debe devolver true  
✔️ Si la fecha no es festivo, la API debe devolver false  

🏷 HU02 - Obtener Todos los Festivos de un País
Como usuario de la API
Quiero obtener una lista de todos los festivos de un país
Para conocer las fechas importantes de esa nación  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta GET a /festivos/{idPais}  
✔️ La API debe devolver un JSON con la lista de festivos de ese país  
✔️ Si el país no tiene festivos registrados, debe devolver una lista vacía  

🏷 HU03 - Registrar un Nuevo Festivo
Como administrador del sistema
Quiero poder agregar un nuevo festivo a la base de datos
Para actualizar la información cuando haya cambios  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta POST a /festivos enviando un JSON con los datos del festivo  
✔️ La API debe almacenar el festivo en la base de datos  
✔️ Si el festivo ya existe, la API debe devolver un mensaje de error  

🏷 HU04 - Listar Todos los Países Disponibles
Como usuario de la API
Quiero obtener una lista de todos los países registrados
Para saber qué países tienen información de festivos  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta GET a /paises  
✔️ La API debe devolver un JSON con la lista de países disponibles  
✔️ Si no hay países registrados, debe devolver una lista vacía  

🏷 HU05 - Consultar Detalles de un País
Como usuario de la API
Quiero obtener la información detallada de un país
Para conocer sus festivos y otros datos relevantes  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta GET a /paises/{id}  
✔️ La API debe devolver un JSON con la información del país y sus festivos  
✔️ Si el país no existe, la API debe devolver un error 404  

🏷 HU06 - Eliminar un Festivo
Como administrador del sistema
Quiero eliminar un festivo de la base de datos
Para corregir errores o actualizar la información  

Criterios de Aceptación:  
✔️ Debo poder hacer una consulta DELETE a /festivos/{id}  
✔️ La API debe eliminar el festivo de la base de datos  
✔️ Si el festivo no existe, la API debe devolver un error 404  
