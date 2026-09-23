# 💬 IA para Jovens Curiosos — Leitora de Sentimentos (Google Colab)

[![GitHub Repo](https://img.shields.io/badge/GitHub-ia--para--jovens--curiosos%2Fleitora__de__sentimentos__colab-blue?logo=github)](https://github.com/ia-para-jovens-curiosos/leitora_de_sentimentos_colab)
[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ia-para-jovens-curiosos/leitora_de_sentimentos_colab/blob/master/sample.ipynb)

Um projeto para crianças treinarem sua própria Inteligência Artificial para ler frases digitadas e
adivinhar se estão **positivas**, **negativas** ou **neutras** — direto do navegador, sem instalar
nada.

Esta é a versão **Google Colab** do projeto
[`leitora_de_sentimentos_jupyter`](https://github.com/ia-para-jovens-curiosos/leitora_de_sentimentos_jupyter).
Como esse projeto não usa câmera nem depende do computador (é só Python puro), as duas versões
funcionam de forma idêntica — use esta se não quiser instalar nada na máquina.

## Como abrir

Clique no botão **"Abrir no Colab"** acima (ou abra `sample.ipynb` diretamente em
[colab.research.google.com](https://colab.research.google.com)) e execute as células de cima para
baixo, com `Shift + Enter`.

O notebook guia você por cinco passos:

1. **Dados de treino** — a turma monta, em grupo, as listas de palavras positivas e negativas
2. **Limpar a frase** — deixar o texto digitado pronto para comparar (minúsculas, sem pontuação)
3. **Classificar** — a função que decide se a frase é positiva, negativa ou neutra
4. **Testar** — conferir o robô com frases já conhecidas e ajustar as listas quando ele errar
5. **Modo estande** — deixar o programa rodando para o público testar na exposição

Há também uma célula opcional de **modo avançado**, comparando o robô caseiro com uma IA
profissional de verdade (Hugging Face).

## Como funciona por baixo dos panos

Diferente do projeto de Pedra-Papel-Tesoura, aqui **nada fica escondido**: as listas de palavras e a
função `classificar_sentimento()` ficam à vista, dentro do próprio notebook — é literalmente assim
que a turma "programa" a IA. O robô não entende a frase como uma pessoa; ele só reconhece as
palavras que estiverem nas listas de treino que a turma escreveu.

## ⚠️ Atenção: o Colab não guarda seu progresso sozinho

Se a turma passar tempo enriquecendo as listas de palavras, use **Arquivo → Salvar uma cópia no
Drive** antes de fechar a aba — assim vocês não perdem o que foi digitado quando a sessão do Colab
terminar.

## Ambiente

Este notebook já roda com o ambiente padrão do Google Colab — não precisa instalar nada. O arquivo
`requirements.txt` serve só de referência, caso queiram reproduzir o mesmo ambiente localmente (veja
a versão `leitora_de_sentimentos_jupyter`).
