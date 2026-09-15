# Fluxo interno

## Visão geral

A Skill executa um pipeline controlado que separa conteúdo, referências visuais e geração. O layout é tratado independentemente da caligrafia; o PDF é convertido em uma biblioteca de referências visuais.

## Imagem → Imagem

1. Solicitar o modo e aguardar a escolha.
2. Receber todas as imagens originais.
3. Solicitar o PDF de caligrafia.
4. Renderizar páginas do PDF e selecionar exemplos úteis.
5. Analisar letras, símbolos, números, pressão, inclinação, espaçamento, textura e instrumento.
6. Analisar folha, linhas, margens, sombras, manchas e marcas.
7. Consolidar tudo em `WritingStyleProfile`, preservando variantes.
8. Transcrever cada original sem corrigir; usar `[trecho ilegível]` quando necessário.
9. Mostrar a transcrição e aguardar revisão e alterações.
10. Pedir confirmação explícita.
11. Gerar cada página separadamente com Nano Banana 2 Pro, quando disponível.
12. Exibir original e recriação e oferecer ferramentas de comparação.
13. Regenerar apenas a página solicitada, mantendo versões.
14. Organizar a ordem e exportar, se houver suporte.

## Texto → Imagem

1. Solicitar o texto e suas quebras.
2. Solicitar o PDF.
3. Repetir a extração e a análise visual.
4. Criar `WritingStyleProfile` sem converter a escrita em fonte.
5. Perguntar o layout e as características do papel.
6. Mostrar a composição para revisão.
7. Pedir confirmação.
8. Gerar, comparar, regenerar e organizar.

## Controle de fidelidade

A imagem original é a referência do layout. A transcrição revisada controla o conteúdo. O conjunto de páginas do PDF controla a caligrafia. O gerador deve receber as referências simultaneamente e preservar variação humana, sem repetir uma única forma de letra.

## Falhas

Falhas de PDF, OCR ou geração devem ser comunicadas. Nunca transformar uma leitura incerta em conteúdo inventado. Caso uma ferramenta esteja indisponível, informar a etapa que não pôde ser concluída.
