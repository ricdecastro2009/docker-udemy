## A partir de qual imagem quero basear minha nova imagem
## E construir a minha imagem a partir das layers do nginx
FROM nginx:latest

## Vai aproveitar todas as layers do nginx e vai adicionar essa que estou adionando no RuN
RUN echo '<h1>Hello World</h1>' > /usr/share/nginx/html/index.html

## o . é pra ele pegar a pastal local e achar arquivo dockerfile.
## Ex: docker image build -t ex-simple-build .
## ---------------------------------------------
## agora para executar o container eu rodo esse comando
## docker container run -p 80:80 ex-simple-build



