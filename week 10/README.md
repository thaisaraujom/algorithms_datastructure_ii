# Analysis about the flights network in Brazil

This work aims to perform an analysis on the Brazilian flight network and was done by [Mariana Azevedo](https://github.com/marianabritoazevedo/data-structure-ii/tree/main/flights-brazil) and [Thaís Medeiros](https://github.com/thaisaraujo2000/algorithms_datastructure_ii/tree/main/week%2010). For this, the dataset present in the [Álvaro's Repository](https://github.com/alvarofpp/dataset-flights-brazil) was used.

## Assortativity

In a network, it is possible to analyze the propriety called _assortativy_.  From this, you can determine whether the network is assortativity or not, that is, analyze how connected the nodes are to each other. There are two ways to perform this analysis: by attribute (categorical or numerical) or by degree, which can be seen in the following example.

<p align="center" style="text-align:center">
    <img width='700' src='./img/assortativity_att_dg.png'>
</p align="center">

According to the figure below, you can see that the brazilian flight network can be assortativity, since the extremities are quite dark, indicating that elements of the same group tend to connect more. However, it is also possible to observe that there are many connections between elements from different groups.

<p align="center" style="text-align:center">
    <img width='500' src='./img/assortativity.png'>
</p align="center">

With this, the assortativity coefficient based on a give node atribute was calculated, obtaining a value of approximately `0.37`, which indicates that the network assortativity, since it is positive. In addition, the generated matrix, with its values assigned to the table below, this property of assortativity is strengthened.

 Region           |    1    |     2      |      3     |      4     | 5 
 :--------:| :--------: | :------:   | :--------: | :--------: | :--------:
1| **0.07358156** | 0.01340869 | 0.04022606 | 0.0120789  | 0.0070922
2| 0.01340869 | **0.0802305**  | 0.05474291 | 0.0106383  | 0.01983599
3| 0.04022606 | 0.05474291 | **0.17309397** | 0.03390957 | 0.02759309
4| 0.0120789  | 0.0106383  | 0.03390957 | **0.13453014** | 0.02293883
5| 0.0070922  | 0.01983599 | 0.02759309 | 0.02293883 | **0.05363475**

## Connected components

The network is not connected and has 6 connected components. For each of them, an analysis was performed considering all five regions of Brazil in quantity and percentage. 

Thus, for each connected component, the values obtained can be visualized in the figure below.

<p align="center" style="text-align:center">
    <img width='100%' src='./img/regions.png'>
</p align="center">

## References
- [Álvaro's Repository](https://github.com/alvarofpp/dataset-flights-brazil)
- [Ivanovitch's Repository](https://github.com/ivanovitchm/datastructure)