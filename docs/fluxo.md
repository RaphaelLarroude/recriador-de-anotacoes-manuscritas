# Fluxo interno

## Controle de fidelidade

O pipeline deve copiar a caligrafia, não apenas produzir uma escrita manuscrita genérica. O perfil registra várias ocorrências de cada letra e preserva suas diferenças. O modelo não deve escolher uma única forma perfeita e repeti-la.

A avaliação considera formas específicas, proporções, deformações, inclinação, pressão, espessura, textura, espaçamento, alinhamento, conexões, ritmo e imperfeições. Não embelezar nem uniformizar.

## Pipeline

1. Perguntar o modo.
2. Receber imagens originais ou texto.
3. Receber PDF.
4. Renderizar e selecionar páginas visuais úteis.
5. Criar `WritingStyleProfile` com múltiplas variantes.
6. Analisar papel e instrumento.
7. Transcrever no modo Imagem → Imagem, usando `[trecho ilegível]`.
8. Mostrar transcrição, aceitar alterações e aguardar confirmação.
9. Preparar todas as referências simultaneamente.
10. Gerar com Nano Banana 2 Pro quando disponível.
11. Mostrar original e resultado.
12. Perguntar se está bom e se realmente parece com a letra da pessoa.

## Loop de avaliação

Se aprovado, marcar a página como aprovada. Se recusado, não repetir a geração sem mudanças. Perguntar ou interpretar o feedback, por exemplo: “parece fonte”, “está perfeita demais”, “não copiou o formato do meu a”, “o traço está grosso” ou “o espaçamento está errado”.

Depois:

1. Transformar o feedback em instruções concretas.
2. Reforçar as imagens de referência relevantes.
3. Exigir cópia visual das letras e não uma aproximação genérica.
4. Solicitar variação natural e menor perfeição.
5. Regenerar somente a página recusada.
6. Salvar como nova versão.
7. Perguntar novamente se está boa.

Repetir até aprovação ou até o usuário pedir para parar.

## Organização

Processar páginas separadamente, permitir comparação lado a lado, sobreposição, slider e zoom quando possível, manter histórico e exportar um PDF com uma imagem por página, sem distorção ou cortes acidentais.