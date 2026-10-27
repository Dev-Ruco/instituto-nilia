# Instituto Nília — Website e portal de demonstração

Proposta de voluntariado digital de Felisberto Ruco para apreciação da instituição.

## Executar e alojar

Servir a pasta `dist/` através de qualquer servidor estático. A página principal é `index.html`; o botão “Portal académico” abre `portal.html`. Não há compilação nem dependências de execução. A fonte Manrope é carregada através de Google Fonts, com Arial como alternativa.

## Portal

Interface minimalista em preto e branco, logótipo original, ícones SVG, menu lateral no computador e barra inferior de navegação no smartphone. Listagens passam a fichas em ecrãs pequenos; o horário semanal mantém deslocação horizontal. Animações de entrada repetem-se com o scroll e respeitam movimento reduzido.

Perfis exploráveis de Secretaria, Professor e Encarregado de educação; alunos, turmas, avaliações, presenças, propinas simuladas, horários e mural. Dados fictícios guardados apenas no localStorage. “Repor dados de demonstração” recupera os exemplos iniciais.

Não inclui autenticação de produção, permissões no servidor, pagamentos reais ou ligação aos registos da escola. Os perfis são exclusivamente demonstrativos. Conteúdos e condições institucionais devem ser confirmados pela escola.

## Verificação

Verificadas apresentações de 320 e 378 píxeis e desktop, navegação inferior, menu, edição de avaliações e sintaxe JavaScript.
