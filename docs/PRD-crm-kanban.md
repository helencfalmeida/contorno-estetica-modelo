# CRM em Kanban · Contorno Estética

Documento do produto (PRD) · versão 1 · outubro de 2026

> A Contorno Estética é uma clínica fictícia, criada para o IA Sem Segredo. Nomes, números e casos são inventados.

---

## 1. Por que fazer este CRM

Hoje a Nina anota cada contato numa planilha e escreve a situação "do jeito que dá na hora". Na planilha de exemplo, com 80 clientes, aparecem estes problemas:

- **A situação é escrita de 12 jeitos diferentes** ("fez avaliação", "avaliação?", "ligar de novo", "sumiu", "não respondeu", "achou caro", "vai pensar", "remarcar"...). Não dá para saber, de bater o olho, em que ponto cada cliente está.
- **Cerca de 1 em cada 10 clientes está sem situação nenhuma**, e várias estão sem data do último contato. Essas clientes ficam esquecidas.
- **Faltam origem e interesse em várias linhas**, então a Paula não consegue saber de onde vêm as clientes que fecham pacote.
- **As datas não têm ano**, o que vai confundir a partir de janeiro.
- **Ninguém sabe quem precisa de retorno hoje.** As regras de retorno existem no roteiro do WhatsApp, mas dependem da memória da Nina.
- **Informações importantes ficam soltas na observação** ("só pode sábado", "prefere áudio", "quer parcelar", "pediu foto de antes e depois").

**O objetivo do CRM:** cada cliente vira um cartão num quadro com colunas. O cartão anda de coluna em coluna conforme a cliente avança, e o sistema avisa quem precisa de retorno e quando.

**Como vamos saber que deu certo:**
- Nenhuma cliente sem etapa e sem data de próximo retorno.
- Nenhum retorno atrasado no fim do dia.
- A taxa de avaliações que viram pacote (hoje 4 em cada 10) fica visível para a Paula toda semana, e a meta é subir.

---

## 2. Quem usa

| Pessoa | Papel na clínica | O que faz no CRM |
|---|---|---|
| **Nina** | Recepção e WhatsApp | É a dona do quadro no dia a dia. Cadastra cada contato novo, move os cartões, registra cada conversa e trabalha a lista "Retornos de hoje". Envia as propostas. |
| **Otávio** | Biomédico esteta: avaliações, criolipólise e laser | Vê a agenda de avaliações. Depois de cada avaliação, registra o tratamento indicado e monta a proposta (tratamento, número de sessões, valor) dentro do cartão. Registra o retorno de 60 dias da criolipólise. |
| **Camila** | Terapeuta corporal: drenagem e modeladora | Vê as clientes em tratamento corporal. Marca cada sessão feita, para o sistema contar quantas faltam. |
| **Paula** | Fundadora, define preços e exceções | Vê o quadro inteiro e o painel de números. É a única que aprova exceções, sempre por escrito dentro do cartão. |

Todas usam pelo celular e pelo computador.

---

## 3. As etapas do funil (as colunas do quadro)

O quadro tem 7 colunas na ordem do caminho da cliente, mais 1 coluna separada para quem desistiu.

| # | Coluna | Quando o cartão entra aqui | Quem move para a próxima |
|---|---|---|---|
| 1 | **Novo contato** | A cliente mandou a primeira mensagem (WhatsApp, Instagram, Google, indicação, fachada). | Nina |
| 2 | **Em conversa** | A Nina já respondeu, a cliente pediu preço ou tirou dúvida, mas ainda não marcou a avaliação. | Nina |
| 3 | **Avaliação marcada** | A avaliação gratuita está com dia e hora marcados. | Nina (ou Otávio, ao fazer a avaliação) |
| 4 | **Proposta enviada** | A cliente fez a avaliação, o Otávio montou a proposta e a Nina enviou (sempre no mesmo dia da avaliação). | Nina |
| 5 | **Fechou pacote** | A cliente pagou ou assinou o pacote e falta fazer a 1ª sessão. | Quem registrar a 1ª sessão |
| 6 | **Em tratamento** | A 1ª sessão foi feita. O cartão mostra quantas sessões faltam e a data limite do pacote. | Sistema (quando a última sessão é marcada) |
| 7 | **Pós-venda** | O pacote terminou. Hora de pedir a opinião, a indicação e oferecer o próximo tratamento. | Nina (fecha o cartão ou abre um novo pacote) |
| — | **Perdido** | A cliente disse não, ou não respondeu depois de 3 tentativas. É obrigatório escolher o motivo. | Nina |

**Regras de movimento:**
- O cartão **não pode ir para "Fechou pacote" sem passar por "Avaliação marcada"** com a avaliação registrada como feita. A clínica só vende pacote depois da avaliação.
- Cartão em **"Perdido" pode voltar** para "Em conversa" a qualquer momento, quando a cliente reaparecer.
- Na coluna **"Proposta enviada"**, a Nina pode marcar uma etiqueta de situação: *achou caro*, *vai pensar* ou *quer parcelar*. Isso não cria coluna nova, só ajuda na conversa de retorno.

