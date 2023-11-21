<div align="center" style="display: inline_block">
  <img align="center" alt="VS" src="https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white" />
  <img align="center" alt="Linux" src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img align="center" alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img align="center" alt="Overleaf" src="https://img.shields.io/badge/Overleaf-47A141?style=for-the-badge&logo=Overleaf&logoColor=white" />
  <img align="center" alt="Latex" src="https://img.shields.io/badge/latex-%23008080.svg?style=for-the-badge&logo=latex&logoColor=white" />
</div>

<br>
<h1 align="center">
    <a>
        <img alt="Banner" title="#Banner" style="object-fit: fill; height:200px;" src="imgs/github-header-image.png"/>
    </a>
</h1>

# Observações:

<div align="justify">
  
É amplamente reconhecido que a teoria dos grafos oferece uma aplicabilidade extensa a uma ampla variedade de problemas emergentes em diversas areas e disciplinas. Nesse contexto, como parte do desenvolvimento acadêmico, cada aluno é incumbido de identificar um problema específico que seja suscetível de modelagem por meio de um grafo. Logo, cada um deve então propor e aplicar um ou mais algoritmos adequados para abordar uma questão de pesquisa
relacionada a esse problema. 

É importante ressaltar que, embora um mesmo problema possa ser selecionado por mais de um aluno, a seleção do algoritmo para sua resolução deve ser única. Este requisito visa a estimular a diversidade de abordagens e soluções, promovendo um ambiente de aprendizado e pesquisa amplo. Para facilitar a organização e evitar potenciais problemas na avaliação, será empregado o canal do Telegram para divulgar as associações entre os problemas escolhidos e os algoritmos selecionados por cada aluno. Isso garantirá que cada abordagem única seja devidamente documentada e avaliada, contribuindo para a qualidade do processo de aprendizado e pesquisa neste contexto acadêmico.
  
Cada problema abordado deve ser explicado em detalhes por um artigo, o qual deve contemplar no mínimo: Resumo, Introdução, Contextualização, Trabalhos Correlatos, Resultados, Considerações finais e trabalhos futuros. Nesse modelo, é impressindível que as referencias sejam parte de exploração sobre o tema. Logo, de imporância para esse ponto e considere citar bons trabalhos e livros que tratam sobre o problema abordado.

Considerando o artigo a ser apresentado, a parte de maior relevância é a seção de resultados, que deve detalhar minuciosamente os passos realizados, os experimentos executados e resultados obtidos. Nessa seção, os resultados devem não somente ser apresentados mas também discutidos, comparados, relacionados ou evidenciados para conectalos aos objetivos propostos. Nesse momento atentem-se para deixar o texto claro e muito bem detalhado.

Ao citar o algoritmo utilizado, introduza como referência para o mesmo o link para o git. Para tanto, inclua a citação no seu bibtex e faça a referencia conforme normas de citação para artigos. Tais normas podem obdecer as internacionais ou as apresentadas na ABNT. 

Quanto ao git e algoritmo. Como será exigida a construção de um artigo, fica dispensado a necessidade de construção de um README.mb para detalhar o processo. Contudo, qualquer item associado a linguagem deve ser devidamente reportado no artigo, ou seja, qualquer uso de bibliotecas deve ser expressa em detalhes no documento entregue.

No AVA, cada aluno deve enviar apenas o PDF do artigo resultante. A partir dele considerase que o necessário a explicação, observação e execução já serão bem tratados e explicados. Ademais, no artigo preze a definição de pseudo algoritmos e apresente o mesmo seguindo os padrões de um artigo científico padrão.

