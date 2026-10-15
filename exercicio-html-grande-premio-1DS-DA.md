# Exercício de HTML para o 1ºDS DA: a página do Grande Prémio da Escola

Ficheiro temporário, de 2026-10-15. Não está registado em lado nenhum. Tem duas partes: o enunciado do exercício e, no fim, uma cábula com as etiquetas de HTML de que o exercício precisa, e mais algumas.

---

# Exercício: a página do Grande Prémio

A Associação de Estudantes vai organizar um torneio de um jogo de corridas de karts na Semana da Escola e pediu-te a página inicial do site do torneio. Mandou-te o texto num email, sem HTML nenhum, pela ordem em que o quer ver. O teu trabalho é decidir o que é cada parte desse texto (um título, um parágrafo, uma lista, uma tabela, uma imagem, uma zona da página) e escrever a página.

Não há matéria nova: tudo o que precisas está no guia de HTML e semântica. A diferença em relação à ficha é que aqui ninguém te diz que elemento usar. Tens de o descobrir a partir do conteúdo.

## O email da associação

```text
Olá! Segue o texto da página inicial, pela ordem em que o queremos ver.

No topo de todas as páginas: o nosso logótipo (um capacete com uma bandeira
aos quadrados, com 48 por 48 píxeis), logo ao lado o nome "Grande Prémio da
Escola", e o menu com Início e Regulamento.

Torneio de karts na Semana da Escola

Vem descobrir quem é a dupla mais rápida da escola! O torneio é de um jogo de
corridas de karts, joga-se em duplas e a participação é gratuita. As inscrições
fecham a 20 de novembro, e depois dessa data não se aceitam inscrições.

Como te inscreves
Junta-te a um colega: cada dupla tem dois jogadores.
Escolhe um nome para a dupla.
Vai à sala da associação, no piso 0, e preenche a folha de inscrição.
Guarda o papel com o número da dupla, porque vais precisar dele no dia da corrida.

Regras principais
Cada corrida tem quatro duplas.
Os comandos são da escola, e não podes trazer o teu.
Cada jogador corre duas pistas, e conta a soma dos tempos da dupla.
O regulamento completo está noutra página: para o leres, clica aqui.

Calendário
As eliminatórias são na segunda-feira, 23 de novembro, às 14:00, no pavilhão B.
As meias-finais são na quarta-feira, 25 de novembro, às 14:00, também no
pavilhão B. A final é na sexta-feira, 27 de novembro, às 15:30, no auditório.

O prémio
(O desenho do troféu: uma taça dourada com um pequeno kart vermelho em cima e
uma fita azul atada à base. Mede 400 por 300 píxeis.)
Legenda: O troféu deste ano, oferecido pela associação de pais.

Uma dica, para quem quiser: treina em casa com um comando, porque no dia do
torneio não há tempo para treinos.

No fundo de todas as páginas: Organização da Associação de Estudantes.
Ano letivo 2026/2027.
```

## A pasta do site

```text
grande-premio/
├── index.html
├── regulamento.html
└── imagens/
    ├── logotipo.svg
    └── trofeu.svg
```

## Parte 1: Planear antes de escrever

Responde no caderno, antes de abrires o editor.

**a)** Escreve o índice dos títulos da página, com o nível de cada um, de `h1` a `h6`, e com a indentação a mostrar os níveis.

**b)** Divide a página em zonas, de cima para baixo, e diz que elemento usas em cada uma: `header`, `nav`, `main`, `section`, `article`, `aside` ou `footer`. Justifica a zona da dica com o teste do guia.

**c)** O email tem duas listas. Diz qual leva `ol` e qual leva `ul`, e justifica com o teste da troca de itens. Uma das linhas que a associação pôs numa das listas não é um item como os outros: qual é, e onde a pões?

**d)** A associação escreveu o calendário num parágrafo. Explica porque é que estes dados ficam melhor numa tabela e desenha-a à mão: o que fica nas linhas, o que fica nas colunas e que células são cabeçalhos.

## Parte 2: Escrever as duas páginas

**1.** Escreve o `index.html` com tudo o que decidiste na parte 1. Começa pelo esqueleto completo, com a língua certa e um `title` que diga o nome da página e o do site, como nas páginas do Clube de Robótica.

**2.** No primeiro parágrafo há uma frase que nenhum participante pode deixar escapar. Marca-a com o elemento certo.

**3.** Escreve o `regulamento.html` só com o esqueleto, o mesmo `header` e o mesmo `footer` do `index.html` e, no `main`, o título "Regulamento do torneio" e o parágrafo "Página em construção.". Esta página serve para experimentares as ligações. O regulamento verdadeiro fica para outro dia.

