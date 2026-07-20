# Roteiro — Aula 1: Introdução a HTML e Markdown básico
**Duração total: 90 minutos**
**Metodologia:** analisar código pronto → aprender → criar manualmente

**Ferramentas sugeridas:** [W3Schools Tryit](https://www.w3schools.com/html/tryit.asp) ou [CodePen](https://codepen.io) para a parte prática em sala.

**Arquivos de apoio desta aula:**
- `exemplo-completo.html` — página pronta e comentada, usada no Bloco 2 (o aluno abre com **Ctrl+U** para ver o código-fonte)
- `esqueleto.html` — esqueleto vazio, ponto de partida para o Bloco 4

---

## Esqueleto inicial HTML

Todo documento HTML começa com essa estrutura mínima. Vale a pena escrever ela junto com a turma antes de partir para o exemplo completo, já que ela vai se repetir em toda página que criarem daqui em diante:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Site</title>
</head>
<body>

</body>
</html>
```

Vale explicar rapidamente cada linha (sem se aprofundar ainda, só nomear):
- `<!DOCTYPE html>` — avisa o navegador que é um documento HTML5
- `<html lang="pt-BR">` — a "caixa" que envolve tudo; `lang` ajuda acessibilidade e SEO
- `<head>` — informações que não aparecem na página (aba do navegador, configurações)
- `<meta charset="UTF-8">` — garante acentuação correta
- `<meta name="viewport"...>` — comportamento responsivo em celulares
- `<title>` — texto que aparece na aba do navegador
- `<body>` — onde entra tudo que o visitante vê

**Sobre o Markdown:** diferente do HTML, o Markdown não tem um "esqueleto" obrigatório — não existe declaração de documento, `head` ou `body`. Um arquivo `.md` pode começar direto com o conteúdo (ex: `# Título`). Isso é, inclusive, um bom contraste pedagógico a explorar no Bloco 3: HTML precisa de estrutura declarada, Markdown não.

---

## Bloco 1 — Abertura e contexto (0–10 min)

- Pergunta disparadora: "O que vocês acham que faz uma página da internet existir?"
- Explicar em 2–3 frases: HTML é a **estrutura** (o esqueleto) de toda página web. CSS cuida da aparência, JS do comportamento — mas isso vem depois.
- Deixar claro o percurso do curso: hoje só HTML puro, sem estilização nenhuma (páginas vão ficar "feias" de propósito — isso é normal e esperado).

**Objetivo do bloco:** engajar e situar o aluno no que vem pela frente, sem entrar em teoria pesada ainda.

---

## Bloco 2 — Analisar código pronto (10–35 min)

1. Abrir `exemplo-completo.html` diretamente no navegador — mostrar o preview funcionando primeiro, deixar a curiosidade "como isso virou isso?" aparecer.
2. Pedir para os alunos apertarem **Ctrl+U** (ver código-fonte da página) — esse é o momento de "abrir o capô" e mostrar que toda página da internet pode ser inspecionada assim.
3. Ler o código junto com a turma, linha por linha, usando os comentários (`<!-- -->`) já presentes no arquivo como guia, perguntando antes de explicar:
   - "O que vocês acham que essa tag faz?"
   - "Por que será que tem uma tag de abertura e uma de fechamento?"
4. Apresentar o vocabulário essencial à medida que aparece no código (não antes):
   - `<html>`, `<head>`, `<title>`, `<body>`
   - `<h1>` a `<h6>` (hierarquia de títulos)
   - `<p>` (parágrafo)
   - `<a href="">` (link)
   - `<img src="" alt="">` (imagem)
   - `<ul>`, `<ol>`, `<li>` (listas)
   - Conceito de **tag de abertura/fechamento** e **atributo**

**Objetivo do bloco:** o aluno sai daqui reconhecendo as tags mais comuns e entendendo a lógica de aninhamento, sem ainda ter decorado nada — só ter visto funcionando.

---

## Bloco 3 — Markdown básico, por contraste (35–50 min)

Aproveitar que o HTML acabou de ser visto para mostrar o mesmo conteúdo em Markdown, como um "atalho" mais simples.

- Mostrar lado a lado: o mesmo título, parágrafo, lista e link escritos em HTML e em Markdown.
- Sintaxe essencial:
  - `# Título` → `<h1>`
  - `**negrito**` e `*itálico*`
  - `- item` → lista
  - `[texto](url)` → link
  - `![alt](url)` → imagem
- Deixar claro **quando usar cada um**: Markdown é ótimo para documentação, README, anotações; HTML é a base real da web e permite muito mais controle.

**Objetivo do bloco:** o aluno entende que Markdown "vira" HTML por baixo dos panos — isso reforça a lógica do HTML em vez de confundir.

---

## Bloco 4 — Mão na massa: criar uma página HTML do zero (50–80 min)

Proposta de exercício guiado (ajuste o tema à turma — ex: "página sobre você" ou "página sobre um hobby"):

1. Cada aluno parte do arquivo `esqueleto.html` (o mesmo esqueleto visto no início da aula, já com `<head>`, `<meta>` e `<title>` prontos).
2. Um `<h1>` com o título da página.
3. Pelo menos dois `<p>` de texto.
4. Uma `<ul>` ou `<ol>` com no mínimo 3 itens.
5. Um `<a href="">` para algum site.
6. Uma `<img src="" alt="">` (pode usar uma URL de imagem qualquer da internet).

Dinâmica sugerida:
- Primeiros 5 min: abrir o `esqueleto.html` todos juntos, relembrando rapidamente cada linha (fixar a estrutura antes de preencher o `<body>`).
- Depois: cada aluno segue no próprio ritmo adicionando os elementos dentro do `<body>`, com você circulando para tirar dúvidas.
- Reservar os últimos 10 minutos do bloco para quem terminar rápido explorar tags extras (`<br>`, `<hr>`, `<strong>`, `<em>`) e ajudar quem está com dificuldade.

**Objetivo do bloco:** prática autônoma é o coração da aula — é aqui que a memória muscular do HTML começa a se formar.

---

## Bloco 5 — Compartilhamento e fechamento (80–90 min)

- 2 a 3 alunos (voluntários) compartilham a tela e mostram a página que criaram.
- Rápida checagem coletiva: "alguém esqueceu de fechar uma tag? o que aconteceu na página quando isso rolou?" (ótimo gancho para explicar por que a sintaxe importa).
- Fechamento: recapitular em uma frase o que foi visto — "hoje vocês estruturaram uma página inteira só com HTML puro."
- Gancho para a próxima aula: "na próxima aula, essa mesma página vai ganhar cor, espaçamento e estilo com CSS."

**Tarefa opcional para casa:** adicionar mais um elemento à página (uma tabela simples ou mais uma imagem) e testar o que acontece quebrando a sintaxe de propósito (por curiosidade).

---

## Checklist de tags cobertas na Aula 1

`<html>` `<head>` `<title>` `<body>` `<h1>`–`<h6>` `<p>` `<a>` `<img>` `<ul>` `<ol>` `<li>` `<br>` `<hr>` `<strong>` `<em>`

## Sintaxe Markdown coberta

`#` títulos · `**negrito**` · `*itálico*` · `- lista` · `[link](url)` · `![imagem](url)`
