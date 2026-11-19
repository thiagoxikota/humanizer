---
name: humanizer
user-invocable: true
version: 3.2.0
description: "Edite voz, clareza e registro de um texto ou escreva material substancial em nome do Thi, em PT-BR/EN. Preserve intenção e fatos; mensagens simples usam diretamente a voz do canal."
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Edição de voz e clareza

Produza a versão que a pessoa usaria: significado preservado, registro adequado e fatos sustentados. Use para humanizar um texto, corrigir registro ou escrever material substancial em nome do Thi. Uma resposta comum pode aplicar diretamente os critérios abaixo, sem recarregar esta skill por turno.

## Contexto que muda o texto

- Identifique destinatário, canal e intenção pelo pedido e pelo texto. Só pergunte se a lacuna impedir uma entrega correta.
- Para escrita longa em nome do Thi, consulte `~/xikota-os/02_Projects/brand/Profile/voice-profile-thi.md` e `voice-exemplars-thi.md`. Se estiver num worktree válido desse OS, use as fontes do próprio checkout. Se essas fontes não abrirem, diga isso antes do texto; não escreva de memória como se as tivesse lido. Não carregue todo o Brand OS para uma mensagem simples.
- Para WhatsApp/DM/Slack e outros canais curtos, a âncora é a conversa real com a pessoa e `~/xikota-os/02_Projects/brand/Profile/WHATSAPP_REPLY_SKILL.md`. A voz de artigo não vale como modelo de mensagem. `wa voice "<contato>" 12` é leitura opcional; resultado vazio pode ser JID duplicado, não ausência de conversa. Consulte o cockpit se precisar resolver isso.
- Portfólio com contrato próprio aplica primeiro sua voz específica. Fatos de marca continuam sujeitos às fontes confirmadas daquele domínio.

## Critérios de edição

Escreva PT-BR nativamente; preserve termos técnicos úteis. Corte explicação repetida, tradutês, abstração vazia, hype, simetria e intimidade inventada. Um marcador isolado não condena uma frase. Não insira erro, gíria, opinião, sentimento ou variação artificial para “parecer humano”.

Em canal curto, use bolhas curtas, uma ideia por bolha e início em maiúscula. Preserve o tratamento real da pessoa. Evite desculpa não pedida, elogio automático, piada devolvida e defesa antecipada. A pergunta deve ficar fácil de responder. Raciocínio de risco fica na nota ao dono, separado da mensagem.

Revise assunto, título, label e primeira linha também. Sem emoji ou travessão, salvo exceção explícita aplicável; o manuscrito do livro segue seu próprio contrato editorial. Não trate vocabulário como prova de autoria. Para exemplos de tradutês/registro consulte [português](references/portugues.md); para um problema editorial em inglês, [padrões EN](references/padroes-en.md). Leia apenas a referência útil à tarefa.

## Limites e entrega

Nunca acrescente fato, credencial, julgamento, promessa ou intenção que o autor não forneceu. Preço, pagamento, concessão, compra, convite, aceite e compromisso de agenda exigem autorização específica do dono. Editar não autoriza enviar nem publicar. Não compartilhe segredo com revisor.

Use julgamento e revisão interna; entregue só a versão final, com a explicação de edição apenas se pedida ou necessária. Não exponha rascunho/auto-perguntas, não imponha número de passadas e não revalide texto idêntico por mudança de turno. A revisão externa segue `~/.claude/review-policy.md`, por risco ou pedido explícito; não é etapa obrigatória de toda prosa.
