# Visual Áudio-Reativo no TouchDesigner

A ideia é mostrar como sinais sonoros podem ser transformados em elementos visuais dinâmicos.

<a href="https://imgbox.com/EYqtSVeS" target="_blank"><img src="https://thumbs2.imgbox.com/bf/fb/EYqtSVeS_t.gif" alt="image host"/></a>

## O que é áudio-reatividade?

Áudio-reatividade é a técnica de usar frequências, amplitudes e espectros sonoros para modificar parâmetros visuais em tempo real.
Neste projeto, o som atua como gatilho e controlador dos visuais.

## Como executar

* Instale o TouchDesigner

* Clone este repositório

* Abra o arquivo .toe no TouchDesigner.

* Ative seu microfone ou carregue um arquivo de áudio.

## Componente: Análise de Áudio (.tox)

Este componente captura áudio e traduz informações como amplitude e espectro de frequências em sinais que podem ser usados para controlar visuais.
Ele serve como a ponte entre o som e a imagem, permitindo que diferentes parâmetros visuais sejam animados de acordo com as características sonoras.

## Componente: Double Feedback

O Double Feedback é um recurso visual que utiliza o princípio de realimentação da imagem no TouchDesigner.
Na prática, ele funciona como uma “câmera apontada para a própria tela”: a imagem anterior é usada como insumo para gerar a próxima, criando padrões dinâmicos, caleidoscópicos e hipnóticos.

### Como funciona

* Um TOP Feedback captura o estado visual atual.

* Esse sinal é processado com transformações (escala, rotação, cor etc.).

* O resultado é reinserido no fluxo visual, gerando um loop acumulativo.

* No modelo double feedback, usamos duas camadas de feedback em paralelo ou alternadas, aumentando a complexidade visual.
