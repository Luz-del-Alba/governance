# Reto de programación UST

![UST logo](https://cdn-h4.occ.com.mx/images/logos/300x300/a8/a8d20da7c4d240159fa7357fb166dba8.jpg)





Bienvenido al reto de programación **UST**, debajo encontrarás los pasos a seguir para completar el reto.

Fuera de las restricciones técnicas, siéntete libre de diseñar el código como creas más conveniente.


## Aspectos a evaluar
* Limpieza de código
* Diseño de estructura de proyectos
* Diseño de API
* Seguridad en comunicación
* Rendimiento
* Patrones de diseño
* Pruebas unitarias
* Excepciones
* Logging
* Transaccionalidad


## Restricciones

* Spring 5
* Spring Boot 2
* Java 11
* MongoDB
* PostgreSQL
* Redis
* Angular 9
* Docker



## Proyecto
Aseguradora Luz del Alba es una compañía en crecimiento que busca proveer el servicio de generación de pólizas digitales.

### Requerimiento
Cree una plataforma (Frontend y Backend) para el cálculo de la tarifa de acuerdo a cobertura, bonus, edad del cliente, fecha de creación y riesgo tomando como base los siguientes rubros

#### Riesgos

|   Modulo  |     Cobertura      |  Edad | Bonus | Fecha  de antigüedad | Riesgo | Tarifa anual |
|-----------|--------------------|-------|-------|----------------------|--------|--------------|
| Vida      | Cobertura 500k-1m  | 20-40 | 10%   | >2000                | 20%    | 10K          |
| Vida      | Cobertura 500k-2m  | 40-60 | 15%   | <2000                | 40%    | 15K          |
| Automóvil | Cobertura 500k-1m  | 20-40 | 10%   | >2000                | 40%    | 25K          |
| Automóvil | Cobertura 1m-2m    | 40-60 | 15%   | <2000                | 20%    | 35K          |
| Casa      | Cobertura 2m-4m    | 20-40 | 10%   | >2000                | 30%    | 25K          |
| Casa      | Cobertura 4m-30m   | 40-60 | 15%   | <2000                | 10%    | 35K          |
| Robo      | Cobertura 10K-50K  | 20-40 | 10%   | >2000                | 5%     | 5K           |
| Robo      | Cobertura 50K-100K | 40-60 | 15%   | <2000                | 10%    | 7K           |


## Presentación
* Registrar notas sobre decisiones de diseño de código
* Spring Boot 2
* Java 11
* MongoDB
* Redis
* Angular 9


## TODO
1. [ ] El usuario debe ser capaz de registrarse
2. [ ] El usuario debería ser capaz de seleccionar la cobertura para cada módulo que necesite
    * [ ] Debe registrarse la fecha de antigüedad
    * [ ] El precio de la tarifa, debería ser calculado con base en los riesgos
3. [ ] Mostrar previsualización de tarifa antes de adquirirla
4. [ ] Mostrar información de póliza por cliente
5. [ ] Elaborar notas sobre decisiones de diseño de código
6. [ ] Elaborar Readme con indicaciones de uso del proyecto


## Evaluación
* Una vez recibido el código, tienes dos días para entregar el código fuente generado
