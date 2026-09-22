# Práctica 1: Suma de 5 números
## 1. Descripción del problema (Fase 1)
El programa debe pedir al usuario cinco numeros sumarlos y mostrar el resultado de la suma.

_____

## 2. Entradas y salidas (Fase 1)

**Entradas:**
1. 5 numeros que nos da el usuario

**Salidas:**
1. La suma de esos 5 numeros
## 3. Restricciones e invariante (Fase 1 y 2)

**Restricciones** (¿qué debe cumplirse?):
- El programa pide excatamente 5 numeros y la cantidad no debe cambiar

**Decisión sobre negativos y decimales** (¿los acepto? ¿por qué?):
Si se capetan numeros decimales o negativos, el pprograma puede realizar suma con los diferentes tipos de datos. Siempre que sean arabigos
**Invariante** (¿qué es verdad después de cada vuelta del ciclo?):
La suma de todos los numeros hasta el momento, solo pueden ser 5 numeros
## 4. Casos resueltos a mano (Fase 1)

| Caso | Números | Suma calculada a mano |
|---|---|---|
| 1 | 1,2,3,4,5 | 15 |
| 2 | 0,0,0,0,0 | 0 |
| 3 | 5,-2,8,-1,3 | 13 |

## 5. Receta en pseudocódigo (Fase 2)
<!-- Tu receta va en el archivo RECETA.md. Aquí solo responde las dos preguntas. -->

**¿Probé mi receta a mano con un caso?** Sí 
**¿Tuve que corregirla?** No

## 6. Cómo compilar y ejecutar (Fase 3)

```bash
g++ -Wall -Wextra -std=c++17 main.cpp -o suma
./suma
```

## 7. Ejemplo de ejecución (Fase 3)
<!-- Pega aquí lo que muestra tu programa en pantalla con un caso normal. -->

```
Suma de 5 numeros
 Numero 1 de 5 : 3.7
 Numero 2 de 5 : 4.3
 Numero 3 de 5 : 5
 Numero 4 de 5 : 7
 Numero 5 de 5 : 9
 La suma es : 29
_____
```

## 8. Experimentos (Fase 3)

**Experimento A: ¿qué pasó al no inicializar `suma`?**
El programa puede obtener un resultado mal, por que la variable puede contener uno que ya esaba en los intentos, por eso debe inicar en 0
**Experimento B (opcional): ¿qué pasó al usar `int` con 2.5?**
_____

## 9. Tabla de pruebas (Fase 4)

| Caso | Números | Esperado | Obtenido | ¿Pasó? |
|---|---|---|---|---|
| Del 1 al 5 | 1 a 5 | 15 | 15 | si |
| Todos ceros | 0 ×5 | 0 | 0 | si |
| Con negativos | -1,-2,-3,-4,-5 | -15 | -15 | si |
| Decimales | 0.5 ×5 | 2.5 | 2.5 | si |
| Todos iguales | 7 ×5 | 35 | 35 | si |
| Caso propio 1 | 10,20,5,2,3 | 40 | 40 | si |
| Caso propio 2 | -5,10,-2,7,1 | 11 | 11 | si |

## 10. Bitácora de mejoras (Fase 4)

| # | ¿Qué falló o qué quise mejorar? | ¿Qué cambié? | ¿Funcionó? |
|---|---|---|---|
| 1 | mi ciclo "for" tenia problemas de escritura y me marcaba error | lo corregi a que iniciara en 0 hasta aumentar hasta 5 | Si |

**Reto elegido (opcional):** _____

## 11. Dudas para el profesor (Fase 3)

| Duda | Lo que ya intenté |
|---|---|
| _____ | _____ |

## 12. Reflexión final

**¿Qué aprendí con esta práctica?**
Como puedo solucionar problemas en partes pequeñas y que hacer ciclos y rpogramas en c++ no es tan complicado

**Ahora que terminé, ¿qué cambiaría de mi proceso?**
Nada, siento que para mi es correcto pensar que es mi problema, hacer una idea basica y luego pensar que ciclo funciona mejor y luego hacer mi codigo
**¿Qué fue lo más difícil y cómo lo resolví?**
Mi codigo, ya que me marcaba un error que no sabia por que lo marcaba 
**¿Qué pregunta me quedó sin responder?**
Ninguna 
## 13. Lista de verificación antes de entregar (Fase 5)

- [/ ] Llené todas las secciones (no quedan `_____`)
- [/] Mi programa compila sin advertencias
- [/] Probé todos los casos de la tabla
- [/] Hice al menos 3 commits con mensajes claros
- [/] Hice `git push` y verifiqué mi fork en GitHub
- [/] Entregué el enlace de mi fork en Classroom