# Desafio - Estágio para Desenvolvedor na Liber

## Index

- [Desafio React Native - Liber](#Desafio-React-Native---Liber)
- [**Descrição**](#Descri%C3%A7%C3%A3o)
- [**Apresentação**](#Apresenta%C3%A7%C3%A3o)
- [**Avaliação**](#Avalia%C3%A7%C3%A3o)
- [**Envio**](#Envio)
- [**Observações Finais e Prazo**](#Observa%C3%A7%C3%B5es-Finais-e-Prazo)

## **Descrição**

Uma escola contratou sua agência de desenvolvimento de software para criar um sistema simples de gerenciamento de disciplinas e notas de seus alunos, conforme os requisitos abaixo:

- Disciplinas

  - Uma disciplina possui as seguintes propriedades:
    - Nome: nome
    - Critério de aprovação: criterio
    - Nota 1: g1
    - Nota 2: g2
    - Nota 3: g3
    - Nota 4: g4
    - Nota final: nota
    - Status final: status

- Notas

  - As notas seguem uma escala alfabética de A+ a F-, inclusive a nota final
  - Toda nota deve ser associada a um número real entre 0 e 10 (grau associado).

- Critérios

  - O sistema deve contar com os seguintes critérios de aprovação:
    - Critério I: Grau final é a média geométrica entre os quatro graus (onde o Grau 4 possui peso 2)
      - Caso haja um grau menor que 7: Grau final deve ser maior ou igual a 7 
      - Caso contrário: Grau final deve ser maior ou igual a 6
    - Critério II: Grau final é a média harmônica entre os dois maiores graus e deve ser maior ou igual a 6
    - Critério III: Grau final é a média ponderada (com pesos inteiro, linearmente crescentes com coeficiente linear 2 e passo 1) entre os três maiores graus 
      - Caso haja um grau menor que 5: Grau final deve ser maior ou igual a 8
      - Caso contrário: Grau final deve ser maior ou igual a 5
    - Critério IV:
      - Caso haja um grau menor que 3: Grau final é a média aritmética entre os quatro graus (onde o Grau 4 possui peso 3) e deve ser maior ou igual a 8
      - Caso contrário: Grau final é a média aritmética entre os três maiores graus e deve ser maior ou igual a 6
    - Critério V:
      - Caso haja um grau menor que 9: Grau final é a mediana dos quatro graus e deve ser maior do que 5
      - Caso contrário: Grau final é o inverso do menor grau
  - Toda disciplina deve estar associada a um dos critérios listados acima
  - Seu código deve ser robusto ao ponto de generalizar as operações realizadas, tornando assim, fácil a inclusão futura de novos critérios
  - O conceito de **peso** associado aos graus pode mudar com base no tipo de média utilizada na operação e cabe a você discernir as distinções

- Status final (Aprovado)

  - A aprovação de um aluno depende diretamente do critério de aprovação a que uma disciplina pertence e do grau/nota final desta.
  - O status final deve apresentar a estrutura de dados que você julgar adequada

## **Apresentação**

É obrigatório que além do código desenvolvido, exista uma documentação detalhando como você chegou na solução apresentada.

## **Avaliação**

A avaliação será centrada na sua capacidade de organização e arquitetura de software. Além disso, é obrigatória a implementação de testes automatizados em quantidade adequada (não peque por falta ou excesso) visando a garantia de qualidade de software.

## **Envio**

Você deverá fazer um fork desse repositório e enviar um pull request com a sua solução.

## **Observações Finais e Prazo**

O desafio deverá ser entregue em até 48 horas após o recebimento.
