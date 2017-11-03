# ejercicio13dl

# Actividad Presencial 1 de Jquery
### ¿Cuál es el error? - Solución:

```javascript
	var calcularIMC = function(peso, estatura){
	 	return peso / (estatura * estatura);
	}

	var interpretarIMC = function(peso, estatura){
		var imc = calcularIMC(peso, estatura);
		if (imc > 24){
		 		return "sobrepeso";
		} else if (imc > 19 && imc <= 24) {
		 		return "ok";
		} else {
		 		return "bajo peso";
		}
	}

	resultado = interpretarIMC(55, 1.64);
	console.log(resultado);
```

### Ejercicios de Desarrollo

Para realizar estos ejercicios entra a: https://jsfiddle.net/1fk5fyLc/7/ Recuerda documentar todos los pasos en un archivo llamado tunombre.md para que puedas subir tus respuestas a la plataforma.

### Solución:

- Pon tu nombre al atributo value del campo first name
```javascript
$('input[name="firstname"]').val('Daniela');
```
- Pon el valor a la pregunta Favorite Day of Week a Monday
```javascript
$('select[name="fav_day"]').val('Monday');
```
- Cambia la etiqueta de First name a 'Tu nombre'
```javascript
$('label[name="first_name_label"]').text('Tu nombre');
```
- Obtén el valor del atributo 'name' del campo Favorite Day of The Week
```javascript
var name_favday = $('select').attr('name');
```
- Escoge la opción Female de la pregunta de género.
```javascript
$('input[value="female"]').attr("checked", true);
```
- Encuentra la primera form del documento y pon el atributo name = personal_info
```javascript
$('form').eq(0).attr('name', 'personal_info');
```
- Encuentra la primera **(segunda?)** form del documento y pon el atributo name = job_info
```javascript
$('form').eq(1).attr('name', 'job_info');
```
- Agrega un título h1 a cada una de las formas que diga 'Entrevista personal', 'Entrevista de trabajo' respectivamente
```javascript
$('form').eq(0).attr('name', 'personal_info');
$('form').eq(1).attr('name', 'job_info');
```
- Agrega un título a la pregunta Male/Female 'Gender'
```javascript
$('input[value="male"]').before('<h4>Select your Gender:</h4>');
```
- Agrega una pregunta Email: con un input de tipo texto después de last name
```javascript
$('input[name="lastname"]').after('<br><label name="mail">Email:</label>');
$('label[name="mail"]').after('<br><input type="text">');
```
- Agrega la clase form a ambas for
```javascript
$('form').addClass('form');
```
