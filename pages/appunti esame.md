- ## EURISTICA AMMISSIBILE
	- un euristica è ammissibile se è sempre minore del costo effettivo tra un nodo e il goal (ottimistica.)
- ## CSP - FORWARD CHECKING
	- si considerano solo i vincoli legati alla variabile assegnata
	-
- ## RICERCA A*
	- nella ricerca si espande fino a che non ci sono piu nodi da espandere
- ## RICERCA AD APPROFONDIMENTO ITERATIVO
	- ripete la ricerca depth first con limiti di profondita crescente
	- ```
	  depth=0
	  do{
	  result=depthfirstsearch(depth);
	  depth ++;
	  }while(result!=success  && result!=failure);
	  ```
	- vengono espansi nodi piu volte
	- mette insieme depth first  e breat