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
###### <R> Stream<R> map(Function<? super T, ? extends R> mapper) 
Para cada elemento de um Array, o MAP consegue aplicar uma função e retornar um resultado que pode ser encadeado com outras
funções na stream.
