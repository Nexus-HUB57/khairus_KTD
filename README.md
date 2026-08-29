# khairus_KTD

Repositório de entrega e operação de materiais diretamente vinculados às produções audiovisuais e campanhas de marketing de Kháirus The Dragon (KTD).

## Autoridade

Este repositório é a fonte de verdade para masters de áudio aprovados, imagens finais aprovadas, vídeos finais e clipes aprovados, além das letras originais em inglês, traduções PT-BR de referência, matriz de versões, ledgers de revisão e materiais de marketing diretamente associados a cada obra.

O [`Nexus-HUB57/KAIR-S-SONICA`](https://github.com/Nexus-HUB57/KAIR-S-SONICA) continua sendo a fonte de verdade para produção, co-produção, decisões artísticas, provas, candidatos, rejeitados, históricos, RAG, agentes, workflows, estratégia de mídias sociais, relações públicas, administração, jurídico, contratos e campanhas em desenvolvimento. Este repositório recebe o pacote organizado de entrega/ativação, não substitui o histórico de processo.

A aprovação editorial e a proveniência são obrigatórias. O nome do arquivo sozinho não promove uma prova a material final. Cada asset audiovisual deve estar registrado em `MANIFEST.json`; cada letra ou tradução deve estar registrada em `LYRICS_TRANSLATIONS_MATRIX.json` com status, versão, origem, par, revisão e checksum quando aplicável.

## Estrutura de conteúdo

| Área | Diretório ou arquivo | Regra |
|---|---|---|
| Masters de áudio | `audio/singles/<single>/master/` | Somente masters aprovados ou oficiais de distribuição |
| Vídeos e clipes | `video/singles/` e `video/shorts/` | Somente peças finais ou aprovadas para entrega |
| Imagens | `images/singles/` e `images/artist/` | Somente artes finais aprovadas |
| Original inglês | `lyrics/singles/<single>/original-en/` | Fonte de composição vinculada ao registro de origem |
| Tradução PT-BR | `lyrics/singles/<single>/pt-BR-reference/` | Tradução de referência; não substitui a composição inglesa |
| Ledgers | `lyrics/singles/<single>/reviews/` | Auditoria linha a linha e decisões de revisão |
| Campanhas | `campaigns/<single>/` | Roteiros, captions, hashtags, thumbnails, metadata e peças diretamente vinculadas |
| Controle de letras | `LYRICS_TRANSLATIONS_MATRIX.json` | Matriz central de pares, versões e status |
| Controle audiovisual | `MANIFEST.json` | Proveniência, aprovação, especificações e SHA-256 |
| Checksums | `checksums/SHA256SUMS` | Integridade após cópia, clone ou deploy |

## Regra de idiomas

O inglês é o idioma oficial de composição do catálogo, salvo decisão editorial expressa. As versões PT-BR são traduções de referência para leitura, localização e comunicação. Copiar uma tradução para este repositório não autoriza gravação, sincronização vocal ou publicação de uma versão em português.

Cada par deve manter o original inglês e a tradução PT-BR em diretórios separados. Uma nova redação inglesa, uma mudança de significado ou uma alteração substancial de tradução exige nova versão e novo registro na matriz. A versão anterior deve ser preservada em `archive/` quando tiver valor histórico.

## Regra de status

Os estados `approved_official`, `reference_translation`, `campaign_ready`, `candidate`, `proof`, `rejected` e `archived` devem ser diferenciados. Um texto pendente, uma prova musical ou um asset reprovado não pode ser promovido silenciosamente porque o nome contém `final`, `master` ou `approved`.

A Prova 2 Old School do Single 11 permanece fora do pacote de entrega por estar pendente de avaliação humana. O respectivo material de campanha só poderá entrar quando houver aprovação editorial independente e registro na matriz ou no manifest adequado.

## Integridade e segurança

Use `checksums/SHA256SUMS` para confirmar a integridade dos arquivos audiovisuais. WAV e vídeo grandes são rastreados com Git LFS; manifests, letras e documentos menores permanecem em Git normal.

Não substituir uma versão aprovada silenciosamente. Uma atualização deve preservar o arquivo anterior, registrar a nova versão, atualizar a matriz e usar commit separado. Nenhum token OAuth, App Secret, Client Secret, refresh token, arquivo `.env`, credencial administrativa, contrato privado ou dado de fã deve ser armazenado neste repositório.

## Procedimento de atualização

A atualização deve começar no `KAIR-S-SONICA`, onde a fonte, a aprovação e o status são auditados. Em seguida, o pacote elegível é copiado para o diretório semântico deste repositório, os hashes são recalculados, a matriz ou o manifest é atualizado e a revisão de links e secrets é executada antes do commit.

Durante a transição, as cópias da produção permanecem preservadas. A remoção de duplicatas exige uma alteração futura e explícita, depois de verificar todos os consumidores e o rollback.

## Estado do primeiro lote audiovisual

O batch 001 contém masters de áudio dos Singles 1–5 e três materiais de vídeo explicitamente aprovados ou oficiais. O Lote 1 textual em revisão adiciona os pares inglês/PT-BR dos Singles 4, 5, 7, 8, 9 e 10, com traduções v1 preservadas em `archive/`, traduções v2 revisadas e ledgers linha a linha.

Os arquivos administrativos, jurídicos, credenciais, workflows de infraestrutura, RAG de produção e campanhas ainda em desenvolvimento permanecem no repositório de produção. Apenas os materiais de marketing diretamente vinculados e aprovados para ativação devem ser copiados para `campaigns/`.

## Single 16 — pacote oficial aprovado

O Single 16, **HE DIED KNEELING**, foi aprovado pelo titular em 2026-08-29 na versão musical exata da Prova 6. O pacote público inclui master WAV PCM, MP3 companheiro, letra oficial em inglês, tradução PT-BR de referência, registro de aprovação e relatório de QC. O áudio está registrado no `MANIFEST.json` e o par textual está registrado em `LYRICS_TRANSLATIONS_MATRIX.json`. Nenhum vídeo, capa, thumbnail ou campanha visual está implicitamente aprovado por essa promoção.
