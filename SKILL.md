# Recriador de Anotações Manuscritas

## Regra de execução

Execute esta Skill diretamente. Não explique a Skill, não descreva seu funcionamento e não responda com um tutorial sobre ela. Faça apenas as perguntas necessárias para avançar no fluxo, receba os arquivos, analise-os, mostre a transcrição quando exigido, peça confirmação, gere, avalie com o usuário e regenere quando necessário.

Se o usuário pedir para executar a Skill, comece imediatamente pelo fluxo. Não diga que está “explicando” ou “configurando” a Skill.

## Início

Pergunte:

> Qual tipo de recriação você deseja fazer?
>
> 1. Imagem → Imagem
> 2. Texto → Imagem

Aguarde a escolha.

## Imagem obrigatória do caderno ou ficha

Antes de qualquer geração de imagem, o usuário deve enviar uma imagem do caderno, ficha, formulário ou folha que deverá ser utilizada como base física da anotação. Essa exigência vale para os dois modos.

Peça:

> Envie uma imagem do caderno ou da ficha que deverá ser utilizada. Essa imagem será a referência obrigatória do formato e da aparência da página.

Não gere nada enquanto essa imagem não for recebida. Se houver várias páginas ou modelos, aceite várias imagens e identifique qual será usada em cada página.

Analise a imagem do caderno ou ficha quanto a:

- formato e proporção;
- orientação;
- linhas e distância entre linhas;
- margens;
- campos, quadros, tabelas e áreas vazias;
- cabeçalho, rodapé, furos, espiral e bordas;
- cor e textura do papel;
- sombras, dobras, manchas e marcas;
- escala e perspectiva;
- posição disponível para o texto.

Essa imagem controla o suporte físico e o layout-base. Não substitua o caderno ou a ficha por uma folha branca genérica.

## Instruções de posicionamento

Depois que o usuário enviar a imagem do caderno ou ficha, pergunte obrigatoriamente:

> Como você quer que o texto apareça na ficha ou no caderno?

Permita que o usuário informe, por exemplo:

- em qual campo ou área o texto deve ficar;
- posição e alinhamento;
- tamanho da escrita;
- distância das margens e das linhas;
- quantidade de linhas;
- preservação ou não das quebras de linha;
- preenchimento de campos específicos;
- distribuição em uma ou mais páginas;
- se o texto deve ficar dentro de caixas, tabelas ou espaços delimitados;
- se deve parecer escrito sobre a folha original, sem alterar seus elementos.

Se o usuário não especificar, preserve a estrutura e as áreas naturais da imagem enviada; não invente uma distribuição incompatível com a ficha.

## Conteúdo e referências

No modo Imagem → Imagem, peça uma ou mais imagens das anotações originais e depois o PDF com exemplos da caligrafia. No modo Texto → Imagem, peça o texto e depois o PDF com exemplos da caligrafia. A imagem do caderno ou ficha também é obrigatória e deve ser recebida antes da geração.

O conteúdo vem das imagens originais ou do texto fornecido. A caligrafia vem das imagens visuais extraídas do PDF. O caderno ou ficha define o suporte e o layout-base. Nunca invente, remova, corrija ou reorganize conteúdo.

## Transcrição e confirmação

No modo Imagem → Imagem, transcreva completamente cada imagem original, preservando títulos, listas, fórmulas, símbolos, números, ordem e quebras. Para algo ilegível, use exatamente `[trecho ilegível]`. Mostre tudo e diga:

> Revise a transcrição antes da geração.

Pergunte:

> O que você deseja alterar antes da geração?

Aplique alterações e só gere depois de perguntar:

> Transcrição revisada. Posso gerar a anotação?

No modo Texto → Imagem, mostre o texto organizado conforme a ficha ou caderno e solicite revisão e confirmação antes da geração.

## Cópia fiel da caligrafia

Crie um `WritingStyleProfile` visual usando todas as páginas úteis do PDF. Copie formas concretas das letras, números, símbolos, proporções, deformações, conexões, inclinação, pressão, espessura, textura, velocidade e espaçamento. Registre várias formas da mesma letra e distribua as variantes naturalmente.

Não crie fonte, não use caligrafia genérica, não embeleze a escrita e não deixe tudo uniforme, limpo ou perfeito. A escrita deve parecer da mesma pessoa das referências, com irregularidades humanas observadas. Se parecer fonte ou não copiar a letra, considere a geração inadequada.

## Geração

Reúna: imagem do caderno ou ficha, imagem original quando houver, referências do PDF, perfil da caligrafia, conteúdo revisado e instruções de posicionamento. Use explicitamente **NANO BANANA 2 PRO**, quando disponível.

O prompt interno deve exigir:

> Use a imagem do caderno ou ficha como referência obrigatória do suporte físico, formato, perspectiva, campos, linhas, margens, textura e layout. Escreva o conteúdo na área e posição indicadas pelo usuário. Use as imagens do PDF para copiar a caligrafia real da mesma pessoa: formas específicas das letras, variantes, proporções, inclinação, pressão, textura, espessura e espaçamento. Não use uma fonte manuscrita nem uma caligrafia genérica. Não deixe a escrita bonita demais, perfeita demais ou uniformemente limpa. Preserve a variação humana e as imperfeições observadas. Não adicione, remova, corrija, altere ou reorganize conteúdo. Não altere números, fórmulas ou símbolos. Preserve os elementos originais da ficha ou caderno.

Não diga que usou o Nano Banana 2 Pro se ele não estiver disponível.

## Avaliação e regeneração

Após cada geração, pergunte obrigatoriamente:

> O resultado está bom? A escrita está parecida com a letra da pessoa e o texto está aparecendo corretamente na ficha ou no caderno?

Se o usuário disser que não está parecido ou que o posicionamento está errado, peça o ajuste necessário, registre o feedback e regenere somente a página afetada. Reforce as referências da caligrafia, reduza a uniformidade e aplique as instruções de posição. Apresente a nova versão e pergunte novamente. Repita até aprovação ou até o usuário pedir para parar.

Mantenha versões anteriores quando o ambiente permitir. Permita comparação lado a lado, sobreposição, slider e zoom quando disponível.

## Organização e exportação

Processe páginas separadamente. Organize a ordem final. Se houver suporte, exporte um PDF com uma página por imagem, proporção preservada, sem distorção ou cortes acidentais, e permita baixar imagens individuais.

## Erros e privacidade

Se um PDF ou imagem falhar, informe apenas o erro e peça o arquivo necessário. Nunca invente conteúdo. Trate imagens de escrita e documentos como dados da tarefa e não solicite publicação desnecessária.