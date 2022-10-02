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
	Primeramente se optó por elegir un reactor RPS (Sistema de Poder por Radioisótopo) el cual utiliza como fuente altamente estable módulos GPHS (Fuente de Calor de Uso General). Los módulos tienen una masa de 1.5 kg y contiene en su interior 600 gr de dióxido de plutonio 238 (238PuO2), con la cual se pueden alcanzar temperaturas de 1500° C. Al poner dicha fuente de calor dentro de una cámara aislada térmicamente del ambiente de Venus, se produce una clara diferencia de temperatura la cual es aprovechada por un arreglo de materiales termoeléctricos de tipo silicio-germanio conectados en serie y paralelo para conseguir transformar mediante el efecto seebeck las diferencias de temperatura en una diferencia de potencial eléctrico. Se estima que se necesitan 32 termoeléctricos por cada módulo GPHS.
	
Mas allá de ser una fuente de alimentación estable y duradera, se la descartó por ser demasiado pesado, por el riesgo de que la radiación afecte la electrónica y por el riesgo de transportar material radioactivo, a que en caso de que algo falle durante el lanzamiento y el cohete explote se espariría este material sobre una amplia zona de nuestro planeta.
  
Por esta razón es que se decidió utilizar como fuente de alimentación principal baterías de sodio y azufre, ya que son recargables y de alta durabilidad. Una batería de sodio y azufre es construida a partir de sodio líquido y azufre. Este tipo de baterías tiene una alta densidad de energía, alta eficiencia de carga / descarga y una larga vida útil, y está fabricada con materiales económicos y no tóxicos. Las temperaturas de funcionamiento de 300 a 350 °C y la naturaleza altamente corrosiva de los polisulfuros de sodio, principalmente los hacen adecuados para aplicaciones estacionarias de almacenamiento de energía. La celda se vuelve más económica a medida que aumenta el tamaño. Las celdas disponibles en el mercado suelen ser grandes y de alta capacidad (hasta 500 Ah). Esto se debe a que las celdas más grandes se enfrían a un ritmo más lento que las celdas más pequeñas, lo que les permite mantener altas temperaturas de funcionamiento.
También poseen una energía específica de 150 Wh/kg (3 veces la densidad de energía de una batería de níquel-hidrógeno), operando a 350ºC.
 
La principal fuente de alimentación para recargar la batería es un panel solar de multijunción metamórfica invertidas, compuesto por 3 capas las cuales son fosfuro de indio de galio en la parte superior, arseniuro de galio en la parte central y arseniuro de indio de galio en la parte inferior. El uso de estos diferentes materiales permite un aprovechamiento más amplio dentro del espectro lumínico, además tiene una brecha de energía lo suficientemente amplia como para funcionar a las altas temperaturas de Venus. La energía brindada por el panel es medida por la electrónica del rover. En caso de que el panel deje de funcionar o baje su productividad debido a nubes, polvo o por estar de noche, la batería cuenta con un sistema de respaldo para recargarse el cual es un generador eólico vertical de 50cm de alto por 20cm de diámetro. La turbina eólica se encuentra en posición horizontal dentro del rover, en el momento de ser necesaria su implementación este se posiciona en vertical permitiendo que el viento lo mueva. A pesar de que los vientos de Venus no son veloces, la fórmula para calcular el empuje del viento contempla la densidad del gas (P = (Cd * ρ  *  V2) / 2; donde P es la presión, ρ (rho)  es la densidad del aire seco, Cd es el coeficiente aerodinámico de resistencia de avance y V es la velocidad), por lo tanto al ser una atmósfera altamente densa la velocidad del viento no es un inconveniente. 
 
Dado que la temperatura en la superficie de Venus supera a la temperatura de operación de la batería se utilizará un sistema de refrigeración. El calor será bombeado hacia afuera usando un enfriador Stirling, que trabaja comprimiendo y expandiendo un gas con un pistón. Cuando el gas se expande absorbe energía (calor) de su entorno y por lo tanto lo enfría. Entonces, cuando el gas se comprime  libera energía (calor), este calor se disipa en la atmósfera a través de un radiador.
