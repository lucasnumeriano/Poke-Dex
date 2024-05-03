# Poké-Dex

![Pokémon](https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/International_Pok%C3%A9mon_logo.svg/1200px-International_Pok%C3%A9mon_logo.svg.png)

Não há dúvida de que a maior parte de nossa infância foi gasta assistindo Pokémon e jogando jogos como Pokémon Fire-Red, Ruby, Emerald, etc. De Kanto a Hoenn a Sinnoh, nós vimos tudo e experimentamos tudo. Com o Hacktoberfest 2020 chegando e sendo uma das pessoas que participaria pela primeira vez, decidi criar este repositório que na verdade é um site muito básico que permite aos usuários visualizar e adicionar seus Pokémon favoritos.

# Conteúdo do site

1. index.html - Contém o conteúdo da página inicial.
2. index.css - Contém o estilo dado à página inicial.
3. about.html - Contém algumas informações sobre mim.
4. about.css - Contém o estilo dado à página "sobre".

# O que posso contribuir?

Sempre há algo para contribuir em um projeto, seja você um novato ou um veterano. Neste projeto, você pode adicionar seu Pokémon favorito como um card ao site! Ou talvez você não tenha gostado da linha que está lendo agora e queira mudá-la. Claro! Por que não?

# Como posso contribuir?

Por favor, consulte o arquivo [contributing_pt-BR](https://github.com/AM1CODES/Poke-Dex/blob/master/contributing_pt-BR.md) para aprender como contribuir!

E é isso!
Siga esses passos para fazer sua primeira solicitação de pull.

# Mas e se eu não souber como adicionar cards? :(

Não é todo mundo que está ciente de todas as ferramentas presentes no mundo, não importa o quão fácil ou complexa seja. Também não é necessário conhecer todas as ferramentas lá fora. Então, existem duas maneiras de adicionar um Pokémon. **Você só precisa fazer uma** desses métodos, caso contrário, o Pokémon aparecerá duas vezes.

## via html

Use o exemplo de código abaixo para adicionar seu próprio card porque todo mundo ama Pokémon e todos deveriam ter a chance de adicionar seu Pokémon favorito! Basta colar dentro da div com um id de `pokemon-row`

```html
<div class="col-lg-4 mb-4">
  <div class="card">
    <img class="card-img-top" src="[Link para a imagem do Pokémon]" alt="" />
    <div class="card-body">
      <h5 class="card-title">[Nome do seu Pokémon favorito]</h5>
      <p class="card-text">[Pequena descrição sobre o seu Pokémon]</p>
      <a
        href="[Adicione o link para o seu perfil no GitHub]"
        class="btn btn-outline-danger btn-sm"
        >Contribuído por - [Adicione seu nome de usuário/nome do perfil do GitHub]</a
      >
    </div>
  </div>
</div>
```

Agora também é possível usar uma nova classe css para adicionar um distintivo ao seu Pokémon favorito, este distintivo é feito para mostrar o tipo do Pokémon. Siga o exemplo

```html
<div class="col-lg-4 mb-4">
  <div class="card">
    <div class="header">
      <div class="badge grass">Grass</div>
    </div>
    <img class="card-img-top" src="[Link para a imagem do Pokémon]" alt="" />
    <div class="card-body">
      <h5 class="card-title">[Nome do seu Pokémon favorito]</h5>
      <p class="card-text">[Pequena descrição sobre o seu Pokémon]</p>
      <a
        class="btn btn-outline-danger btn-sm"
        href="[Adicione o link para o seu perfil no GitHub]"
        >Contribuído por - [Adicione seu nome de usuário/nome do perfil do GitHub]</a
      >
    </div>
  </div>
</div>
```

Atualmente, os distintivos disponíveis são: grass, bug, electric, dark, fairy, fighting, fire, flying, ghost, ground, ice, normal, poison, psychic, rock, steel, water. Sinta-se à vontade para adicionar mais, basta criar uma classe com o nome do tipo e escolher a cor.

Copie este código e cole no arquivo index.html para fazer suas alterações. Teste-o em seu próprio sistema e depois crie uma solicitação de pull.

## via javascript / json

Ou uma maneira ainda mais fácil é apenas adicionar um objeto ao arquivo `pokemon.json` com

```json
{
	"pokemonName": [Nome do seu Pokémon favorito],
	"pokemonDescription": [Pequena descrição sobre o seu Pokémon],
	"pokemonImage": [Link para a imagem do Pokémon],
	"contributedByName": [Adicione seu nome de usuário do Github],
	"contributedByUrl": [Adicione um link para o seu perfil no Github],
	// esses são necessários apenas se você melhorou um card
	"improvedByName": [Adicione seu nome de usuário do Github],
	"improvedByUrl": [Adicione um link para o seu perfil no Github],
},
```

Se todos os Pokémon forem adicionados a este arquivo, podemos expandir este projeto para incluir funcionalidades como pesquisa e filtragem.

# Parabéns!

Parabéns! Você acabou de fazer sua primeira solicitação de pull e se ela for mesclada, você poderá ver as alterações que fez ao vivo usando o link fornecido acima!