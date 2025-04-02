# Dígito verificador de un rut en Excel

¿Alguna vez necesitaste una fórmula que calcule el DV de un rut en Excel? ¿Googleaste y lo único que encontrabas era usar macros o lenguajes de programación? Entonces llegaste al lugar correcto 😄 Únicamente usando fórmulas de Excel, sin macros.

# Uso

Escribe un RUT en la celda A1. Pega la fórmula en cualquier otra celda de la misma hoja. Si necesitas leer el RUT desde una celda distinta puedes usar "Reemplazar" para cambiar todos los A1 por la celda donde esté el RUT.
 
=SI(11-(RESIDUO((SI.ERROR(EXTRAE(A1;LARGO(A1);1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-1;1); 0)*3)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-2;1); 0)*4)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-3;1); 0)*5)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-4;1); 0)*6)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-5;1); 0)*7)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-6;1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-7;1); 0)*3);11))=10; "K"; SI(11-(RESIDUO((SI.ERROR(EXTRAE(A1;LARGO(A1);1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-1;1); 0)*3)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-2;1); 0)*4)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-3;1); 0)*5)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-4;1); 0)*6)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-5;1); 0)*7)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-6;1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-7;1); 0)*3);11))=11; 0; 11-(RESIDUO((SI.ERROR(EXTRAE(A1;LARGO(A1);1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-1;1); 0)*3)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-2;1); 0)*4)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-3;1); 0)*5)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-4;1); 0)*6)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-5;1); 0)*7)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-6;1); 0)*2)+(SI.ERROR(EXTRAE(A1;LARGO(A1)-7;1); 0)*3);11))))

# Cierre

- Si la fórmula te salvó en la pega, puedes darme las gracias por X en [@Chaskon](https://x.com/Chaskon)
  
- Si quieres ser el master en Excel puedes comprar mi libro en [Apple](https://books.apple.com/cl/book/excel-avanzado-2024/id6450328094) o [Amazon](https://a.co/d/5spQTNj)
