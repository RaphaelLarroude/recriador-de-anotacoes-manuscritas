# Recriador de Anotações Manuscritas

Skill para o ChatGPT recriar anotações manuscritas preservando conteúdo, layout e características individuais da caligrafia.

## Objetivo

O resultado deve parecer escrito pela mesma pessoa das imagens de referência. A Skill não aplica uma fonte manuscrita e não aceita uma escrita apenas genericamente parecida. Ela deve copiar formas concretas das letras, proporções, deformações, inclinação, pressão, textura, espessura, espaçamento e variantes observadas no PDF.

A escrita não deve ficar bonita demais, limpa demais, uniforme demais ou perfeita demais. A referência do usuário tem prioridade sobre qualquer padrão de caligrafia ideal.

## Arquivos necessários

- Imagem → Imagem: uma ou mais imagens originais e um PDF com exemplos da caligrafia.
- Texto → Imagem: o texto e um PDF com exemplos da caligrafia.

O PDF é analisado visualmente como biblioteca de referências, não apenas por OCR.

## Fluxo

1. Escolha do modo.
2. Recebimento do conteúdo.
3. Recebimento do PDF.
4. Extração visual das páginas úteis.
5. Criação do `WritingStyleProfile` com várias ocorrências e variantes das letras.
6. Análise do papel, instrumento, traço e layout.
7. Transcrição no modo Imagem → Imagem.
8. Revisão, alterações e confirmação obrigatória.
9. Geração com Nano Banana 2 Pro quando disponível.
10. Apresentação da imagem original e recriada.
11. Pergunta obrigatória: “O resultado está bom? A escrita está realmente parecida com a letra da pessoa das referências?”
12. Se o usuário reprovar, a Skill registra o motivo, reforça a cópia da caligrafia, reduz uniformidade e regenera somente a página recusada.
13. O ciclo continua até aprovação ou solicitação para parar.
14. Organização, comparação, versões e exportação.

## Avaliação e regeneração

Após cada geração, o usuário pode aprovar ou informar que a letra não parece correta, está perfeita demais, parece uma fonte, precisa de mais irregularidade ou tem problemas no layout. A Skill não deve defender uma geração inadequada nem repetir o mesmo prompt sem mudanças. Cada regeneração precisa incorporar o feedback e preservar as versões anteriores quando possível.

## Limitações

A geração de imagens pode falhar ao reproduzir texto, fórmulas ou pequenas características da caligrafia. O sistema deve informar limitações e nunca inventar conteúdo ilegível. O uso do Nano Banana 2 Pro depende de sua disponibilidade no ambiente.

## Instalação

Adicione o conteúdo de `SKILL.md` às instruções de um GPT personalizado ou ao ambiente de Skills compatível. O GitHub funciona como armazenamento e versionamento do projeto.

## Contribuição

Faça um fork, crie uma branch, teste com dados autorizados e abra um pull request. Não publique amostras pessoais de escrita sem autorização.

## Licença

MIT.
