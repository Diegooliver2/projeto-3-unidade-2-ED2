<h1>Estrutura de Dados 2</h1>
<h2>Trabalho 3 - Unidade 2 | Grafos Dirigidos - Links das páginas Wikipedia</h3>
<h2>Componentes:</h2>
<ul>
  <li>Diego de Oliveira Silva</li>
  <li>Fernando Manoel de Queiroz Neto</li>
  <li>Luiz Fernando Tavares</li>
</ul>
<h2>Para reprodução do código:</h2>
<ul>
  <li>Versão do NetworkX utilizada: 2.6.3</li>
  <li>
    <ul>
      <li><h4>Bibliotecas e Pacotes utilizados:</h4></li>
      <li>operator import itemgetter</li>
      <li>networkx</li>
      <li>wikipedia</li>
      <li>matplotlib.pyplot</li>
      <li>matplotlib.patches</li>
      <li>collections import deque</li>
      <li>numpy</li>
      <li>seaborn</li>
      <li>pandas</li>
    </ul>
  </li>
  <li>
    <ul>
      <li><h4>Passo a passo de execução</h4></li>
      <li>
        <h5>Escolha da "Semente"</h5>
        <p>
          Você escolhe o título de uma página da Wikipedia, para a partir dela uma network ser criado, tendo por camadas da rede as páginas linkadas a página acessada pelo algoritmo durante a verredura. Neste projeto limitamos a menos que duas camadas a partir da semente.
        </p>
      </li>
      <li>
        <h5>Escolhas das paradas</h5>
        <p>
          Na tupla STOPS deverá ser adicionados títulos de páginas que não deverão gerar ramificações na rede, para evitar a geração de repetições de acessos, escalonamento de ramificações e acesso a páginas que estão longe da ideia central da página semente.
        </p>
      </li>
      <li>
        <h5>Entendimento dos resultados</h5>
        <p>
          Depois de definir os parâmetros necessários para a execução do algoritmo, ele deverá gerar os gráficos em imagens no formato png, que são resultados obtidos através do estudo de direct networks de página da Wikipedia; Estes são referentes aos temas Degree, Closeness, Betwenness, Eigenvector centrality, Centrality distributions e Core decomposition. 
        </p>
      </li>
    </ul>
  </li>
  <li>
    <section>
      <h4>Resultados do Projeto</h4>
      <p>
        Analisamos a rede (grafo) do site wikipedia tendo como semente a página com o título "Copa do Mundo FIFA". Realizamos uma limpeza nos nós dessa rede, eliminando duplicações, extraimos o arquivo "cmf.graphml" e em seguida o usamos para plotar e analisar os indicadores à seguir.
      </p>
      <h4>Degree Centrality</h4>
      <img src="/Imagens/1-degree_centrality.PNG" height="400px">
      <h4>Closeness Centrality</h4>
      <img src="/Imagens/2-closeness_centrality.PNG" height="400px">
      <h4>Betwenness Centrality</h4>
      <img src="/Imagens/3-betweenness_centrality.PNG" height="400px">
      <h4>Eigenvector Centrality</h4>
      <img src="/Imagens/4-eigenvector_centrality.PNG" height="400px">
      <h4>Cumulative Density Function</h4>
      <img src="/Imagens/5-cumulative-density-function.PNG" height="400px">
      <h4>Probability Desity Function</h4>
      <img src="/Imagens/6-probability-density_function.PNG" height="400px">
      <h4>Indicator comparisons</h4>
      <img src="/Imagens/7-all.PNG" height="400px">
      <h4>K-core</h4>
      <img src="/Imagens/8-k-core_sociopatterns.PNG" height="400px">    
    </section>
  </li>
</ul>
<pre><h3>Link para pasta com os gráficos no drive: <a href="https://drive.google.com/drive/folders/1v-Vcb8yu-hCSTb-12baKazKUKs9bBoCN?usp=sharing">https://drive.google.com/drive/folders/1v-Vcb8yu-hCSTb-12baKazKUKs9bBoCN?usp=sharing</a></h3></pre>
<pre><h3>Link para vídeo com descrição dos resultados: <a href="https://www.loom.com/share/c611f8dba0644f34b9092a77dcc29f70">https://www.loom.com/share/c611f8dba0644f34b9092a77dcc29f70</a></h3></pre>
<h2>Visualizações de análise de rede:</h2>
<ul>
  <li>
    <section>
      <h4>Métricas para criação das comunidades</h4>
      <p>
        Foi utilizado o arquivo cmf.graphml no programa Gephi, nele extraímos as informações estatísticas da rede como os valores do Grau médio (degree, indegree, outdegree), Modularidade (modularity_class) e o valor de Excentricidade (eccentricity).<br/>
        Essas informações foram extraídas como os arquivos U3Finalnodes.csv e U3Finaledges.csv, inserimos o U3Finalnodes.csv em um DataFrame e dele extraimos um histograma utilizando a coluna ‘degree’ do arquivo:
      </p>
      <img src="/Imagens/histograma.PNG" height="400px">
      <p>
        A partir do histograma criamos uma coluna para classificar os dados da coluna ‘degree’ em seis grupos, A, B, C, D, E e F, onde se:<br/>
        <strong>
          Grau menor que 70 -> Grupo A (Roxo)<br/>
          Grau entre 70 e 140 -> Grupo B (Azul)<br/>
          Grau entre 140 e 210 -> Grupo C (Verde)<br/>
          Grau entre 210 e 280 -> Grupo D (Rosa)<br/>
          Grau entre 280 e 490 -> Grupo E (Laranja)<br/>
          Grau maior 490 -> Grupo F (Verde escuro)<br/>
        </strong>
        Depois inserimos a coluna no dataframe e exportamos como U3Final2nodes.csv, que foi inserido no gephi para analisar o gráfico com a nova métrica que criamos, ‘group’, obtivemos o seguinte gráfico:
      </p>
      <img src="/Imagens/networkGit.PNG" height="400px">
    </section>
  </li>
  <li>
    <section>
      <h4>Retina</h4>
      <p>
        Para visualizar a rede no Retina, será necessário acessar o link <a href="https://ouestware.gitlab.io/retina/beta/#/">https://ouestware.gitlab.io/retina/beta/#/</a> e adicionar manualmente o arquivo U3.graphml.<br/>
      </p>
      <img src="/Imagens/networkRetina.PNG" height="400px">
    </section>
  </li>
  <li>
    <section>
      <h4>Gesphisto</h4>
      <p>
        Depois utilizamos o site <a href="https://jacomyma.github.io/gephisto/">Gephisto</a>, lá foi inserido o arquivo U3.graphml e foi obtido a seguinte imagem<br/>
      </p>
      <img src="/Imagens/networkGephisto.jpeg" height="400px">
    </section>
  </li>
<ul>
<pre><h3>Link para o network no github pages: <a href="https://diegooliver2.github.io/projeto-3-unidade-2-ED2/network/index.html">https://diegooliver2.github.io/projeto-3-unidade-2-ED2/network/index.html</a></h3></pre>