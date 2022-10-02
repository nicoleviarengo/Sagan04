# Sagan04 - Challenge para el NASA Spaceapps San Francisco
### [Exploring Venus Together 🚀](https://2022.spaceappschallenge.org/challenges/2022-challenges/exploring-venus/details)
<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://images.spaceappschallenge.org/images/8xBhEEUSQiafDwF09-ioi2ptqXU=/20069/fill-591x300/" alt="Logo" width="80" height="40">
  </a>
El planeta Venus presenta una superficie con altas temperaturas y una densa atmósfera convirtiéndolo en un ambiente muy difícil de explorar. La temperatura asciende a los 450°C y su atmósfera está compuesta por un 96,5% de CO2, en menor proporción contiene ácido sulfúrico y nitrógeno. Posee un campo eléctrico 10 veces mayor al de la Tierra.

Nuestro objetivo es diseñar un sistema de almacenamiento de energía que dure al menos 60 días terrestres. 
Uno de los mayores desafíos que se deben superar es el de soportar las altas temperaturas sin que se dañen los equipos, teniendo en cuenta las fuerzas y vibraciones debidas al lanzamiento, reingreso, descenso y aterrizaje. 

Para la resolución de este desafío, consideramos varias opciones antes de encontrar la más viable.
	Primeramente se optó por elegir un reactor RPS (Sistema de Poder por Radioisótopo) el cual utiliza como fuente altamente estable módulos GPHS (Fuente de Calor de Uso General). Los módulos tienen una masa de 1.5 kg y contiene en su interior 600 gr de dióxido de plutonio 238 (238PuO2), con la cual se pueden alcanzar temperaturas de 1500° C. Al poner dicha fuente de calor dentro de una cámara aislada térmicamente del ambiente de Venus, se produce una clara diferencia de temperatura la cual es aprovechada por un arreglo de materiales termoeléctricos de tipo silicio-germanio conectados en serie y paralelo para conseguir mediante el efecto seebeck las diferencias de temperatura en una diferencia de potencial eléctrico. Se estima que se necesitan 32 termoeléctricos por cada módulo GPHS.  
  
	Más allá de ser una fuente de alimentación estable y duradera, se la descartó por ser demasiado pesado, por el riesgo de que la radiación afecte la electrónica y por el riesgo de transportar material radiactivo, a que en caso de que algo falle durante el lanzamiento y el cohete explote se esparciría este material sobre una amplia zona de nuestro planeta.
  
Por esta razón es que se decidió utilizar como fuente de alimentación principal baterías de sodio y azufre, ya que son recargables y de alta durabilidad. Una batería de sodio y azufre es construida a partir de sodio líquido y azufre. Este tipo de baterías tiene una alta densidad de energía, alta eficiencia de carga / descarga y una larga vida útil, y está fabricada con materiales económicos y no tóxicos. Las temperaturas de funcionamiento de 300 a 350 °C y la naturaleza altamente corrosiva de los polisulfuros de sodio, principalmente los hacen adecuados para aplicaciones estacionarias de almacenamiento de energía. La celda se vuelve más económica a medida que aumenta el tamaño. Las celdas disponibles en el mercado suelen ser grandes y de alta capacidad (hasta 500 Ah). Esto se debe a que las celdas más grandes se enfrían a un ritmo más lento que las celdas más pequeñas, lo que les permite mantener altas temperaturas de funcionamiento.

Un panel solar capaz de soportar altas temperaturas es la principal fuente de alimentación para recargar la batería. La energía brindada por el panel es medida por la electrónica del rover, en caso de que el panel deje de funcionar o baje su productividad debido a nubes, polvo o por estar de noche, la batería cuenta con un sistema de respaldo para recargarse el cual es un generador eólico vertical. A pesar de que los vientos de Venus no son veloces, la fórmula para calcular el empuje del viento contempla la densidad del gas (P = (Cd * ρ  *  V2) / 2; donde P es la presión, ρ (rho)  es la densidad del aire seco, Cd es el coeficiente aerodinámico de resistencia de avance y V es la velocidad), por lo tanto al ser una atmósfera altamente densa no es un inconveniente la velocidad del viento. 

### Panel Solar
Para saber identificar paneles solares eficientes de los que no lo son, no te fijes solo en la potencia del panel, debes mirar la potencia y los metros cuadrados del panel solar para saber su eficiencia. Eficiencia = Watts del panel / superficie. Cuanto más elevado, más eficiente.
Los paneles solares más eficientes que existen son los que incorporan las tecnologías monocristalinas, que usan silicio tipo N.

### Sistema de refrigeración
El calor será bombeado fuera usando un enfriador Stirling, que trabaja comprimiendo y expandiendo un gas con un pistón. Cuando el gas se expande se enfría, absorbiendo el calor desde el compartimento de la electrónica. Entonces, como el gas se comprime y su temperatura se eleva, se permite que el calor se disipe en la atmósfera a través de un radiador.


