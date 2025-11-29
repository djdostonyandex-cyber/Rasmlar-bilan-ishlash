# Rasmlar-bilan-ishlash
Google Colabda python dasturlash tilida rasmlar bilan ishlash
Bu loyiha bilan biz rasmlarni rangsiz qilishimiz mumkun
Dastlab opencv kutubxonasini o'rnatib olamiz
!pip install opencv-python

Keyin cv2 kutubxonasini chaqirib olamiz
import cv2
from google.colab.patches import cv2_imshow

Rasmni o'qitib olamiz va hajmini o'zgartiramiz
img = cv2.imread('nature.jpg')
img = cv2.resize(img, (img.shape[1] // 3 ,img.shape[0] // 3))

Rasmni rangsiz qilish kodini kiritamiz
img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

Rasmni ekranga chiqaramiz
cv2_imshow(img)
