# op_quasar1 
Meli
Quasar Fire Operation Microservice
Para el cálculo de la posición se utilizó el método de trilateración. La trilateración es un método matemático para 
determinar las posiciones relativas de objetos usando la geometríade triángulos de forma análoga a la triangulación. 
A diferencia de esta, que usa medidas de ángulo (junto con al menos una distancia conocida para calcular la localización 
del sujeto),la trilateración usa las localizaciones conocidas de dos o más puntos de referencia, y ladistancia medida 
entre el sujeto y cada punto de referencia. 
Para determinar de forma únicay precisa la localización relativa de un punto en un plano con solo trilateración, se 
necesitan generalmente al menos 3 puntos de referencia, y en el nivel 1 del challenge nos dan las posiciones x , y como puntos del eje cartesiano.

Este método nos permite calcular la posición de un punto teniendo como datos iniciales la ubicación de otros 3 puntos y 
sus respectivas distancias con respecto al punto a calcular.
Para esto se utilizó una librería en las dependencias en el archivo pom utilizado por maven.
<dependency>
  <groupId>com.lemmingapex.trilateration</groupId><artifactId>trilateration</artifactId>
  <version>1.0.2</version>
</dependency>

El proyecto se realizó utilizando estas tecnologías:
* Java 11 con Spring-Boot 2.4.4* Maven*
