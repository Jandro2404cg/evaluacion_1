# evaluacion_1
/*
Autor Cabrera Garcia Alejandro Asael
Fecha 23/02/2023
/*
/*
Este programa contas de ayudar a los usuarios que los usen a conserguir una cita mediante 10 preguntas cpn un cierto valor en las cuales les van a ser posible saber si son compatibles o no donde 1 = si y 0 = no al final se sumaran los puntos entre los puntos maximos  y si el resultado es igual o mayor a 70% se lanzara un mensaje en el cual te dice que eres compatible con esa persona y si es el caso contrario se da un mensaje donde dira que lo intentes con otra persona 
*/

#include <stdio.h>

int main() {
    int puntos = 0;
    
    // Preguntas y puntajes
    printf("Pregunta 1: ¿Te gusta la comida picante? (1 = Sí, 0 = No): ");
    int respuesta;
    scanf("%d", &respuesta);
    puntos += respuesta * 2;
    
    printf("Pregunta 2: ¿Practicas algún deporte? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 3;
    
    printf("Pregunta 3: ¿Eres una persona extrovertida o introvertida? (1 = Extrovertido, 0 = Introvertido): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 4;
    
    printf("Pregunta 4: ¿Te gustan los perros? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 2;
    
    printf("Pregunta 5: ¿Te gusta la música electrónica? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 1;
    
    printf("Pregunta 6: ¿Tienes alguna alergia alimentaria? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * -1;
    
    printf("Pregunta 7: ¿Eres una persona madrugadora o noctámbula? (1 = Madrugador, 0 = Noctámbulo): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 3;
    
    printf("Pregunta 8: ¿Te gusta viajar? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 4;
    
    printf("Pregunta 9: ¿Eres una persona paciente? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 2;
    
    printf("Pregunta 10: ¿Te gusta la playa? (1 = Sí, 0 = No): ");
    scanf("%d", &respuesta);
    puntos += respuesta * 3;
    
    // Calcular resultado final
    float resultado = (float)puntos / 24 * 100;
    
    // Imprimir mensaje
    if (resultado > 70) {
        printf("Felicidades, esta persona es la ideal para ti, cumple con tus características deseadas. ¡Suerte en tu cita!\n");
    } else {
        printf("Lo sentimos, esta persona no cumple con tus características deseadas. ¡Sigue buscando!\n");
    }
    
    return 0;
}
