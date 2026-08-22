# khairus_KTD

Repositório exclusivo dos **materiais audiovisuais finalizados de Kháirus The Dragon (KTD)**.

## Autoridade

Este repositório é a fonte de verdade para masters de áudio aprovados, imagens finais aprovadas, vídeos finais e clipes aprovados para entrega. Briefings, letras, provas, demos, candidatos, rejeitados, históricos, RAG, campanhas, workflows, relações públicas, administração e jurídico permanecem em [`Nexus-HUB57/KAIR-S-SONICA`](https://github.com/Nexus-HUB57/KAIR-S-SONICA).

A aprovação editorial é obrigatória. O nome do arquivo sozinho não promove uma prova a material final. Cada item deve estar registrado em `MANIFEST.json` com status, origem, decisão, checksum SHA-256 e especificações técnicas.

## Conteúdo do primeiro lote

O primeiro lote contém masters de áudio aprovados dos Singles 1–5 e três materiais de vídeo explicitamente aprovados ou oficiais. Não contém provas pendentes, demos, takes, stems, referências de identidade, imagens de produção ou materiais reprovados.

| Área | Diretório |
|---|---|
| Masters de áudio | `audio/singles/<single>/master/` |
| Shorts/clipes aprovados | `video/shorts/<single>/approved/` |
| Vídeos/clipes aprovados | `video/singles/<single>/approved/` |
| Checksums | `checksums/SHA256SUMS` |

## Integridade e atualização

Use `checksums/SHA256SUMS` para confirmar a integridade após clone, download ou deploy. Arquivos WAV e vídeo são rastreados com Git LFS; os manifests e arquivos menores permanecem em Git normal.

Não substituir um master aprovado silenciosamente. Uma nova versão exige nova entrada de manifest, decisão editorial explícita e commit separado. O repositório de produção deve apontar para o commit do arquivo final, e este repositório deve apontar para o documento de aprovação de origem.

A Prova 2 Old School do Single 11 permanece fora deste repositório até aprovação humana. O repositório também não contém tokens OAuth, App Secrets, Client Secrets, refresh tokens, dados administrativos privados ou dados de fãs.
