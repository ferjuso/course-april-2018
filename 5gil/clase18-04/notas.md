TDD (Test-Driven Development )
===================

- garantiza mantenimiento
- [SOLID] (principios de programación).
- [JEST] modulo  para pruebas unitarias.
- [SINON] libreria de objetos simulados.

**Proyectos publicados**

- objetos de simulación:
+ dummy : codigo en duro , código harcodeado 
ejemplo

const dummy = {
    error = 'FATAL',
    message = 'Something is wrong!!!'
}

+ mocks : instancia con caracteristicas de pruebas , objeto con caracteristicas especificas que nos pueden servir para nuestra prueba.

ejemplo 
const db = require('moongose');
const mock = sinon.mock(db);

+ spies : llamadas a las funciones, solo nos permite saber si se llaman las funciones o no

ejemplo 

const spy = sinon.spy(db,'short');

+ stubs : manejo de las funciones, nos dice el comportamiento de la funcion

const stub = sinon.stub(db,'short').callsFake (() => { return 5; });

************
en mock , stub y spy terminar con un en cada caso de prueba
en mock es un:  verify();
monck.restore(); 
**************

[SOLID]: <https://thefullstack.xyz/solid-javascript/>
[JEST]: <https://facebook.github.io/jest/>
[SINON]: <http://sinonjs.org/>


