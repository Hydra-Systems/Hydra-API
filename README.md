# Hydra-API
A simple documentation on the hydra api github, a very fun and generic api :)


### URL base: http://hydrabot.xyz/api/v1/{endpoint}

> Endpoints públicos disponiveis atualmente:



|  EndPoint       | Descrição |
| --------------- |:-------------:|
| /info            | Mostra as informações atuais do Hydra |
| /userAvatar      | Pega um avatar aleatório de algum usuario do Hydra |
| /guildIcon       | Pega um icone aleatório de algum servidor que o Hydra esta |
| /pokemonFront    | Mais de 1100 fotos de frente de pokemons diversos |
| /pokemonBack     | Mais de 750 fotos de frente de pokemons diversos |
| /csgoWallpapers  | Mais de 200 wallpapers diferentes de CS:GO |
| /gtavWallpapers  | Mais de 300 wallpapers diferentes de GTA V |
| /animeWallpapers | Mais de 700 wallpapers diferentes de animes |



# Exemplos de requisição com Node.js
> Modulos utilizados nos exemplos:
### [superagent](https://www.npmjs.com/package/superagent)

```js
// Pegando o wallpaper de GTA e mandando como um arquivo no chat do Discord utilizando um bot
const superagent = require('superagent');

let { body } = await superagent.get('http://hydrabot.xyz/api/v1/gtavWallpapers');

message.channel.send({files: [{ attachment: body, name: 'testing.jpg' }]})
```



