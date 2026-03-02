# Como Contribuir

Obrigado por querer contribuir com este repositório! Siga as instruções abaixo para garantir um fluxo de trabalho organizado.

## Git Flow

Este projeto adota uma versão simplificada do **Git Flow**. As branches principais são:

| Branch    | Descrição                                                    |
|-----------|--------------------------------------------------------------|
| `main`    | Código estável e pronto para produção                        |
| `develop` | Branch de integração onde as features são consolidadas       |

### Tipos de branches de suporte

| Prefixo        | Quando usar                                      | Exemplo                         |
|----------------|--------------------------------------------------|---------------------------------|
| `feature/`     | Novas funcionalidades ou melhorias               | `feature/tela-de-login`         |
| `fix/`         | Correção de bugs                                 | `fix/corrige-botao-enviar`      |
| `hotfix/`      | Correção urgente diretamente na `main`           | `hotfix/corrige-crash-inicial`  |
| `docs/`        | Apenas alterações em documentação                | `docs/atualiza-readme`          |
| `chore/`       | Tarefas de manutenção (configurações, scripts…)  | `chore/atualiza-dependencias`   |

---

## Passo a passo para contribuir

### 1. Fork e clone

```bash
# Faça um fork do repositório no GitHub e então clone o seu fork
git clone https://github.com/<seu-usuario>/ihc.git
cd ihc
```

### 2. Configure o repositório original como remote

```bash
git remote add upstream https://github.com/marcmec/ihc.git
```

### 3. Crie uma branch a partir de `develop`

```bash
git checkout develop
git pull upstream develop
git checkout -b feature/nome-da-sua-feature
```

### 4. Faça suas alterações

- Mantenha os commits pequenos e com mensagens descritivas.
- Use o padrão abaixo para mensagens de commit:

```
<tipo>: <descrição curta no imperativo>

Exemplos:
feat: adiciona tela de perfil do usuário
fix: corrige alinhamento do menu lateral
docs: adiciona seção de instalação no README
```

Tipos sugeridos: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.

### 5. Sincronize com `develop` antes de abrir o PR

```bash
git fetch upstream
git rebase upstream/develop
```

### 6. Abra um Pull Request

1. Envie sua branch para o seu fork: `git push origin feature/nome-da-sua-feature`
2. Abra um **Pull Request** do seu fork para `develop` neste repositório.
3. Descreva claramente **o que** foi feito e **por que**.
4. Aguarde a revisão. Fique atento a possíveis pedidos de alteração.

---

## Boas práticas

- Nunca faça commits diretamente em `main` ou `develop`.
- Mantenha as branches com escopo pequeno e focado em uma única tarefa.
- Escreva mensagens de commit em português ou inglês, de forma consistente.
- Certifique-se de que o código está funcionando antes de abrir o PR.

---

## Dúvidas?

Abra uma [issue](https://github.com/marcmec/ihc/issues) descrevendo o problema ou sugestão.
