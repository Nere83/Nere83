-<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Escape Room: Teoría del Vuelo</title>
    <script>
        function verificarRespuesta(pregunta, respuestaCorrecta) {
            let seleccion = document.querySelector(`input[name="${pregunta}"]:checked`);
            if (seleccion) {
                if (seleccion.value === respuestaCorrecta) {
                    alert("✅ ¡Correcto!");
                } else {
                    alert("❌ Incorrecto. Inténtalo de nuevo.");
                }
            } else {
                alert("⚠️ Debes seleccionar una respuesta.");
            }
        }
    </script>
</head>
<body>
    <h1>Escape Room: Teoría del Vuelo</h1>
    <p>Eres un técnico de mantenimiento de aviones. Ayuda al piloto a recuperar el control de la aeronave resolviendo los desafíos.</p>
    
    <h2>Etapa 1: Fuerzas en el Vuelo</h2>
    <p><strong>Pregunta 1:</strong> ¿Cuál de las siguientes opciones NO es una de las cuatro fuerzas aerodinámicas básicas?</p>
    <input type="radio" name="p1" value="Sustentación"> Sustentación<br>
    <input type="radio" name="p1" value="Peso"> Peso<br>
    <input type="radio" name="p1" value="Velocidad"> Velocidad<br>
    <button onclick="verificarRespuesta('p1', 'Velocidad')">Verificar</button>
    
    <h2>Etapa 2: Ascensos y Descensos</h2>
    <p><strong>Pregunta 2:</strong> ¿Cómo se llama el ángulo que determina la pendiente de un ascenso?</p>
    <input type="radio" name="p2" value="Ángulo de ataque"> Ángulo de ataque<br>
    <input type="radio" name="p2" value="Ángulo de ascenso"> Ángulo de ascenso<br>
    <input type="radio" name="p2" value="Factor de carga"> Factor de carga<br>
    <button onclick="verificarRespuesta('p2', 'Ángulo de ascenso')">Verificar</button>

    <h2>Etapa 3: Virajes y Maniobras</h2>
    <p><strong>Pregunta 3:</strong> ¿Cuál es la fuerza que mantiene el avión en un viraje?</p>
    <input type="radio" name="p3" value="Sustentación"> Sustentación<br>
    <input type="radio" name="p3" value="Fuerza centrífuga"> Fuerza centrífuga<br>
    <input type="radio" name="p3" value="Peso"> Peso<br>
    <button onclick="verificarRespuesta('p3', 'Fuerza centrífuga')">Verificar</button>
    
    <h2>Etapa 4: Sustentación y Dispositivos Hipersustentadores</h2>
    <p><strong>Pregunta 4:</strong> ¿Cuál de los siguientes dispositivos es un hipersustentador?</p>
    <input type="radio" name="p4" value="Flaps"> Flaps<br>
    <input type="radio" name="p4" value="Spoilers"> Spoilers<br>
    <input type="radio" name="p4" value="Tren de aterrizaje"> Tren de aterrizaje<br>
    <button onclick="verificarRespuesta('p4', 'Flaps')">Verificar</button>
    
    <h2>Etapa 5: Factores de Carga y Limitaciones</h2>
    <p><strong>Pregunta 5:</strong> ¿Qué representa el factor de carga?</p>
    <input type="radio" name="p5" value="La cantidad de combustible usado"> La cantidad de combustible usado<br>
    <input type="radio" name="p5" value="La relación entre sustentación y peso"> La relación entre sustentación y peso<br>
    <input type="radio" name="p5" value="La velocidad del avión"> La velocidad del avión<br>
    <button onclick="verificarRespuesta('p5', 'La relación entre sustentación y peso')">Verificar</button>

    <p>¡Buena suerte! Completa todas las etapas para ayudar al piloto.</p>
</body>
</html>
