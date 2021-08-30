FROM  python:3.6
LABEL maintainer 'Ricardo Castro <ricdecastro2009@gmail.com>'

RUN useradd www && \ 
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

## Entrypoint é o processo q será iniciado no momento em que meu container tiver execultando
## é o ponto de entrada 
ENTRYPOINT [ "/usr/local/bin/python"]
## CMD é o comando que eu passo pro meu entrypoint
CMD ["run.py"]



## comando para subir esse container com um servidor python
## docker container run -it -v C:/Users/ricardo.castro/Documents/Pessoal/docker-udemy/build-dev:/app -p 80:8000 --name python-server ex-build-dev


## comando para copiar os volumes do container anterior python agora subindo em uma imagem debian
## docker container run -it --volumes-from=python-server debian cat /log/http-server.log


