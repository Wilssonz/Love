import cv2

# Carregar o vídeo
video = cv2.VideoCapture("video.mp4")

while True:
    ret, frame = video.read()
    if not ret:
        break
    
    # Mostra o vídeo em uma janela
    cv2.imshow("Video", frame)
    
    # Fecha ao apertar a tecla 'q'
    if cv2.waitKey(25) & 0xFF == ord('q'):
        break# Love

