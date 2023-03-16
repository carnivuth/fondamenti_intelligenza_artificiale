- informazione sulla conoscenza applicata disponendo di piu possibilità
- #### STRATEGIE NON INFORMATE
	- strategie che non sono a conoscenza del dominio applicativo
- #### STRATEGIE INFORMATE
	- strategie che conoscono il dominio applicativo
- #### CRITERI DI VALUTAZIONE
	- ##### completezza
	  id:: 640b1c21-d260-46d3-bc78-cb50f97d63cc
		- la soluzione trovata è corretta o meno
	- DONE completare criteri di valutazione
	- ##### complessita spaziale
	  id:: 640b1c39-c598-41a4-8a47-e7417df9bbb8
		- quanta memoria occupa la strategia
	- ##### complessita temporale
	  id:: 640b1c46-7eb7-4316-a186-682e4ef1557d
		- quanto tempo impiega la strategia
	- ##### ottimalita
	  id:: 640b1c4b-fe83-4c82-be38-9c458cd40b5d
		- la soluzione trovata è quella ottimale
- #### PROFONDITA
	- la profondita del nodo di partenza è 0 e la profondita di un nodo x è quella del suo genitore +1
- #### STRATEGIA BREADTH-FIRST
  id:: 640b1d0a-beb1-4247-b1ba-59bf87d88dec
	- espande sempre i nodi meno profondi dell'albero
	- ((640b1c46-7eb7-4316-a186-682e4ef1557d)) e ((640b1c39-c598-41a4-8a47-e7417df9bbb8)) b^d
		- complessità esponenziale di esecuzione
	- trova sempre la soluzione ottimale se il costo è indicato come la profondità del goal
- #### STRATEGIA A COSTO UNIFORME
	- viene selezionato per l'espansione il nodo a costo minimo
	- il goal test viene effettuato prima dell'espansione del nodo
- #### STRATEGIA DEPTH-FIRST
	- espande i nodi piu profondi
		- a parita di profondita la selezione è arbitraria
	- ((640b1c39-c598-41a4-8a47-e7417df9bbb8)) ridotta rispetto a ((640b1d0a-beb1-4247-b1ba-59bf87d88dec)) non è necessario tenere attivi tutti i rami dell'albero una volta esplorati
	- ![image.png](../assets/image_1678451291443_0.png)
	- possibile gestirla con uno stack
	- ((640b1c21-d260-46d3-bc78-cb50f97d63cc))
		- la strategia non è completa, in caso di rami di profondità infinita o loop
		- un workaround possibile è quello di imporre un limite alla profondità massima raggiungibile
	- ((640b1c46-7eb7-4316-a186-682e4ef1557d))
		- se la profondita dell' albero è molto maggiore della profondita della soluzione tempi lunghissimi
	- ((640b1c39-c598-41a4-8a47-e7417df9bbb8))
		- lineare con la dimensione dell'albero
	- ((640b1c4b-fe83-4c82-be38-9c458cd40b5d))
		- la strategia non è ottimale
	- ![image.png](../assets/image_1678452245301_0.png)
	-
	-
	-
	-