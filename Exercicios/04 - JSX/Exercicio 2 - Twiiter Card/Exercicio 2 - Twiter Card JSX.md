# Exercicio JSX - Formulário Simples

Neste exercicio vamos construir um simples Card para uma rede social:

![alt text](./imagens/exemplo.png)

Exercicio
Para construir este componente de UI necessitamos primiro perceber a sua estrutura.

Faz uma analise da sua estrutura e tentar dividir o elemento em blocos que façam sentido. O "card" foi pensado em ser construido atraves do recursoa tag `<article> *** </article>`.

### Dados para popular o card:

```js
const twiterMessage = {
	author: {
		avatarSrc:
			"https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairTheCaesarSidePart&accessoriesType=Sunglasses&hairColor=BrownDark&facialHairType=BeardLight&facialHairColor=Black&clotheType=BlazerShirt&eyeType=Default&eyebrowType=Default&mouthType=Default&skinColor=Light",
		avatarDescription: "Cartoon Men",
		name: "Nelson Fernandes",
		handle: "nelsonfernandes",
	},
	content:
		"Os últimos serão os primeiros e os do meio sempre serão os do meio.",
	published: "15 de Janeiro as 9:45pm",
};
```

### Criterios

1. Todo o conteudo do card deve ser preenchido com os dados do objeto `twiterMessage`.
2. Ao clicar no nome dever ser possivel navegar para todos os posts do autor deste post navegando para o link `"user/[handlder do utilizador]"`. (Não é necessario existir esta página)
3. Deve ser inserida a palavra "Postado em " antes de inserir a data de publicação

### Notas

Lembra-te que a tag tag `<article>` pode possuir estrututras como o `<header>` e `<footer>` para uma representação semantica e optimizada para SEO.

### Recursos extra

Para podermos utilizar `JSX` no nosso projeto temos de injetar o script do [Babel](https://babeljs.io/repl#?browsers=defaults%2C%20not%20ie%2011%2C%20not%20ie_mob%2011&build=&builtIns=App&corejs=3.21&spec=false&loose=false&code_lz=MYewdgzgLgBArgSxgXhgHgCYIG42AGwEMIIA5QgWwFNkAiUMKQhMKgJ1oD4B5ImAUSxQ0AeizZOAKCA&debug=false&forceAllTransforms=false&modules=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=react&prettier=true&targets=&version=7.20.4&externalPlugins=&assumptions=%7B%7D)

- https://unpkg.com/@babel/standalone/babel.min.js
- script tag do tipo "text/babel"
