<div align="center">
<h1 align="center">Code Delivery</h1>
</div>

<p align="center">
  <a href="#-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<p align="center">
 <img  src="https://img.shields.io/static/v1?label=license&message=MIT&color=2ef4cc&labelColor=14061f" alt="License" />
  <img src="https://img.shields.io/github/repo-size/jhonatan-oliveiradev/code-delivery?label=forks&message=MIT&color=2ef4cc&labelColor=14061f" alt="Forks" />
  <img src="https://img.shields.io/github/stars/jhonatan-oliveiradev/code-delivery?label=stars&message=MIT&color=2ef4cc&labelColor=14061f" alt="Stars" />
</p>

<p align="center">
    <img src="../images/preview.png" alt="preview">
</p>

<p align="center">
  <img alt="" src=".github/logo-plane.svg" width="10%" />
</p>

<br>

<p align="center">
  <img alt="" src=".github/preview-desktop.png" width="100%" />
</p>

## 📄 Descrição:

### O que será desenvolvido?

- Sistema de entregas que permite visualizar em tempo real o veículo do entregador;
- Há possibilidade de múltiplos entregadores simultâneos;
- Serviço simulador que enviará a posição em tempo real de cada entregador;
- Os dados de cada entrega, bem como as posições, serão armazenadas no [Elasticsearch](https://www.elastic.co/pt/elasticsearch/) para futuras análises.

## 🆘 Principais Desafios:

### ❎ Para evitar perda de informação caso o serviço de backend fique indisponível por alguns momentos, não trabalharemos com REST.

### ✅ SOLUÇÃO: trabalharemos com o Apache Kafka para o envio e recebimento de dados entre os sistemas.

### ❎ Não é responsabilidade do serviço de backend persistir os dados no Elasticsearch. Logo, como armazenar as informações no Elasticsearch?

### ✅ SOLUÇÃO: Utilizaremos o Kafka Connect que também consumirá os dados do simulador e fará a inserção no Elasticsearch.

### ❎ Precisamos exibir em tempo real a localização de cada entregador.

### ✅ SOLUÇÃO: Trabalharemos com websockets (O backend receberá os dados do simulador, e enviará as posições para o frontend via websocket).

<p align="center">
<img src="../images/esquema.png" align="center" alt="dinâmica do sistema"/>
</p>

## 🚀 Tecnologias:

Esse projeto foi desenvolvido com as seguintes tecnologias:

### Simulador: [Golang](https://www.golang.org/) 🌀

### Backend: Nest.js & Mongo 🐯🍃

### Frontend: React & Material UI ⚛️

### [Kafka & Kafka Connect](https://kafka.apache.org/intro/) 🔅

### [Elasticsearch](https://www.elastic.co/pt/elasticsearch/) 🔷

### Doker & Kubernetes 🐋

### Istio, Kiali, Prometheus & Grafana.

## 🚧 Projeto:

### Em construção!

## 🎨 Inspiração:

### Projeto desenvolvido durante a Imersão Full Stack\_ && Full Cycle.

## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

<hr>

Made by Jhonatan Oliveira.
