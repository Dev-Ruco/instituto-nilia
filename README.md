# Instituto Nília — Protótipo institucional

Proposta independente de voluntariado digital desenvolvida por Felisberto Ruco, sujeita à apreciação do Instituto Nília.

## Executar

Abra `index.html` num navegador. Para servir localmente:

```sh
python3 -m http.server 8080
```

Aceda a http://localhost:8080. Não exige instalação de dependências nem compilação.

## Publicar num servidor

Copie `index.html` e a pasta `assets/` para a pasta pública do alojamento, como `public_html` ou `www`. O projecto usa HTML, CSS e JavaScript e pode ser servido por Apache, Nginx ou outro servidor de ficheiros estáticos.

## Funcionalidades

- Apresentação institucional e dos três níveis de ensino.
- Detalhes das etapas de ensino em janelas de diálogo.
- Localização das unidades Tivane e Magumbwé.
- Menu adaptável a telemóveis.
- Preparação de pedidos de informações por `mailto:`. O visitante confirma o envio no seu programa de correio electrónico.

## Limites do protótipo

Não inclui sistema de gestão académica, autenticação, pagamentos, base de dados nem submissão de matrículas. As fotografias são carregadas do site institucional e dependem da sua disponibilidade. O logótipo fornecido está incluído localmente em `assets/logotipo-nilia.jpg`. A utilização definitiva dos conteúdos e da identidade institucional deve ser acordada com a instituição. Antes da publicação institucional, validar os contactos, requisitos, propinas e conteúdos.

## Estrutura

- `index.html`: página, estilos e interacções.
- `assets/logotipo-nilia.jpg`: logótipo original fornecido.
- `README.md`: documentação do projecto.
- `.gitignore`: exclusões de ficheiros locais.

## Referências

- https://institutonilia.edu.mz/
- https://www.facebook.com/profile.php?id=100057280066749

## Identidade visual

O símbolo original é preservado, sem recoloração. A identidade do website combina laranja e terracota com superfícies suaves e texto de elevado contraste.

| Cor | Código | Aplicação |
| --- | --- | --- |
| Laranja | `#F25625` | Símbolo e pequenos destaques |
| Terracota | `#B64221` | Botões e títulos de destaque |
| Marfim | `#FFFAF5` | Fundo principal |
| Pêssego suave | `#F6E5D9` | Secção institucional |
| Areia rosada | `#FAEADE` | Área de admissões |
| Castanho escuro | `#342B28` | Texto principal |

O branco é usado junto ao logótipo para preservar o fundo do ficheiro original. A tipografia usa Manrope (400–800), carregada através de Google Fonts, com Arial como alternativa. As proporções do símbolo são preservadas com `object-fit: contain`.

## Composição e tipografia

Revisão inspirada na organização de conteúdos educativos do UX Design Institute: hierarquia sem serifa, títulos de maior presença, fotografias rectangulares, separadores discretos e oferta de ensino apresentada em linhas. A referência não implica afiliação institucional.

Os tamanhos e a composição ajustam-se a computador, tablet e telemóvel. O símbolo original e a paleta suave são preservados. A fonte externa depende da disponibilidade de Google Fonts; Arial serve de alternativa.

## Template dinâmico

Nova composição com títulos Manrope em peso 800, botões arredondados, cartões de ensino, secção institucional escura e superfícies suaves em pêssego. O cabeçalho adapta-se à deslocação e uma linha indica o progresso de leitura.

As secções e os cartões entram no ecrã através de IntersectionObserver. O scroll controla pequenos deslocamentos das fotografias e dos cartões, com requestAnimationFrame e eventos passivos. Há também uma faixa tipográfica em movimento, elementos flutuantes e transições nos botões.

A preferência `prefers-reduced-motion` desactiva animações e movimentos. Sem JavaScript, os conteúdos mantêm-se visíveis. A vista móvel foi verificada a 378 pixels.
