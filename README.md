# Commits Semânticos: A Importância e Como Utilizar

## O que são Commits Semânticos?

Commits semânticos são uma convenção para escrever mensagens de commit que seguem uma estrutura específica, proporcionando uma história do projeto mais legível e significativa. O objetivo é tornar claro o propósito de cada mudança no código, facilitando a colaboração entre desenvolvedores e a automatização de processos como versionamento e geração de changelogs.

## Estrutura de um Commit Semântico

A estrutura básica de uma mensagem de commit semântico segue este formato:

<tipo>(<escopo opcional>): <descrição curta>

<mensagem detalhada opcional> <footer opcional>```

Componentes
Tipo: Indica o propósito da mudança. Exemplos:

[feat]: Adição de uma nova funcionalidade.
[fix]: Correção de um bug.
[chore]: Tarefas de manutenção, sem impacto no código de produção (como atualizações de dependências).
[docs]: Alterações na documentação.
[style]: Mudanças que não afetam a lógica, como formatação.
[refactor]: Alterações que melhoram o código sem modificar o comportamento.
[perf]: Melhorias de desempenho.
[test]: Adição ou correção de testes.
[build]: Mudanças em arquivos de build ou dependências externas.
[ci]: Alterações em arquivos ou scripts de configuração de integração contínua.
[Escopo]: Indica a área do projeto que foi afetada, como um módulo ou componente. Este campo é opcional, mas útil para especificar melhor o contexto da alteração.

* Descrição Curta: Um resumo direto e objetivo da alteração. Deve ser conciso e, de preferência, não ultrapassar 50 caracteres.

* Mensagem Detalhada (Opcional): Aqui você pode explicar o "porquê" da mudança, o contexto que levou à decisão e detalhes adicionais sobre como a alteração foi feita.

* Footer (Opcional): Utilizado para referências específicas, como problemas fechados (Closes #123) ou notas de breaking changes.

Exemplos de Commits Semânticos
1. Commit de nova funcionalidade
```scss
feat(auth): adiciona autenticação via OAuth2
```
Este commit indica que uma nova funcionalidade foi adicionada relacionada ao módulo de autenticação, especificamente para suporte ao OAuth2.

2. Commit de correção de bug
```scss
fix(api): corrige erro ao validar token JWT
```
Aqui, a mensagem descreve a correção de um bug relacionado à validação de tokens JWT na API.

3. Commit de documentação
```scss
docs(readme): adiciona instruções para configuração do ambiente
```
Este commit faz referência a uma mudança na documentação, especificamente no arquivo README.md.

4. Commit de refatoração
```lua
refactor(core): remove código duplicado em serviços
```
Esse commit refatora o código, eliminando duplicações no core do projeto, sem alterar o comportamento do software.

5. Commit de tarefa (chore)
```scss
chore(deps): atualiza dependências do projeto
```
Este commit indica que houve uma atualização das dependências, mas não traz mudanças no comportamento ou funcionalidade do código.

6. Commit de otimização de desempenho
```scss
perf(db): otimiza consultas SQL para melhorar o tempo de resposta
```
Aqui, a melhoria está no desempenho do banco de dados, especificamente nas consultas SQL.

## Benefícios dos Commits Semânticos
1. Leitura Facilitada da História do Projeto: Com uma estrutura padronizada, fica mais fácil para desenvolvedores, revisores e futuros mantenedores entenderem o histórico de mudanças.

2. Automação do Versionamento: Utilizando ferramentas como o Semantic Release, é possível automatizar o versionamento do projeto com base nos tipos de commit (feat, fix, etc.), garantindo um controle eficiente de versões.

3. Geração Automática de Changelog: Ferramentas como o Conventional Changelog podem gerar changelogs automáticos com base nas mensagens de commit, destacando novas funcionalidades, correções e mudanças significativas.

4. Facilidade de Revisão: Commits bem documentados ajudam a entender o contexto de cada alteração durante o processo de code review, reduzindo ambiguidades.

## Dicas para Escrever Commits Semânticos
Seja conciso, mas claro: Evite mensagens vagas como "correções", "ajustes", ou "melhorias". Diga exatamente o que foi feito e por que.
Utilize o formato correto: As mensagens de commit semânticas seguem uma convenção clara e estruturada. Respeite essa convenção para maximizar os benefícios.
Divida commits grandes: Se possível, divida grandes alterações em commits menores e significativos. Isso facilita o entendimento e a rastreabilidade das mudanças.
Ferramentas para Ajudar no Uso de Commits Semânticos
Existem várias ferramentas e plugins que podem ser integrados ao fluxo de trabalho para garantir a conformidade com commits semânticos:

1. Commitlint: Valida as mensagens de commit de acordo com as convenções estabelecidas.
2. Husky: Utilizado para rodar o Commitlint automaticamente no pre-commit hook.
3. Semantic Release: Automatiza o processo de versionamento e publicação de novas versões com base nos commits semânticos.
## Conclusão
Os commits semânticos são uma prática poderosa para manter um histórico de mudanças claro, coeso e útil. Além de melhorar a comunicação entre desenvolvedores, eles facilitam a automatização de tarefas importantes como versionamento e changelogs. Ao adotar essa prática, você contribui para um desenvolvimento de software mais organizado e eficiente.