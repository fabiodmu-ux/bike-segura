# 🤝 Contribuindo para Bike Segura

Obrigado por considerar contribuir para o **Sistema Bike Segura**! Este documento oferece diretrizes e instruções para contribuir.

## 📋 Código de Conduta

Todos os contribuidores devem seguir nosso Código de Conduta:
- Respeito mútuo e profissionalismo
- Zero tolerância a discriminação ou assédio
- Feedback construtivo e colaborativo

## 🐛 Reportando Bugs

Encontrou um bug? Ótimo! Aqui está como reportar:

### Antes de Submeter um Bug Report
- **Faça uma busca** nas [issues](https://github.com/fabiodmu-ux/bike-segura/issues) para garantir que não foi reportado
- **Verifique a documentação** e tente reproduzir o problema

### Como Submeter um Bug Report
Crie uma [issue](https://github.com/fabiodmu-ux/bike-segura/issues/new) com:

```markdown
**Descrição do Bug**
Descrição clara e concisa do problema

**Passos para Reproduzir**
1. Passo 1
2. Passo 2
3. Passo 3

**Comportamento Esperado**
O que deveria acontecer

**Comportamento Atual**
O que realmente aconteceu

**Screenshots**
Se aplicável, adicione capturas de tela

**Ambiente**
- OS: [ex. Ubuntu 22.04]
- Browser: [ex. Chrome 120]
- Versão: [ex. 1.0.0]
```

## 💡 Sugerindo Melhorias

Tem uma ideia legal? Compartilhe conosco!

### Como Submeter uma Sugestão
Crie uma [issue](https://github.com/fabiodmu-ux/bike-segura/issues/new) com:

```markdown
**Descrição da Melhoria**
Explique sua ideia e por que seria útil

**Casos de Uso**
Quando e como seria usado

**Alternativas Consideradas**
Outras soluções possíveis

**Contexto Adicional**
Qualquer outro detalhe relevante
```

## 🔨 Desenvolvimento Local

### Setup de Desenvolvimento

1. **Fork o repositório**
   ```bash
   # Clique no botão Fork no GitHub
   ```

2. **Clone seu fork**
   ```bash
   git clone https://github.com/seu-usuario/bike-segura.git
   cd bike-segura
   ```

3. **Adicione upstream**
   ```bash
   git remote add upstream https://github.com/fabiodmu-ux/bike-segura.git
   ```

4. **Instale dependências**
   ```bash
   npm install
   ```

5. **Crie uma branch**
   ```bash
   git checkout -b feature/sua-feature
   # ou
   git checkout -b fix/seu-bug-fix
   ```

### Padrões de Nomenclatura de Branch
- `feature/descricao-curta` - Nova funcionalidade
- `fix/descricao-do-bug` - Correção de bug
- `docs/descricao` - Documentação
- `refactor/descricao` - Refatoração de código
- `test/descricao` - Testes

### Executando Testes
```bash
npm test              # Testes unitários
npm run test:e2e      # Testes end-to-end
npm run test:coverage # Cobertura de testes
```

### Verificar Qualidade de Código
```bash
npm run lint          # Verificar linting
npm run format        # Formatar código
npm run build         # Build do projeto
```

## 📝 Estilo de Código

### JavaScript/TypeScript
- Use **ESLint** para linting
- Siga **Prettier** para formatação
- Use **camelCase** para variáveis e funções
- Use **PascalCase** para classes e componentes
- Comentários explicativos em português

### Exemplos
```typescript
// ✅ Bom
const obterUsuarioById = (id: string): User => {
  return usuarios.find(u => u.id === id);
};

// ❌ Ruim
const get_user_by_id = (id) => usuarios.find(u => u.id === id);
```

## 📦 Commits

### Mensagens de Commit
Use o formato **Conventional Commits**:

```
<tipo>(<escopo>): <descrição>

<corpo>

<rodapé>
```

### Tipos de Commit
- `feat`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Documentação
- `style`: Formatação (sem lógica)
- `refactor`: Refatoração (sem mudança de funcionalidade)
- `perf`: Melhoria de performance
- `test`: Adicionar/atualizar testes
- `chore`: Tarefas de build/CI/CD

### Exemplos
```
feat(auth): integrar autenticação com Gov.br

Implementa login federado usando OAuth2 do Gov.br.
Adiciona validação de token e refresh token.

Closes #123
```

```
fix(bikes): corrigir geração de QR code

O QR code não era gerado corretamente para bicicletas
com caracteres especiais no número de série.

Closes #456
```

## 🔄 Submetendo Pull Requests

### Antes de Submeter

1. **Atualize sua branch**
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Execute testes**
   ```bash
   npm test
   ```

3. **Verifique linting**
   ```bash
   npm run lint
   ```

4. **Build do projeto**
   ```bash
   npm run build
   ```

### Criando o PR

1. **Push para seu fork**
   ```bash
   git push origin feature/sua-feature
   ```

2. **Abra um PR no GitHub**
   - Descreva claramente as mudanças
   - Referencie issues relacionadas (#123)
   - Adicione screenshots/gifs se aplicável

### Template de PR
```markdown
## Descrição
Breve descrição do que este PR faz.

## Tipo de Mudança
- [ ] Bug fix
- [ ] Nova funcionalidade
- [ ] Breaking change
- [ ] Documentação

## Issues Relacionadas
Closes #123

## Testes
- [ ] Testes unitários adicionados
- [ ] Testes E2E adicionados
- [ ] Cobertura mantida/aumentada

## Checklist
- [ ] Código segue o estilo do projeto
- [ ] Documentação atualizada
- [ ] Sem console logs ou código de debug
- [ ] Testes passam localmente
```

## 📚 Documentação

- Todas as novas funcionalidades **devem** ter documentação
- Atualize o README.md se necessário
- Adicione exemplos de uso
- Documente decisões arquiteturais em docs/

## ✅ Revisão de Código

Os revisores procuram por:
- ✅ Código funciona corretamente
- ✅ Testes adequados
- ✅ Sem problemas de segurança (LGPD, criptografia)
- ✅ Performance aceitável
- ✅ Documentação clara
- ✅ Segue o estilo do projeto

## 📖 Recursos

- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [Semantic Versioning](https://semver.org/)

## 📞 Precisa de Ajuda?

- 💬 Abra uma discussão: [Discussions](https://github.com/fabiodmu-ux/bike-segura/discussions)
- 🐛 Report de bug: [Issues](https://github.com/fabiodmu-ux/bike-segura/issues)

---

**Obrigado por contribuir! 🎉**