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
      <img src="Imagens\1-degree_centrality.PNG height="500px" width="500px">
      <h4>Closeness Centrality</h4>
      <img src="../Imagens/2-closeness_centrality.png" height="500px" width="500px">
      <h4>Betwenness Centrality</h4>
      <img src="../Imagens/3-betweenness_centrality.png" height="500px" width="500px">
      <h4>Eigenvector Centrality</h4>
      <img src="../Imagens/4-eigenvector_centrality.png" height="500px" width="500px">
      <h4>Cumulative Density Function</h4>
      <img src="../Imagens/5-cumulative_density_function.png" height="500px" width="500px">
      <h4>Probability Desity Function</h4>
      <img src="../Imagens/6-probability_density_function.png" height="500px" width="500px">
      <h4>Indicator comparisons</h4>
      <img src="../Imagens/7-all.png" height="500px" width="500px">
      <h4>K-core</h4>
      <img src="../Imagens/8-k-core_sociopatterns.png" height="500px" width="500px">    
    </section>
  </li>
</ul>
<pre><h3>Link para vídeo com descrição dos resultados: <a href="#">#</a></h3></pre>