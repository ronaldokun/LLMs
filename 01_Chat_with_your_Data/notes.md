# Notes from the class

## 05. Question Answering System
 * O propósito de ter uma aplicação RAG é responder perguntas sobre os nossos dados.
 * Criar prompt templates é uma forma de otimizar essa captação de informações de forma reutilizável.
 * Conforme o banco de dados cresce, a quantidade de chunks pode ser muito extensa e é preciso aplicar técnicas para otimizar o processamento desses chunks.
 * `map_reduce` É uma técnica na qual cada parte que é processada por uma chamada de modelo.
 * `refine`: Cada chunk é processado por um modelo e o resultado é refinado, sendo a saída de uma chamada a entrada de uma subsequente.

## Questions

1. Qual aspecto dos carregadores de documento no lanchinho que é mais crucial para lidar com diversas Fontes de dados 
 * A habilidade de comprimir documentos para salvar de forma eficiente
   * Errado: Com o primeiro documento de forma eficiente , é um método para lidar com uma grande quantidade de documentos ou documentos muito grandes , não necessariamente tem conta diversas Fontes de documentos , como TXT , PDF , vídeo , áudio , áudio .
 * o suporte para múltiplos formatos de arquivos e estruturas de dados . 
   * Correto: múltiplos formatos e estrutura de dados garante diversidade de fonte.
 
2. Qual desafio-chave ao quebrar documentos em partes?
    R. com o grande desafio é assegurar que as partes mantenham a integridade semântica. Por exemplo , uma sentença não ser quebrada em 2 partes distintas e perder o seu significado.
3. Qual o papel de embeddings e vector stores ? 
    R. Habilita busca semântica salvamento e resgate de vetores documentais relevantes 
4. Qual é a principal vantagem em utilizar uma Vector Store para recuperar documentos ?
    R. possibilidade de efetuar busca semântica, por exemplo, distância de cossenos. 