### Como as situações da planilha atual viram colunas

| Situação escrita hoje | Vai para a coluna |
|---|---|
| (em branco) | Novo contato (retorno no mesmo dia) |
| pediu preço · ligar de novo · não respondeu | Em conversa |
| marcou avaliação · remarcar · avaliação? | Avaliação marcada (a Nina confirma a data; "avaliação?" e "remarcar" ganham retorno no mesmo dia) |
| fez avaliação · achou caro · vai pensar | Proposta enviada (com a etiqueta correspondente) |
| fechou pacote | Fechou pacote (a Nina confirma se já começou; se sim, vai para Em tratamento) |
| sumiu | Em conversa, com 1 tentativa já contada. Se não responder, segue a regra das 3 tentativas. |

---

## 4. Os dados de cada cliente (o que fica no cartão)

Campos marcados com ★ são obrigatórios. As listas fechadas existem para acabar com o "cada um escreve de um jeito".

### Identificação
| Campo | Como preenche | Observação |
|---|---|---|
| Nome ★ | Texto | |
| Telefone / WhatsApp ★ | Número com DDD | O sistema avisa se o número já existe (evita cliente repetida). |
| Data de entrada ★ | Automático | Dia, mês **e ano**. |

### De onde veio e o que quer
| Campo | Como preenche | Opções |
|---|---|---|
| Origem ★ | Lista | Instagram · Instagram (anúncio) · Google · Indicação · Fachada · Outro |
| Indicada por | Texto | Aparece só quando a origem é "Indicação". Hoje "veio pela amiga" está escrito na observação, mesmo quando a origem marcada é Google. |
| Interesse ★ | Lista (pode marcar mais de um) | Limpeza de pele · Peeling de diamante · Microagulhamento · Drenagem linfática · Massagem modeladora · Criolipólise · Depilação a laser · Ainda não sabe |
| Área | Automático | Rosto ou Corpo, a partir do interesse. |

### Andamento
| Campo | Como preenche | Observação |
|---|---|---|
| Etapa ★ | Coluna do quadro | |
| Responsável ★ | Lista | Nina por padrão. |
| Último contato ★ | Automático | Atualiza sempre que alguém registra uma conversa. |
| Próximo retorno ★ | Automático | Calculado pelas regras da seção 5. Pode ser ajustado à mão. |
| Tentativas sem resposta | Automático | Conta de 0 a 3. Volta a zero quando a cliente responde. |
| Histórico | Automático | Lista de cada conversa: data, quem falou e um resumo curto. |

### Avaliação e proposta
| Campo | Como preenche |
|---|---|
| Data e hora da avaliação | Data |
| Avaliação feita? | Sim / Não / Faltou |
| Tratamento indicado pelo Otávio | Lista (mesma do interesse) |
| Valor da proposta | R$ |
| Forma de pagamento | Pix à vista (10% de desconto) · Débito · Crédito em até 6x |
| Data de envio da proposta | Data |
| Etiqueta da proposta | achou caro · vai pensar · quer parcelar |

### Pacote e tratamento
| Campo | Como preenche |
|---|---|
| Pacote fechado | Tratamento + número de sessões |
| Data da 1ª sessão | Data |
| Validade do pacote | Automático: 6 meses depois da 1ª sessão |
| Sessões feitas / sessões contratadas | Contagem (Camila, Otávio ou Paula marcam a cada sessão) |
| Profissional | Paula (rosto) · Otávio (criolipólise e laser) · Camila (drenagem e modeladora) |

### Preferências e cuidados (etiquetas)
Etiquetas clicáveis, que aparecem na frente do cartão:
- **Só pode sábado**
- **Prefere áudio**
- **Quer parcelar**
- **Já fez em outra clínica**
- **Perguntou do resultado** → mostra o lembrete: *"Explicar o que o tratamento costuma fazer. Nunca prometer resultado em centímetro ou em quilo."*
- **Pediu foto de antes e depois** → mostra o lembrete: *"Só usar foto de cliente com autorização por escrito."*

### Autorização e perda
| Campo | Como preenche |
|---|---|
| Autoriza uso de foto de antes e depois | Sim / Não + data da autorização por escrito |
| Motivo da perda ★ (só na coluna Perdido) | Achou caro · Não respondeu (3 tentativas) · Fechou em outra clínica · Horário não serve · Desistiu do tratamento · Outro |
| Exceção aprovada pela Paula | Texto + data. Só a Paula preenche. |
| Observação livre | Texto, para o que não couber nos campos acima |

---

## 5. As regras de retorno

O CRM calcula sozinho a data do **próximo retorno** de cada cartão e monta, todo dia de manhã, a lista **"Retornos de hoje"** para a Nina, com os atrasados no topo em vermelho.

