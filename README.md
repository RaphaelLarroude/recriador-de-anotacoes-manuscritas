# Recriador de Anotações Manuscritas

Skill para o ChatGPT recriar anotações manuscritas preservando conteúdo, layout e características individuais da caligrafia a partir de imagens de referência.

## O que faz

A Skill separa conteúdo e estilo visual. O conteúdo vem da imagem original ou do texto fornecido; a caligrafia vem exclusivamente das imagens de referência extraídas de um PDF. O objetivo é reproduzir a escrita da mesma pessoa, incluindo variações e imperfeições humanas, e não aplicar uma fonte manuscrita genérica.

## Quando utilizar

Use quando quiser reconstruir uma ou mais páginas manuscritas com aparência visual semelhante à original e à caligrafia fornecida como referência.

## Arquivos necessários

- **Imagem → Imagem:** uma ou mais imagens das anotações originais e um PDF com exemplos da escrita.
- **Texto → Imagem:** o texto a ser escrito e um PDF com exemplos da escrita.

O PDF é tratado como referência visual de caligrafia, não como simples texto.

## Modos

### Imagem → Imagem

A imagem original define conteúdo e layout. A Skill extrai e analisa as páginas do PDF, cria um perfil estruturado da escrita, transcreve a anotação, mostra a transcrição para revisão e só gera depois da confirmação. Cada imagem original produz uma página separada.

### Texto → Imagem

O texto fornecido define o conteúdo. Depois do PDF, o usuário escolhe o layout: uma ou várias páginas, blocos separados, quebras preservadas ou distribuição automática. A caligrafia e a aparência da folha vêm das referências visuais.

## Fluxo completo

1. Perguntar o modo escolhido.
2. Receber o conteúdo conforme o modo.
3. Receber o PDF de referência.
4. Renderizar páginas úteis do PDF como imagens quando possível.
5. Analisar letras, números, símbolos, espaçamento, inclinação, pressão, textura, papel e instrumento.
6. Preservar variações humanas; nunca criar uma fonte uniforme.
7. No modo Imagem → Imagem, transcrever e usar `[trecho ilegível]` sem inventar.
8. Mostrar a transcrição e pedir alterações.
9. Pedir confirmação antes da geração.
10. Gerar com Nano Banana 2 Pro, usando simultaneamente layout, referências e perfil.
11. Mostrar original e recriada por página.
12. Permitir comparação, regeneração independente e organização da ordem.
13. Exportar um PDF final, se o ambiente permitir.

## Limitações

A geração pode apresentar erros de leitura, símbolos ou posicionamento. Conteúdo ilegível não deve ser adivinhado. O processamento depende das ferramentas disponíveis para ler PDFs, analisar imagens, gerar imagens e criar PDFs. A Skill deve informar falhas claramente e manter versões durante a sessão quando houver armazenamento.

## Privacidade

As imagens devem ser usadas somente para a tarefa. Não solicitar publicação ou compartilhamento desnecessário.

## Instalação

Adicione este repositório ao ambiente de Skills compatível com o ChatGPT e disponibilize o arquivo `SKILL.md` como instrução operacional principal. Consulte a documentação da plataforma correspondente, pois o formato de instalação pode variar.

## Contribuição

Faça um fork, crie uma branch, proponha alterações na documentação ou no fluxo, teste com referências não sensíveis e abra um pull request. Não inclua imagens pessoais de escrita sem autorização.

## Licença

Este projeto é distribuído sob a licença MIT.
