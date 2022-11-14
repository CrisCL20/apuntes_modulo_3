
# Apuntes del problema de transporte

## Casos desbalanceados:

- sum(s<sub>i</sub>) > sum(d<sub>j</sub>):
	- sum(x<sub>ij</sub>) <= s<sub>ij</sub> <br></br>**si fuera una restricción tipo = llegamos a una situación de no factibilidad pues no se satisface exactamente la demanda.**
	- sum(x<sub>ij</sub>) = d<sub>ij</sub> *j=1,2,3,..*
	- caso en que se permite sobresatisfacción de demandas:
		- sum(x<sub>ij</sub>) >= d<sub>ij</sub> *j=1,2,3,..*

- mismo caso pero hay que enviar todo lo que se produce:
	- sum(x<sub>ij</sub>) = s<sub>ij</sub>
	- sum(x<sub>ij</sub>) >= d<sub>ij</sub> *j=1,2,3,..*
