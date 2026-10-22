# Exercício de HTML para o 1ºDS DA: a página da Sala de Fuga

Ficheiro temporário, de 2026-10-22. Não está registado em lado nenhum. Tem duas partes: o enunciado do exercício e, no fim, uma cábula curta com as etiquetas que este exercício pede e que a cábula do Grande Prémio não tinha.

---

# Exercício: a página da Sala de Fuga

O Clube de Teatro transformou duas salas da escola em salas de fuga e pediu-te a página inicial do site. Numa sala de fuga, a tua equipa fica fechada numa sala e tem 30 minutos para resolver os enigmas e descobrir o código que abre a porta. O clube mandou-te o texto num email, sem HTML nenhum, pela ordem em que o quer ver. O teu trabalho é decidir o que é cada parte desse texto e escrever a página.

Não há matéria nova: tudo o que precisas está no guia de HTML e semântica. Tal como no Grande Prémio, ninguém te diz que elemento usar. Tens de o descobrir a partir do conteúdo.

## O email do Clube de Teatro

```text
Olá! Segue o texto da página inicial, pela ordem em que o queremos ver.

No topo de todas as páginas: o nosso logótipo (um cadeado roxo com um ponto
de interrogação, com 48 por 48 píxeis), logo ao lado o nome "Sala de Fuga da
Escola", e o menu com Início e Perguntas frequentes.

Salas de fuga na escola, de 9 a 11 de dezembro

O Clube de Teatro transformou duas salas da escola em salas de fuga. Entras
com a tua equipa, a porta fecha-se, e têm 30 minutos para encontrar as pistas,
resolver os enigmas e descobrir o código que abre o cadeado. É de graça e é
para alunos de todos os anos. NENHUMA EQUIPA ENTRA SEM MARCAÇÃO FEITA NA
BIBLIOTECA.

Não ganha a equipa que sabe mais. Ganha a que OUVE mais.

Os dias e as horas estão no horário das sessões, mais abaixo nesta página.
(Queremos que se possa carregar nesta frase e ir direto ao horário.)

As salas

O Laboratório Trancado
Um cientista distraído saiu para almoçar e deixou a fórmula secreta fechada
no laboratório. Descobre a fórmula antes de ele voltar.
Dificuldade: média. Boa para uma primeira vez.
(O desenho da sala: uma bancada com três frascos de cores diferentes, à
frente de um quadro com contas a meio, e a porta fechada com um cadeado de
quatro números. Mede 400 por 300 píxeis.)
Legenda: A sala tal como a vais encontrar quando a porta se fechar.

O Sótão dos Relógios
Os relógios do sótão pararam todos a horas diferentes, e só um deles diz a
verdade. Descobre qual é: a hora que ele marca abre o baú.
Dificuldade: difícil. Para equipas que já fizeram uma sala de fuga.

Antes de marcares
As equipas têm de 3 a 5 jogadores.
Cada sessão dura 30 minutos, e o relógio não para.
Podes pedir pistas ao guarda da sala:
    a primeira pista é de graça;
    cada pista a seguir tira 2 minutos ao tempo da equipa.
Os telemóveis ficam num cesto, à porta da sala.

Horário das sessões (cada sessão é só para uma equipa)

                        Laboratório Trancado    Sótão dos Relógios
Quarta-feira, dia 9     14:00                   15:30
Quinta-feira, dia 10    15:30                   14:00
Sexta-feira, dia 11     14:00 e 16:00           15:30

Uma dica de quem já saiu: antes de mexerem em tudo, parem um minuto e digam
em voz alta o que estão a ver.

No fundo de todas as páginas, lado a lado:

Onde estamos                    Fala connosco
Biblioteca, piso 1              salafuga@escola.example
Escola Profissional             Respondemos em dois dias de aulas.
```

## A pasta do site

```text
sala-de-fuga/
├── index.html
└── imagens/
    ├── cadeado.svg
    └── laboratorio.svg
```

Falta o ficheiro da segunda página, a das perguntas frequentes. O nome dele escolhes tu, na parte 2.

## Parte 1: Planear antes de escrever

Responde no caderno, antes de abrires o editor.

**a)** Escreve o índice dos títulos da página, com o nível de cada um, de `h1` a `h6`, e com a indentação a mostrar os níveis.

**b)** Divide a página em zonas, de cima para baixo, e diz que elemento usas em cada uma: `header`, `nav`, `main`, `section`, `article`, `aside` ou `footer`. Para a descrição de cada sala, faz as perguntas do guia pela ordem e diz em qual paraste.

**c)** Na lista "Antes de marcares", duas linhas têm mais recuo do que as outras. O que quer dizer esse recuo? Escreve à mão só as etiquetas dessa lista, sem o texto, com a indentação a mostrar o que fica dentro de quê. Diz também, com o teste da troca, se cada nível da lista é ordenado ou não.

**d)** O clube desenhou duas partes do email em colunas: o horário das sessões e o fundo da página. Uma delas é uma tabela de dados e a outra não. Diz qual é qual, e justifica com o teste do guia. Depois desenha a tabela à mão: o que fica nas linhas, o que fica nas colunas, que células são cabeçalhos e o que pões na célula do canto, que no email está vazia. Para a parte que não é tabela, diz que elementos usas.

## Parte 2: Escrever as duas páginas

**1.** Escreve o `index.html` com tudo o que decidiste na parte 1. Começa pelo esqueleto completo, com a língua certa e um `title` que diga o nome da página e o do site.

