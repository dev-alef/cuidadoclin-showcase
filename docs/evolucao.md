# Evolução do CuidadoClin

## Base atual

Gestão de pacientes, histórico de anamnese e geração de documentos, com uma conta administrativa e um modelo visual específico.

## Primeira versão SaaS — escopo confirmado

- Contas individuais.
- Clínicas independentes no mesmo produto.
- Permissões por associação à clínica.
- Separação de dados entre clínicas.
- Identidade visual e documentos personalizados por clínica.
- Preservação do modelo de documentos da clínica de origem.

Esses itens são planejados. O repositório público não representa conclusão da implementação.

## Critérios propostos para verificar a versão

| Cenário | Evidência esperada |
| --- | --- |
| Usuário de uma clínica tenta acessar paciente de outra | Operação recusada no servidor |
| Usuário tenta emitir documento de outra clínica | Operação recusada, sem PDF ou dados do paciente |
| Duas clínicas emitem documentos | Cada PDF utiliza apenas a identidade correspondente |
| Revogação do acesso de um membro | Requisições posteriores deixam de ser autorizadas |
| Migração da clínica de origem | Dados e documentos preservados, com ensaio em ambiente isolado |

A matriz detalhada de permissões e a estratégia de verificação serão fechadas no plano técnico.

## Depois da primeira versão

Expansão para outras especialidades, orientada por necessidades verificadas. Cobrança de assinaturas, integrações e novos módulos deverão ser priorizados separadamente. Não há datas de lançamento prometidas neste documento.
