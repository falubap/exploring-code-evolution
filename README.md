# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: https://github.com/vuetifyjs/vuetify

2. Gráfico selecionado: Lines of Code (LOC)
  
3. Explicação: O vuetify é uma popular library de UI com componentes vue.js já prontos para serem incorporados em qualquer projeto. O número de linhas de código do projeto teve um crescimento amortecido desde o seu início até o ano de 2022, a partir do qual esse número começou a cair aceleradamente. Enquanto em 2022 o vuetify atingiu o seu pico histórico de 74251 linhas de código, no atual momento (maio de 2025), ele conta com 36694 linhas de código. No ano de estreia do vuetify ele já contava com 63439 linhas de código, o que quer dizer que no atual momento o projeto apresenta quase metade do volume de linhas de código em relação ao seu início. Que o número de linhas de código de um projeto diminua ao longo dos anos pode, a princípio, parecer um fato contraintuitivo, porém ao analisar a história do vuetify podem ser encontradas algumas justificativas para tal fenômeno. O primeiro deles, e talvez o principal é, foi a migração do projeto de vue.js 2 para vue.js 3, framework no qual ele está construído. O vue.js, até sua segunda versão, apresentava uma estrutura que era conhecida como "Options API", e partir da versão 3, passou a adotar a chamada "Composition API". Esta, por sua própria natureza faz com que o desenvolvedor utilize menos linhas de código pois apresenta uma estrutura de projeto mais modularizada, e, como o próprio nome indica, focada na componentização do código. Além disso, também houveram outras mudanças que impactaram no número de linhas de código como a adoção de Tree Shaking, que é uma ténica JavaScript para remover automáticamente código não utilizado no momento do build, a importação seletiva de componentes, remoção de funcionalidades obsoletas ou pouco utilizadas e remoção de seletores CSS não utilizados por meio da ferramenta nuxt-purgecss. Em resumo, uma série de eventos de refatoração e melhorias no vuetify fez com que o projeto apresentasse essa queda brusca no número de linhas de código, o que não indica que o projeto tenha ficado pior, mas ao contrário agora está mais otimizado e organizado. 