**2.** O clube escreveu duas coisas em maiúsculas, porque num email não há negrito nem itálico. Para cada uma, escolhe o elemento que diz o que ela é, e justifica com o guia. No HTML, escreve as duas com letras normais. Explica numa frase porque é que as maiúsculas deixam de ser precisas.

**3.** Duas ligações desta página não levam a outra página. A do horário leva a uma parte desta mesma página, e a do email abre o programa de correio. Procura na secção "Ligações" do guia como se escreve o `href` de cada uma, e escreve-as. Escolhe bem as palavras de cada ligação.

**4.** Escreve a página das perguntas frequentes só com o esqueleto, o mesmo `header` e o mesmo `footer` do `index.html` e, no `main`, o título "Perguntas frequentes" e o parágrafo "Página em construção.". Dá ao ficheiro um nome que siga as regras do guia para os nomes dos ficheiros.

## Parte 3: Verificar

**a)** Abre o `index.html` no browser e lê a página de cima a baixo. Aparece tudo pela ordem do email? As duas imagens aparecem? O fundo da página aparece lado a lado, como o clube o desenhou? Explica porquê, e diz de quem vai ser esse trabalho.

**b)** Lê a página outra vez, mas troca cada imagem pelo seu `alt`, como se a estivesses a descrever ao telefone. A página continua a fazer sentido, sem faltar nada e sem repetir nada? Se não, corrige o `alt`.

**c)** Sem tocar no rato, percorre a página com a tecla Tab. Escreve o texto de cada sítio onde o foco para. Cada um diz sozinho para onde leva? Na ligação do horário, carrega em Enter: a página salta para o sítio certo? Na ligação do email, o computador pode abrir um programa de correio. Se abrir, fecha-o sem enviar nada.

**d)** Segue o menu para as perguntas frequentes e volta à página inicial pelo mesmo menu.

## Desafio opcional

O clube quer que se possa carregar no logótipo para voltar à página inicial, como em muitos sites. Há duas maneiras de o fazer: pôr o logótipo e o nome do site dentro da mesma ligação, ou pôr só o logótipo. Escreve as duas, e diz em cada uma que `alt` fica no logótipo e porquê. A resposta está na secção do guia sobre o texto alternativo. Depois escolhe uma das duas e põe-na nas duas páginas.

## Para ires mais longe

Isto é matéria nova, que não está no guia. Na cábula do Grande Prémio, a secção 8 mostra o elemento `time`. Marca com ele as horas das sessões, na tabela. Repara que cada célula só mostra a hora, mas o atributo `datetime` precisa do ano, do mês, do dia e da hora. Onde vais buscar o que falta? E o que fazes na célula que tem duas horas?

---

# Cábula: o que este exercício acrescenta

As etiquetas que o Grande Prémio já usava, e o esqueleto de uma página, estão na [cábula do fim desse exercício](exercicio-html-grande-premio-1DS-DA.md). Aqui ficam só as que este exercício pede e essa cábula não tinha. Estão todas no guia de HTML e semântica.

## 1. Uma lista dentro de outra

Dentro de um `ul` ou de um `ol` só podem estar elementos `li`. Por isso, uma lista que pertence a um item vai **dentro** do `li` desse item, depois do texto dele, e nunca entre dois `li`.

```html
<ul>
  <li>Traz o teu tabuleiro.</li>
  <li>
    Escolhe a peça que queres estudar:
    <ul>
      <li>o cavalo;</li>
      <li>o bispo.</li>
    </ul>
  </li>
</ul>
```

O browser mostra a lista de dentro mais afastada da margem, com uma bolinha vazia em vez de cheia. As duas listas não têm de ser do mesmo tipo: cada uma passa pelo seu teste da troca.

## 2. Ligações que não levam a outra página

| `href` | Para onde leva | O que é preciso |
| --- | --- | --- |
| `#torneio` | A uma parte da mesma página | O elemento de destino tem o atributo `id="torneio"`. O `id` é único na página e escreve-se em minúsculas, sem espaços e sem acentos |
| `mailto:xadrez@escola.example` | Abre o programa de correio, com o destinatário já preenchido | O endereço vem logo a seguir aos dois pontos, sem espaços |

```html
<p>As <a href="#torneio">datas do torneio</a> estão no fim da página.</p>
<p>Dúvidas: <a href="mailto:xadrez@escola.example">xadrez@escola.example</a></p>

<section id="torneio">
  <h2>Datas do torneio</h2>
  ...
</section>
```

O texto destas ligações segue a regra de todas as outras: diz sozinho para onde leva. "Clica aqui" continua a não servir.

## 3. Uma imagem sozinha dentro de uma ligação

Quando uma imagem é o único conteúdo de uma ligação, o leitor de ecrã lê o `alt` como o nome da ligação. Por isso, o `alt` diz para onde a ligação leva, e não o que a imagem mostra.

```html
<a href="horario.html"><img src="imagens/calendario.svg" alt="Horário dos treinos" width="32" height="32"></a>
```

Se a ligação tiver também texto, o nome dela é esse texto, e o `alt` volta a seguir as regras de sempre.

## 4. Os nomes dos ficheiros

Os nomes dos ficheiros e das pastas escrevem-se em minúsculas, sem espaços e sem acentos, com hífenes entre as palavras: `horario-do-clube.html`, e nunca `Horário do Clube.html`. No teu computador, `Foto.svg` e `foto.svg` podem ser o mesmo ficheiro. No servidor onde o site vai ser publicado, são dois ficheiros diferentes, e a página deixa de encontrar a imagem.