## Parte 3: Verificar

**a)** Abre o `index.html` no browser e lê a página de cima a baixo. Aparece tudo pela ordem do email? As duas imagens aparecem?

**b)** Sem tocar no rato, percorre a página com a tecla Tab. Escreve o texto de cada sítio onde o foco para. Cada um diz sozinho para onde leva? Se algum não disser, corrige-o.

**c)** Segue a ligação para o regulamento e volta à página inicial pelo menu.

## Desafio opcional

A associação quer arrumar numa pasta própria as páginas que não são a inicial. Cria a pasta `informacoes`, muda para lá o `regulamento.html` e corrige, nas duas páginas, todos os caminhos que deixaram de funcionar. Antes de mexeres, escreve a lista dos caminhos que vão mudar. Depois confirma-a no browser.

---

# Cábula de HTML: as etiquetas do exercício e mais algumas

Um **elemento** de HTML é formado por uma etiqueta de abertura, um conteúdo e uma etiqueta de fecho: `<p>Olá</p>`. Os **atributos** escrevem-se dentro da etiqueta de abertura, sempre na forma `nome="valor"`, e acrescentam informação ao elemento: `<a href="regras.html">`. Alguns elementos são **vazios**: não têm conteúdo nem etiqueta de fecho, porque tudo o que precisam está nos atributos. É o caso do `img`, do `meta` e do `br`.

Os elementos encaixam-se uns nos outros, e fecha-se sempre primeiro o que se abriu por último: `<p><strong>Atenção</strong></p>`, e nunca `<p><strong>Atenção</p></strong>`.

Escolhe cada elemento pelo que o conteúdo **é**, e nunca pelo aspeto que tem no browser. O aspeto é trabalho do CSS.

## 1. O esqueleto de todas as páginas

```html
<!doctype html>
<html lang="pt-PT">
    <head>
        <meta charset="utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <title>Início | Clube de Xadrez</title>
    </head>
    <body>
        <!-- Aqui vai tudo o que se vê na página. -->
    </body>
</html>
```

| Etiqueta                     | Para que serve                                                                                                                                                |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<!doctype html>`            | Diz ao browser que a página está escrita em HTML atual. É sempre a primeira linha                                                                             |
| `<html lang="pt-PT">`        | Contém a página inteira. O `lang` diz a língua: o leitor de ecrã pronuncia o texto em português de Portugal, e o tradutor do browser sabe de que língua parte |
| `<head>`                     | A informação sobre a página, que não aparece no meio dela                                                                                                     |
| `<meta charset="utf-8">`     | Diz ao browser como ler os caracteres. Sem ele, os acentos e o "ç" podem aparecer trocados                                                                    |
| `<meta name="viewport" ...>` | Faz a página ocupar a largura do ecrã do telemóvel, em vez de aparecer encolhida                                                                              |
| `<title>`                    | O nome que aparece no separador do browser, nos favoritos e nos resultados das pesquisas. Diz o nome da página e o do site: "Início \| Clube de Xadrez"       |
| `<body>`                     | Tudo o que se vê na página                                                                                                                                    |

## 2. Títulos e texto

| Etiqueta        | Para que serve                                                                                                                                                 | Quando não se usa                                                                                                               |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `<h1>` a `<h6>` | Os títulos, do mais importante (`h1`) ao menos importante (`h6`). Juntos, formam o índice da página. Há um só `h1` por página, com o assunto da página inteira | Nunca se escolhe um título pelo tamanho da letra, e não se saltam níveis a descer: depois de um `h2` vem um `h3`, e não um `h4` |
| `<p>`           | Um parágrafo: um bloco de texto corrido, com uma ideia                                                                                                         | Uma lista não fica dentro de um parágrafo. Fecha o `p` antes do `ul` ou do `ol`                                                 |
| `<strong>`      | Texto de importância forte, que o leitor não pode deixar escapar, como um prazo ou um aviso. Aparece a negrito                                                 | Não serve para pôr texto a negrito só por enfeite                                                                               |
| `<em>`          | Ênfase: a palavra onde se põe a força quando se diz a frase em voz alta, e que às vezes muda o sentido da frase. Aparece em itálico                            | Não serve para pôr texto em itálico só por enfeite                                                                              |
| `<br>`          | Muda de linha dentro do mesmo parágrafo, quando a mudança de linha faz parte do conteúdo, como nas linhas de uma morada. É vazio                               | Nunca se usa para afastar blocos de texto, nem se empilham vários `br` para fazer espaço                                        |

```html
<h1>Clube de Xadrez</h1>
<p>
    Treinamos à quarta-feira.
    <strong>Traz o teu tabuleiro, porque a escola só tem quatro.</strong>
