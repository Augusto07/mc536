# Aluno
* 200025: José Augusto Nascimento Afonso Marcos

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução
~~~cypher
MATCH (:Categoria{id: 'Serviços'})<-[:Pertence]-(r)
RETURN r
~~~

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução
~~~cypher
MATCH (m:Marcador) 
MATCH (c:Categoria{id:'Serviços'})
	WHERE (m)-[*]->(c)
RETURN m
~~~