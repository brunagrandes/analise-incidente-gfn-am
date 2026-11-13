# analise-incidente-gfn-am
# Análise de Incidente Cibernético: GeForce NOW / GFN.am (2026)

## Sobre o projeto

Este projeto analisa o vazamento de dados de usuários do GeForce NOW ocorrido em 2026 no GFN.am, parceiro regional da NVIDIA que opera o serviço de jogos na nuvem na Armênia. O objetivo é entender como o incidente aconteceu, quais foram os impactos e, principalmente, o que ele ensina sobre **gestão de risco de terceiros** e **governança de segurança**.

A análise usa apenas informações públicas. O que não foi divulgado pelas empresas está marcado como hipótese.

## Resumo do caso

- **43 dias** entre o início da invasão (20 de março) e a detecção (2 de maio)
- **5 tipos de dados pessoais** expostos: e-mail, telefone, data de nascimento, nome completo e nome de usuário. As senhas não foram afetadas
- **US$ 100 mil** foi o preço pedido pela base em um fórum de cibercrime, sob o nome ShinyHunters (o grupo negou a autoria)
- Segundo a NVIDIA, **nenhum sistema operado por ela foi afetado**: a base invadida era do parceiro

## Linha do tempo

| Data | Evento |
|---|---|
| 9 mar 2026 | Data de corte: só contas criadas até aqui estão na base exposta |
| 20 a 26 mar 2026 | Período da invasão ao banco de dados, segundo o GFN.am |
| 2 mai 2026 | GFN.am detecta o incidente |
| 5 mai 2026 | GFN.am divulga o vazamento; NVIDIA confirma e delimita o escopo |
| Mai 2026 | Base anunciada por US$ 100 mil; anúncio sai do ar |

## O que foi analisado

- Contexto e partes envolvidas (NVIDIA, GFN.am e usuários)
- Dados expostos e riscos para os usuários
- Etapas do ataque pela **Cyber Kill Chain**, separando fatos de hipóteses
- **Avaliação de risco** qualitativa (probabilidade x impacto)
- Resposta ao incidente pelas fases do **NIST SP 800-61**
- **Visão de GRC**: lacunas na gestão de terceiros e controles sugeridos (ISO 27001, NIST CSF 2.0)
- Como a **LGPD** trataria um caso parecido no Brasil
- Recomendações e lições aprendidas

## Principal conclusão

> A marca era da NVIDIA. O controle dos dados era do parceiro.

Para o usuário, quem falhou foi o GeForce NOW. Quando um parceiro guarda dados de clientes em nome de uma empresa, a reputação dessa empresa depende da segurança dele. Terceirizar a operação não terceiriza o risco.

## Lições aprendidas

- **Terceirizar a operação não terceiriza o risco:** contratos com parceiros precisam de requisitos mínimos de segurança, direito de auditoria e prazo para avisar incidentes.
- **Detectar é tão importante quanto prevenir:** 43 dias de exposição aumentam o dano e o custo da resposta.
- **Menos dados guardados, menos dados vazados:** minimização é controle de segurança, não só exigência legal.
- **Comunicar cedo e com clareza preserva confiança:** delimitar o escopo logo no início ajudou a separar fatos de boatos.

## Apresentação completa

A análise detalhada está no PDF deste repositório: [Ver apresentação](./analise-incidente-gfn-am.pdf)

## Fontes

- HotHardware, TweakTown, Cybersecurity News, Notebookcheck, Daily Security Review e ThreatCluster (cobertura do caso, maio de 2026)
- Lei nº 13.709/2018 (LGPD) e Resolução CD/ANPD nº 15/2024
- ISO/IEC 27001:2022, NIST Cybersecurity Framework 2.0 e NIST SP 800-61

## Projeto de estudo

Desenvolvido por **Bruna Grandes Rodrigues** como parte da trilha de Cibersegurança da Cisco Networking Academy, pelo programa Mulher Digital (Junior Achievement Brasil), com foco em Governança, Risco e Conformidade (GRC).