</p>
<p>Não disse que a partida era difícil. Disse que era <em>longa</em>.</p>
<p>
    Sala 12, piso 1<br />
    Escola Profissional
</p>
```

## 3. Listas

| Etiqueta | Para que serve                                                                  |
| -------- | ------------------------------------------------------------------------------- |
| `<ul>`   | Lista não ordenada: a ordem dos itens não muda a informação. Aparece com pontos |
| `<ol>`   | Lista ordenada: a ordem dos itens faz parte da informação. Aparece com números  |
| `<li>`   | Um item de uma lista. Fica sempre dentro de um `ul` ou de um `ol`               |

Para escolher, faz o **teste da troca**: imagina que trocas o primeiro item com o último. Se a informação fica errada, a lista é ordenada (`ol`). Se só fica diferente, é não ordenada (`ul`). E cada item tem de ser do mesmo género dos outros: se uma linha não é um item como os restantes, não pertence à lista.

```html
<ol>
    <li>Abre o tabuleiro.</li>
    <li>Coloca as peças.</li>
    <li>As brancas jogam primeiro.</li>
</ol>
```

## 4. Ligações e imagens

| Etiqueta ou atributo | Para que serve                                                                                                                                                                                                                                                                                                  |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<a href="...">`     | Uma ligação. O `href` diz para onde leva: um caminho relativo para uma página tua (`regras.html`) ou um endereço completo para outro site (`https://...`). O texto da ligação diz, sozinho, para onde ela leva. "Clica aqui" não diz nada a quem percorre a página com a tecla Tab ou a ouve num leitor de ecrã |
| `<img>`              | Uma imagem. É vazio                                                                                                                                                                                                                                                                                             |
| `src`                | O caminho do ficheiro da imagem, por exemplo `imagens/tabuleiro.svg`                                                                                                                                                                                                                                            |
| `alt`                | O texto alternativo: o que dirias da imagem se estivesses a descrever a página ao telefone. Toda a imagem tem `alt`. Fica vazio, `alt=""`, quando a imagem é decorativa ou quando o texto ao lado já diz tudo. Não começa por "Imagem de"                                                                       |
| `width` e `height`   | A largura e a altura em píxeis, sem unidade. O browser reserva logo o espaço, e a página não salta quando a imagem acaba de carregar                                                                                                                                                                            |
| `<figure>`           | Junta uma imagem e a sua legenda numa unidade                                                                                                                                                                                                                                                                   |
| `<figcaption>`       | A legenda, dentro do `figure`. Acrescenta o que toda a gente deve saber, e o `alt` não a repete                                                                                                                                                                                                                 |

Os **caminhos relativos** partem da pasta onde está a página que tem a ligação. Para descer a uma pasta, escreve o nome dela e uma barra: `imagens/peao.svg`. Para subir à pasta de cima, escreve `../`: `../index.html`.

```html
<p>
    Lê as <a href="regras.html">regras do torneio de xadrez</a> antes da
    primeira partida.
</p>

<figure>
    <img
        src="imagens/tabuleiro.svg"
        alt="Tabuleiro de xadrez a meio de uma partida, com o rei branco cercado por três peças pretas."
        width="400"
        height="300"
    />
    <figcaption>A partida decisiva do torneio do ano passado.</figcaption>
</figure>
```

## 5. As zonas da página

