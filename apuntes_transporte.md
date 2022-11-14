
# Apuntes del problema de transporte

## Casos desbalanceados:

- sum(s<sub>i</sub>) > sum(d<sub>j</sub>):
	- sum(x<sub>ij</sub>) <= s<sub>ij</sub> <br>**si fuera una restricción tipo = llegamos a una situación de no factibilidad pues no se satisface exactamente la demanda.**</br>
	- sum(x<sub>ij</sub>) = d<sub>ij</sub>, *j=1,2,3,..*
	- caso en que se permite sobresatisfacción de demandas:
		- sum(x<sub>ij</sub>) >= d<sub>ij</sub>, *j=1,2,3,..*

- mismo caso pero hay que enviar todo lo que se produce:
	- sum(x<sub>ij</sub>) = s<sub>ij</sub>
	- sum(x<sub>ij</sub>) >= d<sub>ij</sub>, *j=1,2,3,..*
*Notas del caso*: me obligan a enviar todo lo que se produce pero se tienen que enviar todo con demandas sobresatisfacidas.

- sum(s<sub>i</sub>) < sum(d<sub>j</sub>):
	- **Fuente artificial que suministra la demanda faltante para equilibrar el problema** <br>
s<sub>m+1</sub> = sum(d<sub>j</sub> - sum(s<sub>i</sub>)</br>
	- El modelo es el mismo del caso balanceado pero los coeficientes de costos desde s<sub>m+1</sub> son cero pues no hay transporte hacia la fuente.
