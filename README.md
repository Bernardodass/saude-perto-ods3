# Saúde Perto

Protótipo acadêmico para Programação Orientada a Objetos, com foco no ODS 3.

## Problema e proposta

O projeto explora como organizar informações de serviços de saúde num catálogo pesquisável. O público pensado são moradores que querem localizar informações por bairro ou tipo de serviço. A proposta se relaciona ao ODS 3, Saúde e Bem-Estar. O protótipo usa quatro fichas fictícias explicitamente identificadas. A fonte pública proposta para uma versão futura é o [Cadastro Nacional de Estabelecimentos de Saúde (CNES/DATASUS)](https://cnes.datasus.gov.br/). Esta versão ainda não integra os dados do CNES.

## Como executar

Extraia o ZIP e abra `index.html` no navegador. Para usar com um servidor local, abra a pasta no terminal, rode `python -m http.server 8000` e acesse `http://localhost:8000`. O protótipo funciona sem dependências externas. A persistência dos favoritos depende de o navegador permitir armazenamento local.

## Fluxo da demonstração

1. Busque por **Parque Horizonte** e selecione **Vacinação**.
2. Abra a ficha **Ponto de vacinação Estação**.
3. Salve a ficha, abra **Salvos** e confira que ela aparece.
4. Abra a ficha salva e remova-a. Volte à lista para ver o estado vazio.

## Tecnologias e modelagem

HTML para estrutura, CSS para layout responsivo e JavaScript para navegação e regras de negócio. A classe `Servico` guarda os dados de uma ficha e verifica os filtros. `Catalogo` concentra a pesquisa, e `Favoritos` separa a persistência da interface. O protótipo não coleta dados de saúde, contatos ou localização.

## Evolução demonstrada nesta proposta

A ideia de um catálogo virou um fluxo navegável com filtro combinado, detalhes e favoritos persistentes.

## Capturas do protótipo

- [Catálogo](demo/catalogo.jpg)
- [Busca e filtro combinados](demo/busca.jpg)
- [Detalhes da ficha salva](demo/detalhes.jpg)
- [Lista de favoritos](demo/salvos.jpg)

## Demonstração

- [Abrir o protótipo](https://bernardodass.github.io/saude-perto-ods3/)
- [Assistir ao vídeo com legendas](demo/demonstracao.mp4)

## Roteiro de apresentação

- **0:00–0:15** — Apresente o problema e o ODS 3. Explique que os registros são fictícios.
- **0:15–0:35** — Demonstre a busca por bairro, o filtro por categoria e a abertura de uma ficha.
- **0:35–0:50** — Salve a ficha e mostre a tela de favoritos. Remova a ficha para demonstrar a atualização.
- **0:50–1:00** — Mostre no código as classes Servico, Catalogo e Favoritos. Diga que integrar dados oficiais é uma etapa futura.
