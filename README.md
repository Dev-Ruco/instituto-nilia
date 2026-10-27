# Instituto Nília — Protótipo institucional

Proposta independente de voluntariado digital desenvolvida por Felisberto Ruco, sujeita à apreciação do Instituto Nília.

## Executar

Abra `index.html` num navegador. Para servir localmente:

```sh
python3 -m http.server 8080
```

Aceda a http://localhost:8080. Não exige instalação de dependências nem compilação.

## Publicar num servidor

Copie `index.html` para a pasta pública do alojamento, como `public_html` ou `www`. O projecto usa HTML, CSS e JavaScript e pode ser servido por Apache, Nginx ou outro servidor de ficheiros estáticos.

## Funcionalidades

- Apresentação institucional e dos três níveis de ensino.
- Detalhes das etapas de ensino em janelas de diálogo.
- Localização das unidades Tivane e Magumbwé.
- Menu adaptável a telemóveis.
- Preparação de pedidos de informações por `mailto:`. O visitante confirma o envio no seu programa de correio electrónico.

## Limites do protótipo

Não inclui sistema de gestão académica, autenticação, pagamentos, base de dados nem submissão de matrículas. As fotografias e o logótipo são carregados do site institucional e dependem da sua disponibilidade. A utilização definitiva dos conteúdos e da identidade institucional deve ser acordada com a instituição. Antes da publicação institucional, validar os contactos, requisitos, propinas e conteúdos.

## Estrutura

- `index.html`: página, estilos e interacções.
- `README.md`: documentação do projecto.
- `.gitignore`: exclusões de ficheiros locais.

## Referências

- https://institutonilia.edu.mz/
- https://www.facebook.com/profile.php?id=100057280066749
