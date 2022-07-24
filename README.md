
# API de imagens e ranking de Linguagens de programação

Este projeto foi desenvolvido a partir do evento da escola Alura, da qual a proposta
era criar um gerador de figurinhas utilizando o Java como linguagem principal.
Esta API foi parte da proposta elaborada na imersão, onde desenvolvemos uma API
e hospedamos-a no Heroku, e guardamos os dados no MongoDB.


## Autores

- [@carlosantony](https://www.github.com/carlosantony-dev)

## Apêndice

O campo "ranking" é uma posição fictícia, inserida para fins da elaboração do projeto.


## Rodando localmente

Clone o projeto

```bash
  git clone https://github.com/carlosantony-dev/languagesAPI
```

Entre no diretório do projeto

```bash
  cd languagesAPI
```

Rode através de sua IDE

```bash
  Run =)
```

Acesse seu localhost no subdomínio "/linguagens"
```bash
  Acesse http://localhost:8080/linguagens
```


## Aprendizados

Neste projeto consegui compreender o que é o Spring, como se conectar com o MongoDB,
utilizar Verbos HTTP dentro do Spring e hospedagem do projeto no Heroku disponibilizando
a API na nuvem.


### Documentação da API

#### Retorna todos os itens

```http
  GET https://alura-linguagens-api-br.herokuapp.com/linguagens
```

### Insere um item no Banco de Dados via API
Formato JSON

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `title`      | `string` | **Obrigatório**. O nome da linguagem que deseja inserir|
| `image`       | `string`| **Obrigatório**. O link correspondente a imagem a ser inserida|
| `ranking`     | `int` | **Obrigatório**. A posição do ranking de melhores linguagens |

### Insere um item

```http
    POST https://alura-linguagens-api-br.herokuapp.com/linguagens
```

### Exemplo JSON:

```
  [{"title":"seu-titulo", "image": "sua url", "ranking": "posicao do rank"}]
```

## Licença

[ALURA](https://www.alura.com.br/)
