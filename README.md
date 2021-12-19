# 1.6Escala_de_grises
Es la sexta tarea del Primer Parcial de mi materia de Análisis y Procesamiento de Imágenes

## *INSTRUCCIONES*

Investigar la ecuación matemática que transforma los tres canales del BGR hacia la escala de grises. 

Subir un PDF con el nombre de archivo correcto.
- La ecuación utilizada para la transformación
- El código visto en clase (abajo)
- Escoger una imagen de su computadora (o internet) y pegarla en original
- Aplicar el código de abajo y pegar en escala de grises
```
import cv2
imagen = cv2.imread('messi5.jpg')
img_gris = cv2.cvtColor(imagen, cv2.COLOR_BGR2GRAY) #un canal
img_rgb = cv2.cvtColor(img_gris, cv2.COLOR_GRAY2BGR) #tres canales
cv2.imshow('Gris', img_rgb)
k = cv2.waitKey(0)
cv2.destroyAllWindows()
```
