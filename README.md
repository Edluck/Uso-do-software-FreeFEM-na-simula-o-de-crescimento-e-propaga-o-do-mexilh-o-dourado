# Modelagem da Propagação do Mexilhão-Dourado (*Limnoperna fortunei*) em Ambientes Aquáticos

Este repositório contém o código e os arquivos necessários para a simulação da propagação do mexilhão-dourado em ambientes aquáticos usando o **FreeFEM** e o **Método dos Elementos Finitos (MEF)**. O objetivo do projeto é modelar e prever o comportamento e dispersão dessa espécie invasora em diferentes cenários de rios e lagos, permitindo insights para o controle e mitigação de sua invasão.

---

## Índice
- [Introdução](#introdução)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Método dos Elementos Finitos](#método-dos-elementos-finitos)
- [FreeFEM](#freefem)
- [Configuração e Execução do Projeto](#configuração-e-execução-do-projeto)
- [Experimentos Realizados](#experimentos-realizados)
- [Como Contribuir](#como-contribuir)
- [Licença](#licença)

---

## Introdução
O mexilhão-dourado (*Limnoperna fortunei*) é uma espécie invasora que causa sérios danos ambientais e econômicos ao colonizar infraestruturas aquáticas, como barragens e sistemas de abastecimento de água. Este projeto visa modelar a propagação dessa espécie usando um sistema de equações diferenciais que leva em conta:
- A densidade de larvas, mexilhões adultos e algas (principal fonte de alimento).
- O fluxo do ambiente aquático, como a velocidade e direção da correnteza.
  
O modelo é resolvido numericamente usando o **Método dos Elementos Finitos (MEF)** implementado no software **FreeFEM**.

---

## Tecnologias Utilizadas
- **[FreeFEM](https://freefem.org/)**: Software de código aberto para simulações numéricas com métodos de elementos finitos.
- **Linguagem**: O código é escrito na linguagem de script própria do FreeFEM.
- **Ferramentas de Visualização**: Os resultados podem ser visualizados e analisados em softwares como Paraview.

---

## Método dos Elementos Finitos
O **Método dos Elementos Finitos (MEF)** é uma técnica numérica para resolver problemas de equações diferenciais parciais, dividindo o domínio do problema em pequenos pedaços chamados **elementos finitos**. No contexto deste projeto, o MEF é utilizado para resolver as equações que descrevem:
- O transporte e dispersão das larvas de mexilhões ao longo da correnteza.
- A interação entre mexilhões adultos e algas, que representa uma relação predador-presa.

Ao dividir o domínio aquático em uma malha de elementos, o MEF permite aproximar as soluções em cada elemento, possibilitando a simulação de ambientes complexos, como rios e lagos com geometrias irregulares.

---

## FreeFEM
**FreeFEM** é uma ferramenta de código aberto para a solução numérica de problemas de equações diferenciais parciais em uma ampla variedade de domínios. Ele é especialmente adequado para resolver problemas com o MEF, devido à sua capacidade de:
- Gerar e manipular malhas de elementos finitos.
- Resolver sistemas de equações diferenciais complexos de forma eficiente.
  
No projeto, o FreeFEM é usado para implementar o modelo de equações do mexilhão-dourado, considerando o transporte convectivo, a difusão e as interações biológicas (como crescimento e predação).

### Instalação do FreeFEM
Para instalar o FreeFEM, consulte a [documentação oficial](https://freefem.org/download/). Ele está disponível para Windows, macOS e Linux.

---

## Configuração e Execução do Projeto
### Pré-requisitos
- Instale o FreeFEM.
- Clone este repositório:
  ```bash
  git clone https://github.com/seu-usuario/seu-repositorio.git
  cd seu-repositorio

