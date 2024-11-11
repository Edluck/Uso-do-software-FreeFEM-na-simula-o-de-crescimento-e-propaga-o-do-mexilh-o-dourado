# Modelagem da Propagação do Mexilhão-Dourado (*Limnoperna fortunei*) em Ambientes Aquáticos

Este repositório contém o código e os arquivos necessários para a simulação da propagação do mexilhão-dourado em ambientes aquáticos usando o **FreeFEM** e o **Método dos Elementos Finitos (MEF)**. O objetivo do projeto é modelar e prever o comportamento e dispersão dessa espécie invasora em diferentes cenários de rios e lagos, permitindo insights para o controle e mitigação de sua invasão.

---

## Índice
- [Introdução/Resumo](#introdução-resumo)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Método dos Elementos Finitos](#método-dos-elementos-finitos)
- [FreeFEM](#freefem)
- [Configuração e Execução do Projeto](#configuração-e-execução-do-projeto)
- [Experimentos Realizados](#experimentos-realizados)

---

## Introdução/Resumo
- O mexilhão-dourado ({\it Limnoperna fortunei}), um molusco bivalve invasor nativo do sudeste asiático que adentrou o ecossistema Brasileiro, tem causado sérios danos ambientais e econômicos no Brasil, especialmente em rios que possuem hidroelétricas e/ou pisciculturas. A compreensão do ciclo de vida, da sua forma larval e adulta, e da interação desse organismo com seu principal alimento, a alga, é fundamental para o desenvolvimento de estratégias de controle e mitigação da população desse molusco, tendo em vista que medidas de controle atuais mostram-se ineficazes. Este subprojeto analisa essa relação por meio de um modelo matemático predador-presa, através da utilização do método dos elementos finitos via software FreeFEM, que soluciona equações diferenciais ordinárias 2D e 3D. As simulações visam investigar como diferentes combinações de parâmetros físicos do modelo influenciam a dispersão do mexilhão em diferentes ambientes criados para essas simulações e também como o uso de diferentes funções dentro do FreeFem podem influenciar na otimização do tempo de execução do algoritmo e na solução, contribuindo para o entendimento de sua dinâmica populacional e fornecendo subsídios para a elaboração de medidas de controle mais eficazes.

---

## Tecnologias Utilizadas
- **[FreeFEM](https://freefem.org/)**: Software de código aberto para simulações numéricas com métodos de elementos finitos.
- **Linguagem**: O código é escrito na linguagem de script própria do FreeFEM, FreeFem++.
- **Ferramentas de Visualização**: Os resultados podem ser visualizados e analisados no **[Paraview](https://www.paraview.org/)**.

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
Para instalar o FreeFEM, consulte a [documentação oficial](https://doc.freefem.org/documentation/index.html). Ele está disponível para Windows, macOS e Linux.

---
## Experimentos Realizados
- Observar a pasta Experimentos deste Git, Nele existem 4 experimentos com diferentes formatos de domínio, detalhado tanto no relatório final e no artigo aqui disponibilizados.
---

## Configuração e Execução do Projeto
### Pré-requisitos
- Instale o FreeFEM.
- Clone este repositório:
  ```bash
  git clone https://github.com/seu-usuario/seu-repositorio.git](https://github.com/Edluck/Uso-do-software-FreeFEM-na-simula-o-de-crescimento-e-propaga-o-do-mexilh-o-dourado.git
  cd Uso-do-software-FreeFEM-na-simula-o-de-crescimento-e-propaga-o-do-mexilh-o-dourado.git

