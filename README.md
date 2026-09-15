# Recriador de Anotações Manuscritas

Skill que recria anotações usando a caligrafia real das referências e a imagem do caderno ou ficha como base obrigatória.

## Execução direta

A Skill deve ser executada, não explicada. Ao ser usada, ela faz as perguntas necessárias, recebe os arquivos, analisa a caligrafia, revisa o conteúdo, gera a imagem, pergunta se o resultado está bom e refaz quando necessário.

## Imagem do caderno ou ficha

Antes de qualquer geração, o usuário deve enviar uma imagem do caderno, ficha, formulário ou folha que será utilizada. Essa imagem define formato, perspectiva, linhas, margens, campos, tabelas, áreas de escrita, textura e aparência física. Uma folha branca genérica não deve ser usada no lugar dela.

Depois de receber a imagem, a Skill pergunta:

> Como você quer que o texto apareça na ficha ou no caderno?

O usuário pode informar campo, posição, alinhamento, tamanho, linhas, margens, quebras, caixas e distribuição.

## Modos

### Imagem → Imagem

Recebe imagens originais, a imagem do caderno ou ficha e um PDF com exemplos da caligrafia. Transcreve o original, mostra para revisão e só gera após confirmação.

### Texto → Imagem

Recebe texto, a imagem do caderno ou ficha e um PDF com exemplos da caligrafia. Organiza o texto conforme as instruções do usuário e revisa antes de gerar.

## Fidelidade

A imagem do PDF é usada para copiar as formas reais das letras. A Skill deve preservar variantes, imperfeições, pressão, inclinação, textura, espessura e espaçamento. Não deve criar uma fonte, uniformizar a escrita ou deixá-la perfeita demais.

## Pós-geração

Depois de cada imagem, pergunta se a escrita parece com a pessoa e se o texto está correto na ficha ou caderno. Se não estiver, registra o problema, aplica novas instruções e regenera somente a página afetada até aprovação.

## Limitações

O Nano Banana 2 Pro será usado quando estiver disponível. Leitura de texto, fórmulas e reprodução exata da caligrafia podem falhar; conteúdo ilegível nunca deve ser inventado.

## GitHub

O repositório armazena e versiona a Skill. Para usar em um GPT personalizado, coloque o conteúdo de `SKILL.md` nas instruções do GPT.