| Etiqueta    | Para que serve                                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<header>`  | O cabeçalho: a zona de introdução do topo, com o nome do site, o logótipo e o menu. Repete-se em todas as páginas                                                                     |
| `<nav>`     | O bloco de ligações que leva às partes principais do site, como o menu. Não é para qualquer grupo de ligações                                                                         |
| `<main>`    | O conteúdo principal: o que é próprio desta página e não se repete nas outras. Há um só por página, e não fica dentro do `header`, do `footer`, do `nav`, do `article` nem do `aside` |
| `<section>` | Uma parte do conteúdo com um título próprio. Se não lhe consegues dar um título, provavelmente não é uma secção                                                                       |
| `<article>` | Um conteúdo completo, que faria sentido sozinho se o copiasses para outro site, como uma notícia                                                                                      |
| `<aside>`   | Um conteúdo secundário, que se pode saltar sem perder nada essencial, como uma dica ou uma caixa de "sabias que"                                                                      |
| `<footer>`  | O rodapé: a zona de informação final, com a autoria, os contactos e os avisos. Repete-se em todas as páginas                                                                          |
| `<div>`     | Uma caixa genérica, sem significado nenhum. É o último recurso, para quando nenhum dos outros serve. Vais usá-lo no CSS                                                               |

Quando estiveres indeciso, faz estas perguntas por ordem e para na primeira a que respondes que sim:

1. É o conteúdo principal desta página? É o `main`.
2. É o menu do site? É um `nav`.
3. É a zona do topo ou a do fundo? É o `header` ou o `footer`.
4. Pode saltar-se sem perder nada? É um `aside`.
5. Faria sentido sozinho noutro site? É um `article`.
6. Consegues dar-lhe um título? É uma `section`.
7. Nenhuma das anteriores? Talvez um `div`, ou talvez não precise de caixa nenhuma.

## 6. Tabelas

Uma tabela é só para **dados** que se leem em linhas e colunas, em que cada valor responde a uma pergunta que junta uma linha e uma coluna. Nunca se usa uma tabela para arrumar a página.

| Etiqueta ou atributo | Para que serve                                                         |
| -------------------- | ---------------------------------------------------------------------- |
| `<table>`            | Contém a tabela inteira                                                |
| `<caption>`          | O nome da tabela. Fica logo a seguir à etiqueta de abertura do `table` |
| `<thead>`            | A parte de cima, com a linha dos cabeçalhos das colunas                |
| `<tbody>`            | O corpo, com as linhas de dados                                        |
| `<tr>`               | Uma linha da tabela (de _table row_)                                   |
| `<th>`               | Uma célula de cabeçalho. Aparece a negrito e centrada                  |
| `scope="col"`        | Diz que o `th` é o cabeçalho da sua coluna                             |
| `scope="row"`        | Diz que o `th` é o cabeçalho da sua linha                              |
| `<td>`               | Uma célula de dados (de _table data_)                                  |

Os cabeçalhos com `scope` permitem ao leitor de ecrã anunciar, em cada célula, de que linha e de que coluna ela é: "Sandes mista, Professor, 1,50 euros".

```html
<table>
    <caption>
        Preços do bar da escola (inventados)
    </caption>
    <thead>
        <tr>
            <th scope="col">Produto</th>
            <th scope="col">Aluno</th>
            <th scope="col">Professor</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">Sandes mista</th>
            <td>1,20 €</td>
            <td>1,50 €</td>
        </tr>
        <tr>
            <th scope="row">Sumo natural</th>
            <td>0,80 €</td>
            <td>1,00 €</td>
        </tr>
    </tbody>
</table>
```

## 7. Comentários

```html
<!-- Isto é um comentário: o browser ignora-o e não o mostra na página. -->
```

Os comentários são notas para quem lê o código. Cuidado: qualquer pessoa os vê, se abrir o código da página no browser, por isso nunca escrevas lá nada que não possas mostrar.

## 8. Mais algumas, que o guia não deu

Estas três etiquetas são matéria nova: não estão no guia de HTML e semântica, e não precisas delas no exercício. Ficam aqui para quando o teu conteúdo as pedir.

| Etiqueta                | Para que serve                                                                                                                                                                                                                                                                                                  | Quando não se usa                                                                                                                                                                       |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<time datetime="...">` | Uma data ou uma hora. O texto entre as etiquetas é para as pessoas, e o atributo `datetime` repete a mesma data numa forma que os programas percebem: ano, mês e dia (`2026-12-04`), e, se houver hora, um `T` e a hora (`2026-12-04T14:00`). Assim, um calendário ou um motor de pesquisa conseguem ler a data | Não serve para datas vagas, como "no fim do período", que não têm um dia certo                                                                                                          |
| `<abbr title="...">`    | Uma abreviatura ou uma sigla. O `title` tem a forma por extenso, que aparece quando se passa o rato por cima                                                                                                                                                                                                    | O `title` não aparece no telemóvel nem para quem usa só o teclado. Por isso, escreve a forma por extenso no texto da primeira vez que a sigla aparece, e usa o `abbr` daí para a frente |
| `<blockquote>`          | Uma citação mais longa, tirada de outra fonte: uma frase de um regulamento, de um livro ou de uma entrevista. O browser mostra-a afastada da margem                                                                                                                                                             | Nunca se usa só para afastar texto da margem. Isso é trabalho do CSS                                                                                                                    |

```html
<p>O teste é a <time datetime="2026-12-04">4 de dezembro</time>.</p>
<p>A <abbr title="Associação de Estudantes">AE</abbr> organiza o torneio.</p>
<blockquote>
    <p>Cada jogador tem dez minutos para a partida inteira.</p>
</blockquote>
```