### Regras que já existem no roteiro da clínica
| Situação | Quando a Nina volta a falar |
|---|---|
| Contato novo parou de responder | **1 dia** depois do último contato |
| Fez a avaliação e não respondeu à proposta | **2 dias** depois do envio da proposta |
| Comprou o pacote | Mensagem de pós-venda **7 dias** depois da compra |
| Contato sem data | **No mesmo dia** |
| Fez a 1ª sessão | Retorno da Nina depois da 1ª sessão (está incluído em todo pacote) |
| Fez criolipólise | Consulta de retorno com o Otávio **60 dias** depois da aplicação |

### Regras novas, que completam o roteiro
| Situação | Quando |
|---|---|
| Cliente não responde | Até **3 tentativas**. Depois da 3ª sem resposta, o cartão vai para "Perdido" com o motivo "Não respondeu (3 tentativas)". |
| Contatos perdidos | Voltam para a lista de retornos **60 dias** depois, uma única vez, com uma mensagem de reaproximação. |
| Avaliação marcada | Lembrete para a cliente **na véspera** da avaliação. |
| Cliente faltou à avaliação ou pediu para remarcar | Retorno **no mesmo dia**. |
| Cartão com etiqueta "achou caro" ou "vai pensar" | Mesmo prazo da proposta (2 dias). O cartão mostra as formas de pagamento como apoio: 6x sem juros ou 10% à vista no Pix. Desconto acima de 10% não existe. |
| Retorno da 1ª sessão | **1 dia** depois da 1ª sessão. |
| Microagulhamento | Lembrete para marcar a próxima sessão **25 dias** depois da última (o intervalo é de 30 dias). |
| Criolipólise | Lembrete para marcar o retorno com o Otávio **53 dias** depois da aplicação, para caber na agenda dos 60 dias. |
| Pacote perto de vencer | Aviso **30 dias** antes da validade de 6 meses, se ainda houver sessões sobrando. |
| Fim do pacote (Pós-venda) | Mensagem pedindo opinião e indicação **7 dias** depois da última sessão. Novo contato oferecendo o próximo tratamento **30 dias** depois. |

### Regras do calendário
- O retorno sempre cai dentro do horário comercial: **segunda a sexta, das 9h às 19h, e sábado, das 9h às 13h**.
- Se a data cair no domingo ou num feriado, passa para o próximo dia útil.
- Para cliente com a etiqueta **"Só pode sábado"**, o CRM sugere os horários de sábado de manhã.
- Para cliente com a etiqueta **"Prefere áudio"**, o lembrete avisa a Nina para responder por áudio.

---

## 6. Regras que o CRM não deixa quebrar

1. **Só vende pacote depois da avaliação.** O cartão não chega em "Fechou pacote" sem avaliação feita.
2. **Desconto máximo de 10%, só à vista no Pix.** O campo de valor não aceita desconto maior. Exceção de outro tipo só com aprovação da Paula, registrada no cartão.
3. **Nunca prometer resultado em centímetro ou em quilo.** Lembrete automático em cartões com a etiqueta "Perguntou do resultado".
4. **Foto de antes e depois só com autorização por escrito.** O cartão mostra se a cliente autorizou.
5. **Proposta enviada no mesmo dia da avaliação.** Se a avaliação foi feita e a proposta não foi enviada até o fim do dia, o cartão fica vermelho.

---

## 7. O painel da Paula

Uma tela simples, com os números da semana e do mês:
- Contatos novos por semana (hoje, cerca de 45) e de onde vieram.
- Avaliações feitas e quantas viraram pacote (hoje, 4 em cada 10), por origem e por tratamento.
- Valor médio do pacote (hoje, R$ 1.180).
- Retornos atrasados no dia.
- Clientes perdidas por motivo.
- Pacotes perto de vencer.

---

## 8. Passar a planilha atual para o CRM

1. Importar as 80 clientes da planilha atual.
2. Usar a tabela da seção 3 para colocar cada uma na coluna certa.
3. Considerar o ano de 2026 em todas as datas.
4. Ler a coluna de observação e transformar em etiqueta ("só pode sábado", "prefere áudio", "quer parcelar", "já fez em outra clínica", "perguntou do resultado", "pediu foto de antes e depois"). "Veio pela amiga" vira origem Indicação.
5. Clientes sem origem ou sem interesse ficam marcadas com "A completar". A Nina completa na próxima conversa.
6. Clientes sem data de último contato entram na lista "Retornos de hoje" do primeiro dia.

---

## 9. Fora desta primeira versão

- Envio automático de mensagens pelo WhatsApp. Nesta versão o CRM avisa e a Nina envia.
- Agenda completa das salas e das profissionais.
- Controle financeiro, nota fiscal e estoque de produtos.
- Venda dos produtos para usar em casa.

---

## 10. Pontos para a Paula confirmar

Estas regras são sugestões, porque os documentos da clínica não dizem o prazo:
- Retorno depois da 1ª sessão: **1 dia** está bom?
- Lembrete de véspera da avaliação: a clínica quer?
- Contatos perdidos: tentar de novo **60 dias** depois, uma única vez?
- Pós-venda: oferecer o próximo tratamento **30 dias** depois do fim do pacote?
- Camila e Otávio podem mover cartões ou só marcar sessões e avaliações?
