# Busca Bike Scraper

Projeto voltado para raspagem de anúncios de bicicletas a venda nas plataformas como OLX, Mercado Livre, entre outros.

## Instalação

1. Faça o checkout do projeto:

```shell
$ git clone https://github.com/rochacbruno/buscabike-scraper.git
```

2. Crie o ambiente virtual e instale as dependências:

```shell
$ cd buscabike-scraper
$ python3 -m venv .venv
```

```shell
$ source .venv/bin/activate
$ pip install -r requirements.txt
```

3. Rode o spider desejado. Nesse exemplo será coletado anúncios na OLX.

```shell
$ scrapy crawl olx
```

Os dados coletados segue a estrutura de exemplo abaixo:

```json
{
  "_id": "<id do documento>",
  "url": "http://df.olx.com.br/distrito-federal-e-regiao/ciclismo/bicicleta-aro-24-435226286",
  "type": "Ciclismo",
  "price": " R$ 500,00",
  "created_at": "ISODate('2018-01-04T16:56:42.669Z')",
  "posted_at": "8 Janeiro às 16:15",
  "image": "http://img.olx.com.br/images/35/357804005117894.jpg",
  "district": "Santa Maria",
  "cep": "72505-222",
  "title": "Setor Total Ville",
  "description": "Descrição do anúncio",
  "owner": "Nome do Dono da bicicleta"
  "city": "Brasília",
  "phone": "(61) 99999-9999"
}
```

## Como Contribuir
Veja mais no arquivo `CONTRIBUTING.md`, as formas de ajudar com o projeto, e o `AUTHORS.md` para saber quem estão a frente e que pode te auxiliar.
