## Resumo do artigo "On the Testability of Artificial Intelligence and Machine Learning Systems"
##### R. Sangwan, Y. Badr, S. Srinivasan and P. Mukherjee. DOI: 10.1109/MC.2021.3132710
---
O artigo fala sobre preocupações com a testabilidade de sistemas de inteligência artificial e de aprendizado de máquina.
Ele começa falando sobre a os três maiores desafios da checagem de comportamento de IA:

- Falta de um modelo para previsão que não siga o modelo de aprendizado de máquina
- Dificuldade em determinar se os dados de treinamento são suficientes para representar todo o conjunto de entradas
- Observar todos os estados internos possíveis durante a execução é imprático

Porém, mesmo com esses desafios, o artigo mostra que a checagem de comportamento de IA é uma tarefa muito importante, pois impede desde perda de investimento a perda de vidas.
Então, ele fala sobre os diferentes níveis de granularidade em que se pode testar um sistema de IA:
- Teste de entrada
- Teste de modelo
- Teste de integração
- Teste de sistema

Listando também diferentes análises que podem ser feitas em cada um desses testes

Mais à frente, o artigo fala sobre preocupações que os desenvolvedores devem ter ao projetar um sistema de IA:

- Evitar que o sistema complete seu objetivo com efeitos colaterais negativos
- Evitar que o sistema ganhe sua recompensa sem realizar a tarefa (reward hacking)
- Evitar comportamento indesejado causado por amostras limitadas
- Garantir que o sistema possa aprender novos comportamentos sem consequências indesejadas
- Garantir que o sistema possa continuar a operar como pretendido em um ambiente

O artigo também sugere o uso de um monitor de teste com três entradas — entrada, saída e estado interno — para melhorar a testabilidade do sistema. Ele demonstra como poderia ser aplicado de forma real em uma plataforma de empréstimos que faria a previsão da concessão do empréstimo avaliando os riscos. A plataforma conta com monitoramento das mudançãs de comportamento e uma ferramenta de auto-diagnóstico que periodicamente realiza testes paraa verificar o estado. Por fim, o artigo enumera táticas de design que têm como pilares principais a supervisão escalável, exploração segura e robustez em relação ao desvio de distribuição