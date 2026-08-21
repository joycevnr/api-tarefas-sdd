# Convenções

## Idioma
- Código em inglês; artefatos SDD (spec, design, tasks) em português.

## Organização
- src/routes/ (HTTP), src/services/ (regra de negócio), src/db/ (dados).
- Um teste por rota e por regra, em *.test.ts ao lado do arquivo.

## Nomenclatura
- Rotas no plural (/tasks); função de serviço começa por verbo (createTask).

## Anti-padrões (o que NÃO fazer)
- Regra de negócio na rota: mora no service.
- 500 genérico para falha de validação: use 400 com mensagem.
- Query solta na rota: todo acesso a dados passa por src/db/.
