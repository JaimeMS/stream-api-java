# Streams JAVA API

![Java](https://github.com/JaimeMS/JaimeMS/blob/main/img/java.JPG)

## Interface Stream

- [Documentação](https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html)
- [Artigo](https://www.oracle.com/br/technical-resources/articles/java-stream-api.html)

#### As Streams possui três partes 
- Construção 
- Desenvolvimento 
- Terminal

#### E são
- Ordenadas
- Não ordenadas

#### E executam funções 
- Linha
- Paralela 

## MAP
###### map(Function<? super T, ? extends R> mapper) 
Para cada elemento de um Array, o Map consegue aplicar uma função e retornar um resultado que pode ser encadeado com outras
funções na stream.

## FILTER
###### filter(Predicate<? super T> predicate)
Para cada elemento de um Array, o Filter vai filtrar os dados através do critério que for passado.

## REDUCE
* ###### reduce(BinaryOperator< T > accumulator)
Realiza uma redução nos elementos da stream, usando uma função de acumulação associativa, 
e retorna um Optional descrevendo o valor reduzido, se houver.

* ###### reduce(T identity, BinaryOperator< T > accumulator)
Reduce recebe um acumulador e um elemento e realiza uma redução nos elementos deste fluxo, usando o valor de identidade fornecido 
e uma função de acumulação associativa, e retorna o valor reduzido.

* ###### reduce(U identity, BiFunction<U, ? super T, U> accumulator, BinaryOperator<U> combiner);
Em sua forma mais geral, uma operação de redução em elementos do tipo < T > gerando um resultado do tipo < U > requer três parâmetros.
O valor de identidade deve ser uma identidade para a função do combinador. Isso significa que para todo u, combiner.apply(identity, u) é igual a u. Além disso, a função do combinador deve ser associativa e compatível com a função do acumulador: para todo u e t, combiner.apply(u, accumulator.apply(identity, t)) deve ser equals() para accumulator.apply(u, t).
