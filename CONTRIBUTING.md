# Guia de Contribuicao - Paycon Automacoes

## Estrategia de branches

Utilizamos o seguinte fluxo:

- **main** - producao, protegida, somente via PR aprovado
- **develop** - integracao, protegida, recebe features finalizadas
- **feature/*** - branches de desenvolvimento, criadas a partir de develop

### Fluxo padrao

1. Crie uma branch a partir de develop: git checkout -b feature/minha-feature develop
2. Desenvolva e faca commits claros e objetivos
3. Abra um Pull Request para develop
4. Aguarde review (humano + IA)
5. Apos aprovacao, o merge sera feito

## Convencao de commits

Siga o padrao Conventional Commits (https://www.conventionalcommits.org/):

Formato: tipo(escopo): descricao curta

Exemplos:
- feat(odoo): adicionar modulo de faturamento
- fix(rpa): corrigir timeout no robo de consulta
- docs: atualizar contributing.md
- chore(infra): atualizar versao do docker

Tipos aceitos: feat, fix, docs, style, refactor, test, chore, ci, perf

## Padrao de Pull Request

Todo PR deve seguir o template disponivel no repositorio. Verifique:

- Descricao clara do que foi feito
- Tipo de mudanca marcado
- Issue relacionada vinculada
- Passos para testar
- Checklist do autor preenchido

## Code Review

- Todo PR exige pelo menos 1 reviewer
- O bot de IA fara uma revisao automatica sugestiva
- Push direto em main e develop e proibido
- PRs com mais de 400 linhas devem ter justificativa

## Seguranca

- Nunca commite secrets, tokens ou credenciais
- Use variaveis de ambiente para configuracoes sensiveis
- Reporte vulnerabilidades conforme descrito em SECURITY.md

## Padrao de codigo

- Python: siga as regras do Ruff (linter configurado no CI)
- Mantenha o codigo legivel e documentado
- Escreva testes para funcionalidades criticas

## Duvidas

Entre em contato com o time via os canais internos da Paycon.
