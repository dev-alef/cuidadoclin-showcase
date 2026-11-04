# Evolução e limites

## Concluído na implementação local

Contas e clínicas, papéis, sessões, equipe, isolamento na API e no banco, documentos personalizados, interface responsiva e demo separada. Backend e interface passaram por revisão independente; os achados foram corrigidos e revalidados.

## Evidências disponíveis

- PostgreSQL real descartável com papel restrito: isolamento, vínculos, convites e concorrência.
- Backup e restauração com dados sintéticos e verificação de campos cifrados.
- Cinco fluxos pessoais de PDF, seis páginas, com comparação raster ao baseline para entradas equivalentes.
- Jornadas da interface: cadastro parcial sem duplicação, troca de clínica, permissões, PDFs e logout.
- Demo offline sem requisições HTTP; build normal separado dos dados de exemplo.

A data civil foi corrigida para evitar deslocamento de dia por fuso. Essa correção intencional de conteúdo não é apresentada como visualmente idêntica à data errada anterior.

## Antes da publicação SaaS

Recuperar acesso operacional, restaurar backup atual em ambiente isolado, validar proxy/cookies na hospedagem e executar migração coordenada. A produção ainda não foi migrada; o usuário legado deverá manter sua senha e receber vínculo de administrador + dentista na clínica de origem.

Entrega real de e-mail não foi verificada. Convites/reset na interface foram também exercitados com respostas sintéticas; isso não prova entrega. O piloto admite links privados preparados pelo operador, sem prometer e-mail automático.

## Fora do escopo

Cobrança, cadastro aberto, agenda nova, assinatura digital, anexos clínicos e outras especialidades. Não há data de lançamento ou certificação regulatória anunciada.
