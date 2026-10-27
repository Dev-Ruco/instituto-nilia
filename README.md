# Instituto Nília — Protótipo institucional

Proposta independente de voluntariado digital desenvolvida por Felisberto Ruco, sujeita à apreciação do Instituto Nília.

## Executar

Abra `index.html` num navegador ou execute:

```sh
python3 -m http.server 8080
```

Aceda a http://localhost:8080. Não exige dependências nem compilação.

## Alojamento

Copie `index.html` e a pasta `assets/` para a pasta pública do servidor. Apache, Nginx e alojamentos de ficheiros estáticos são compatíveis.

## Funcionalidades

- Apresentação da escola, etapas de ensino e unidades.
- Detalhes das etapas em janelas de diálogo com nomes acessíveis.
- Menu móvel com acesso às admissões, fecho por Escape e clique no exterior.
- Ligação directa para telefonar à secretaria.
- E-mail preparado a partir das opções seleccionadas; o envio é confirmado pelo visitante no seu programa de correio electrónico.
- Entradas animadas uma única vez por elemento; transições nos botões e progresso de leitura.
- Conteúdos visíveis sem JavaScript e suporte à preferência de movimento reduzido.

## Identidade visual

Logótipo original fornecido, sem recoloração; títulos Manrope em peso 800 e paleta de laranja, terracota, marfim e pêssego. A fonte é carregada através de Google Fonts, com Arial como alternativa.

A revisão de usabilidade coloca o título e o contacto antes da fotografia no telemóvel, aumenta os textos de leitura e elimina elementos decorativos em movimento contínuo. As fotografias estão guardadas em `assets/`, optimizadas em WebP, com dimensões declaradas no HTML.

## Verificação

Verificadas as vistas de 378 e 320 píxeis, sem deslocamento horizontal, o menu móvel, os detalhes das etapas e a ligação de e-mail com a etapa seleccionada. A sintaxe JavaScript foi validada com `node --check`.

## Limites

Não inclui gestão académica, autenticação, pagamentos, base de dados nem submissão de matrículas. Horários, distribuição das classes pelas unidades e condições de ingresso devem ser confirmados com a instituição. As fotografias e a identidade institucional requerem validação da escola antes de utilização definitiva.

## Estrutura

- `index.html`: página, estilos e interacções.
- `assets/`: logótipo e fotografias.
- `README.md`: documentação.
- `.gitignore`: exclusões locais.

## Referências

- https://institutonilia.edu.mz/
- https://www.facebook.com/profile.php?id=100057280066749