O modelo de artigo a ser utilizado será o IEEE Conference Template disponível no Overleaf através do [link](https://www.overleaf.com/latex/templates/ieee-conference-template/grfzhhncsfqn).

</div>

## Modelagem do Problema:

**1. Vértices:** Cada jogador no banco de dados é representado como um vértice no grafo.

**2. Arestas:** As arestas são estabelecidas entre jogadores de posições que normalmente interagem em campo (por exemplo, atacante com meio-campista, meio-campista com lateral, etc.). 

**3. Pesos das Arestas:** O peso de cada aresta é determinado com base na diferença ou na soma dos "overalls" dos jogadores conectados. O "threshold" mencionado seria um critério para estabelecer essas arestas. Por exemplo, se a soma dos "overalls" dos dois jogadores exceder um determinado valor (o threshold), uma aresta é criada entre eles.

### Algoritmos e Solução:

**1. Criação do Grafo:** Primeiramente, você criaria o grafo com base nos dados disponíveis, conectando jogadores conforme o critério estabelecido.

**2. Análise de Redes:** Você pode usar algoritmos de análise de redes para identificar padrões importantes. Por exemplo:

   - **Centralidade:** Identificar jogadores que são "centrais" em várias combinações, indicando sua versatilidade ou importância na equipe.
   - **Clusters ou Comunidades:** Detectar grupos de jogadores que frequentemente formam boas combinações entre si.

**3. Identificação de Perfis de Jogadores:** Com base nas conexões estabelecidas, você pode identificar tipos específicos de jogadores. Por exemplo, um lateral que frequentemente atinge o threshold com atacantes pode ser classificado como "ofensivo".

### Considerações Adicionais na Modelagem:

- **Seleção de Estatísticas:** Além do "overall", você pode considerar outras estatísticas relevantes para a posição (como passe, velocidade, finalização) para refinar a análise.
  
- **Definição de Thresholds:** O valor do threshold pode variar de acordo com a posição e a estratégia de jogo. Por exemplo, para um time que valoriza a defesa, o threshold para relações defensivas pode ser mais alto.

- **Visualização:** Utilizar ferramentas de visualização de grafos para interpretar as relações e identificar padrões significativos.

- **Análise Temporal:** Se você tiver dados ao longo do tempo, pode analisar como as relações entre jogadores mudam ao longo das temporadas.




### Conclusão:

Esta abordagem permite uma análise sofisticada das interações entre jogadores e pode revelar insights sobre dinâmicas de equipe, compatibilidade entre jogadores e identificar jogadores-chave em diferentes estratégias de jogo. A aplicação de técnicas de análise de redes e a escolha cuidadosa das estatísticas a serem consideradas são fundamentais para o sucesso desta modelagem.


    'CB': 'Zagueiro Central',
    'LB': 'Zagueiro Esquerdo',
    'RB': 'Zagueiro Direito',
    'RWB': 'Lateral Direito',
    'LWB': 'Lateral Esquerdo',
    'CDM': 'Meia-Central', 'CM': 'Meia-Central', 'CAM': 'Meia-Central',
    'ROM': 'Meia-Direita', 'RM': 'Meia-Direita', 'RWM': 'Meia-Direita', 'RW': 'Meia-Direita',
    'LOM': 'Meia-Esquerda', 'LM': 'Meia-Esquerda', 'LWM': 'Meia-Esquerda', 'LW': 'Meia-Esquerda',
    'LF': 'Ponta-Esquerda', 'LS': 'Ponta-Esquerda',
    'ST': 'Atacante', 'CF': 'Atacante',
    'RF': 'Ponta-Direita', 'RS': 'Ponta-Direita',

Mudanças Necessárias:

Parte 1:

- Agrupar as posições gerais.

- Podar aproximadamente 100 players por posição com mais overall do .csv:
    - Atacantes : 33/33/33 : atacantes, pontas direitas e pontas esquerdos
    - Meias : 33/33/33 : meia centrais, direitos e esquerdos
    - Zagueiros : 33/33/33 : zagueiros centrais, direitos e esquerdos
    - Laterais : 50/50 : laterais direitos e esquerdos

- Ciar um Thresshold para link de cada posição.
    - Criar política de conexões (zagueiro liga com meia e lateral, etc)

Parte 2:

- Criar 'Cluster de maior conectividade':
    - Avaliar quantos jogadores tem de cada posição.
    - Qual a maior qntd de posição, (após analisar o treshold) 
        - Ex: Mais atacante e mais meias, 
        - Verifico se a conectividade é real (atacantes são mais relevantes)
    ou
    - A partir do 'maior cluster' pegar os 'top k' mais conectados e verificar se fazem parte do mesmo time ou qual a qntd relacionada ao mesmo time.
        - Verificar se a base do jogo tendencia algo time e se isso esta ligado ao cluster.


