# cycless

A collection of algorithms to analyze a graph as a set of cycles.

Some codes come from [https://github.com/vitroid/Polyhed](vitroid/Polyhed) and [https://github.com/vitroid/countrings](vitroid/countrings) are integrated and improved.

Version {{tool.poetry.version}}

## API

API manual is [here]({{project.urls.manual}}).

## cycles.py

A simple algorithm to enumerate all irreducible cycles of n-members and smaller in an undirected graph. [Matsumoto 2007]

```python
{% include "samples/cycles.py" %}
```

## dicycles.py

An algorithm to enumerate the directed cycles of a size in a dircted graph. [Matsumoto 2021]

```python
{% include "samples/dicycles.py" %}
```

## polyhed.py

An algorithm to enumerate the quasi-polyhedral hull made of cycles in an undirected graph. A quasi-polyhedral hull (vitrite) obeys the following conditions: [Matsumoto 2007]

1. The surface of the hull is made of irreducible cycles.
2. Two or three cycles shares a vertex of the hull.
3. Two cycles shares an edge of the hull.
4. Its Euler index (F-E+V) is two.

```python
{% include "samples/polyhed.py" %}
```

## simplex.py

Enumerate triangle, tetrahedral, and octahedral subgraphs found in the given graph.

## References

1. M. Matsumoto, A. Baba, and I. Ohmine, Topological building blocks of hydrogen bond network in water, J. Chem. Phys. 127, 134504 (2007). http://doi.org/10.1063/1.2772627
2. Matsumoto, M., Yagasaki, T. & Tanaka, H. On the anomalous homogeneity of hydrogen-disordered ice and its origin. J. Chem. Phys. 155, 164502 (2021). https://doi.org/10.1063/5.0065215
