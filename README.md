## ASSINplus
Repositório com dados da partição de teste do *dataset* ASSIN com anotação extra para atributos do texto.

## Atributos 

A anotação extra está dividida em dois tipos: atributos das sentenças e atributos dos pares de sentenças. A primeira considera o texto em si, a segunda uma relação entre os atributos das sentenças para cada par.   

### Atributos das sentenças

<ol>
  <li><strong>Comprimento:</strong> Quantidade de tokens da sentença.</li>
  <li><strong>Entidade nomeada:</strong> Entidades nomeadas presentes nas sentenças anotadas manualmente.
      Entre elas constam nomes de esportistas, políticos e instituições.</li>
  <li><strong>Tópico:</strong> Os tópicos identificados foram: esporte, entretenimento, produtos de tecnologia, economia e mercado, política, saúde, notícias mundiais (notícias de países do mundo exceto o Brasil e Portugal), ciência e outras notícias. A cada sentença foi atribuído apenas um tópico. A anotação foi feita manualmente para as sentença individualmente considerando-se apenas a informação contida em cada uma.</li>
  <li><strong>Dependência sintática:</strong> Estrutura de dependência sintática de acordo com o modelo de Universal Dependency anotada de forma automatizada pelo parser sintático do SciPy.</li>
</ol>

### Atributos dos pares

<ol>
  <li><strong>Proporção do comprimento:</strong> Relação do comprimento entre as duas sentenças. Tomamos a diferença de comprimento dividido pelo comprimento médio das sentenças.</li>
  <li><strong>Proporção de entidade nomeada em ambas sentenças:</strong> Proporção de entidades nomeadas presentes nas duas sentenças em relação a soma de entidades do par.</li>
  <li><strong>Relação entre tópicos:</strong> Valor binário no qual foi atribuído 0 se o tópico de cada sentença do par é distinto e 1 caso o tópico seja o mesmo.</li>
  <li><strong>Semelhança de dependência sintática:</strong> Mesma estrutura sintática do primeiro nível de dependência a partir da raiz. São observados quantos nós filhos a raiz possuí nas sentenças e feita uma proporção entre aqueles que são iguais em ambas (possuem o mesmo rótulo sintático) e todos do par. Na prática isso significa que se a raiz tiver os mesmos nós filhos sintáticos, o valor será 1. Caso as raízes das sentenças tenham filhos distintos, o valor é menor, chegando a 0 para nenhuma intersecção de filhos sintáticos.</li>
</ol>

### Informações adicionais
  
Mais informações sobre o ASSIN podem ser encontradas em: http://www.nilc.icmc.usp.br/assin/

Os scripts utilizados na *share task* estão disponíveis em: https://github.com/erickrf/assin

O *dataset* completo está disponível também na plataforma do Hugging Face, com acesso pelo link: https://huggingface.co/datasets/assin


## Referências

### .bib

Referência ASSINplus (anotação extra disponibilizada neste repositório)

<pre><code>@phdthesis{rodrigues2018similarity,
    title={Avaliação de representações embeddings para similaridade sentencial no Portugu{\^e}s},
    author={Rodrigues, Ana Carolina},
    year={2022},
    school={Universidade de S{\~a}o Paulo}
  }</code></pre>

Referência dataset ASSIN
<pre><code> @inproceedings{fonseca2016assin,
  title={ASSIN: Avaliacao de similaridade semantica e inferencia textual},
  author={Fonseca, E and Santos, L and Criscuolo, Marcelo and Aluisio, S},
  booktitle={Computational Processing of the Portuguese Language-12th International Conference, Tomar, Portugal},
  pages={13--15},
  year={2016}
}</code></pre>


