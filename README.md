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


## Galeria de fotografias restauradas e navegação móvel

A galeria automática apresenta sete versões restauradas das fotografias fornecidas: geologia, música, desporto, laboratório, sala de aula, simulação clínica e formação profissional. Os ficheiros estão em `assets/nilia-*.webp`, optimizados sem deformação. O enquadramento completo é mantido com `object-fit: contain`.

Os controlos são discretos e ficam abaixo das fotografias: anterior, seguinte, indicadores e pausa. Há navegação por deslize horizontal e teclas de seta. A apresentação alterna a cada 6,5 segundos e pausa quando a galeria fica fora do ecrã, a página perde visibilidade ou o foco entra nos controlos. A preferência de movimento reduzido inicia a galeria em pausa.

No telemóvel, os textos e as acções aparecem antes da galeria. Uma barra fixa dá acesso a Ensino, Admissões e Ligar à escola; o espaço inferior da página acomoda essa barra. Os itens do menu têm áreas de toque amplas. A ordem do documento acompanha a apresentação móvel.

Verificadas as vistas de 320 e 378 píxeis sem deslocamento horizontal, a abertura e o fecho do menu e os controlos da galeria. A publicação mantém a audiência anterior do protótipo.
