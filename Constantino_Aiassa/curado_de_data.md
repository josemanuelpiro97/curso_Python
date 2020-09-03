# Curado de Data

## Se debera realizar un programa que realice las siguientes funciones

1. importar un archivo del tipo csv de la base de datos dada
2. realizar un curado preliminar de la data data tratande de reducir al minimo los espacios en blanco
   - en este curado preliminar se debe reemplazar los espacios en blanco con 2 posibles valore, uno seria el de la informacion reconstruida de alguna manera(o bien un valor deducido logicamente), el otro seria con la variable NULL (esto en caso de que creas que la informacion es ingenerable).
3. exportar el archivo .csv con la base de data ya curada

## Notas

- para que se pueda interpretar correctamente cual fue el curado realizado, se debera realizar un informe con el siguiente formato:
  - columna que presentaba los espacios en blanco: "--------------------------------"
  - cantidad de espacios en blanco corregidos: "---------"
  - criterio utilizado para reemplazar los espacios en blanco
    - Esta seccion debe ser lo mas descriptiva posible, ya que dejara en evidencia la manera de ver a la informacion que adoptaste.
  - cantidad de espacios en blanco reemplazados por NULL
    - Aqui tambien es importante definir el porque crees que esa data fue imposible de deducir logicamente
  - porcentaje de informacion recuperada
  - porcentaje de informacion con perdida inminente