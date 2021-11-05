# Aluno
* 200025: José Augusto Nascimento Afonso Marcos

## Modelo simplificado de conceito do grafo de conhecimento

> ![Diagrama simplificado do grafo](images/conceito.png)

## Explicação

> Nosso banco de dados poderia ser facilmente transformado em um grafo de conhecimento seguindo o esquema básico: Recurso --> Propriedade --> Valor. Podemos fazer esse tipo de grafo pois os dados do nosso banco de dados são altamente hierarquizados, onde muitos dos dados de cada nó apontam para outros nós seguindo uma propriedade expecífica (por exemplo Time -> Joga -> Jogadora), o que de fato é a aplicação de um valor sendo usado novamente como um recurso. Usando a dbpedia como exemplo, poderíamos também transformar nosso grafo em um esquema com N-Triples, com links para cada um dos atributos até chegarmos em atributos primitivos (como número de gols, idade da jogadora, que são inteiros por exemplo) que não necessitam de links, sendo tratados somente como valor. Abaixo está um exemplo real, onde o grafo é montado utilizando valores como recursos até atingir os gols da jogadora, representados com um tipo primitivo (inteiro).

> ![Exemplo de Grafo](images/exemplo.png)

## Perguntas de Pesquisa/análise

> Pergunta 1
> * Qual foi a jogadora que mais marcou gols pela seleção X no ano Y?

> Pergunta 2
> * 

> Pergunta 3
> *