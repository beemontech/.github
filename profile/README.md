# Bem vindo ao repositório técnico da Beemôn

## Branches
- Nome da branch segue a o número do card do JIRA
- Use traços para separar palavras
- Seguir os seguintes namespaces
    - `feature/` Implementações de funcionalidades
        - `git checkout -b feature/COD-1234`
    - `improvement/` Melhorias e otimizações em implementaçoes já existente
        - `git checkout -b improvement/COD-1234`
    - `fix/` Correções com prioridade "BAIXA/MÉDIA/ALTA"
        - `git checkout -b fix/COD-1234`
    - `hotfix/` Correções com prioridade "MUITO ALTA"
        - `git checkout -b hotfix/COD-1234`
- Apague seu branch do upstream do repositório depois de integrado (a menos que haja uma razão específica para não fazê-lo).


# Commits
- Cada commit deve ser uma mudança lógica simples. Não faça várias mudanças lógicas em um commit. Por exemplo, se uma alteração corrige um bug e otimiza a performance de uma funcionalidade, o divida em dois commits separados.

- Não divida uma mudança lógica simples em vários commits. Por exemplo, a implementação de uma funcionalidade e os testes correspondentes à ela devem estar no mesmo commit.

- Commit cedo e frequentemente. Commits pequenos e autônomos são mais fáceis de entender e reverter quando algo dá errado.

- Commits devem ser ordenados logicamente. Por exemplo, se commit X depende de uma mudança feita no commit Y, então commit Y deve vir antes do commit X.

- Utilizamos o [Commitizen](https://commitizen-tools.github.io/commitizen/) para geração das tags de versionamento
- Seguimos as seguintes nomenclaturas para geração de MAJOR / MINOR / PATCH
    - Exemplo `1.2.3`, sendo:
        - `1` MAJOR
        - `2` MINOR
        - `3` PATCH
    - Commit para MAJOR
        - Utilize `BREAKING CHANGE:` para subir o MAJOR
        - `git commit -m "BREAKING CHANGE: break change"`
    - Commit para MINOR
        - Utilize `feat:` para subir o MINOR
        - `git commit -m "feat: feature"`
    - Commit para PATCH
        - Utilize `fix:` para subir o PATCH
        - `git commit -m "fix: fix"`

## Pull Request (PR)

- Abra o PR quando finalizar a tarefa ou um PR draft para receber avaliação
- Adicione os "Reviewers". Normalmente é quem criou ou designou a tarefa para você. Caso tenha sido você mesmo que criou a issue, marque ali quem você acredita ser a melhor pessoa para fazer o review dessa tarefa.
- Marque o desenvolvedor da tarefa como "Assignee". Na maioria dos casos, você irá se marcar.
- Selecione as "Labels" fazendo referência a(s) lable(s) da issue.
