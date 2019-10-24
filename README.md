# Streamming de vídeo

## Aplicação Cliente-Servidor utilizando os protocolo RTP + RTSP

Essa atividade visa aplicar os conceitos teóricos vistos na disciplina, através de uma aplicação prática do protocolo de Streaming RTSP. Será implementado um cliente e um servidor que irão se comunicar pelo protocolo RTSP, encapsular alguns dados no protocolo RTP/UDP e demonstrar o uso.

O projeto foi separado em 4 classes, onde cada uma dela é responsável por implementar uma função na aplicação. A classe Client, cuida do controle do protocolo do lado cliente; A classe Server cuida do protocolo do lado servidor; A classe VideoStream é responsável por inicializar o vídeo e buscar frame a frame do mesmo; A classe RTP packet é responsável por fazer toda a abstração do protocolo RTP.


Rode o servidor:
```
java Server server_port
java Server 3000
```

Rode o cliente
```
java Client server_ip server_port movie
java Client localhost 3000 movie.Mjpeg
```