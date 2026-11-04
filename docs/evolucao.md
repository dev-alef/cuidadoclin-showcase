# Evolução e limites

## Implementação e piloto

Contas e clínicas, papéis, sessões, equipe, isolamento na API e no banco, documentos personalizados, interface responsiva e demo separada. Backend e interface passaram por revisão independente; os achados foram corrigidos e revalidados. O piloto da clínica original foi publicado em 04/11/2026.

## Evidências disponíveis

- PostgreSQL real descartável com papel restrito: isolamento, vínculos, convites e concorrência.
- Backup e restauração com dados sintéticos e verificação de campos cifrados.
- Cinco fluxos pessoais de PDF, seis páginas, com comparação raster ao baseline para entradas equivalentes.
- Jornadas da interface: cadastro parcial sem duplicação, troca de clínica, permissões, PDFs e logout.
- Demo offline sem requisições HTTP; build normal separado dos dados de exemplo.

A data civil foi corrigida para evitar deslocamento de dia por fuso. Essa correção intencional de conteúdo não é apresentada como visualmente idêntica à data errada anterior.

## Publicação de 04/11/2026

O backup criptografado do piloto foi restaurado em PostgreSQL isolado e conferido. A conta legada mantém o mesmo hash de senha e o vínculo de administrador + dentista; a chave clínica e o modelo pessoal de PDF foram preservados. A API usa um papel restrito, e migrações deixaram de ser executadas automaticamente pelo deploy.

Onze verificações passaram pelo endereço publicado, com uma conta temporária sem vínculos clínicos: login, cookie seguro, sessão após recarregar, acesso negado sem vínculo, CSRF e logout, entre outras. A conta temporária e suas sessões foram removidas. O teste não utilizou a senha pessoal do profissional; sua preservação foi verificada no banco.

O site institucional do cliente passou a ter repositório privado e deploy independentes do produto SaaS. Este showcase continua exclusivamente documental, com imagens fictícias.

Entrega real de e-mail não foi verificada. Convites/reset na interface foram também exercitados com respostas sintéticas; isso não prova entrega. O piloto admite links privados preparados pelo operador, sem prometer e-mail automático.

## Fora do escopo

Cobrança, cadastro aberto, agenda nova, assinatura digital, anexos clínicos e outras especialidades. Não há data de lançamento ou certificação regulatória anunciada.
