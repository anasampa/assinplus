## ASSINplus
**Breve descrição:** Repositório com dados da partição de teste do *dataset* ASSIN anotado para outros atributos.

## Atributos 

### Atributos das sentenças

<ol>
  <li><strong>Comprimento:</strong> Quantidade de tokens da sentença.</li>
  <li><strong>Entidade nomeada:</strong> Entidades nomeadas presentes nas sentenças anotadas manualmente.
      Entre elas constam nomes de esportistas, políticos e instituições.</li>
  <li><strong>Tópico:</strong> Os tópicos identificados foram: esporte, entretenimento, produtos de tecnologia, economia e mercado, política, saúde, notícias mundiais (notícias de países do mundo exceto o Brasil e Portugal), ciência e outras notícias. A cada sentença foi atribuído apenas um tópico. A anotação foi feita manualmente para as sentença individualmente considerando-se apenas a informação contida em cada uma.</li>
  <li><strong>Dedependência sintática:</strong> Estrutura de dependência sintática de acordo com o modelo de Universal Dependency anotada de forma automatizada pelo parser sintático do SciPy.</li>
</ol>


## Acesso rápido

Mais informações sobre o *dataset* original podem ser encontradas em: http://www.nilc.icmc.usp.br/assin/

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


