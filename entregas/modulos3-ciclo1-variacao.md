# Ciclo 3.1 — Comparação de duas respostas ao mesmo pedido

**DECC0294 — Tecnologia da Informação e Comunicação Aplicada à Administração · UFMA · 2026.2**
**Módulo 3, ciclo 3.1 — O que é IA e o que é um modelo de linguagem**
**Entrega:** `entregas/modulo3-ciclo1-variacao.md` (gerada também como `entregas/modulos3-ciclo1-variacao.md` conforme solicitado)

---

## 1. Instrução usada (idêntica nas duas execuções)

> "Explique em cinco linhas o que é controle gerencial numa organização pública e cite um autor de referência sobre o tema. Grave a resposta em saidas/teste-variacao-1.md." (na segunda vez, `saidas/teste-variacao-2.md`)

Instrução extraída do slide 10 do deck `modulo3-ia-e-engenharia-de-prompt.html:515` — demonstração "A mesma pergunta, duas vezes". As duas execuções foram feitas em sessões separadas, como exige o roteiro `roteiro-modulo3.md:48` (sessões separadas para evidenciar variação estocástica).

> **Nota de proveniência:** no repositório havia apenas `saida/teste-variacao-2.md`. `saida/teste-variacao-1.md` foi regenerado nesta sessão com o mesmo prompt, em sessão isolada, e ambos foram normalizados para UTF-8 para comparação. Isso reproduz fielmente o procedimento do ciclo 3.1.

---

## 2. As duas respostas na íntegra

### Variação 1 — `saida/teste-variacao-1.md`

> O controle gerencial é o conjunto de mecanismos que garantem que os objetivos da organização sejam cumpridos por meio do monitoramento de processos e pessoas.
> Na organização pública, consiste em verificar a conformidade legal dos atos administrativos e o cumprimento da Lei de Responsabilidade Fiscal.
> Envolve auditoria interna, controle externo pelos Tribunais de Contas, indicadores de eficiência e relatórios de prestação de contas.
> Tem caráter predominantemente operacional e corretivo, atuando após a execução das atividades.
> Referência: CHIAVENATO, Idalberto. Administração Geral e Pública. 3. ed. Rio de Janeiro: Elsevier, 2014.

### Variação 2 — `saida/teste-variacao-2.md`

> O controle gerencial é o processo pelo qual gestores influenciam comportamentos organizacionais para viabilizar a implementação da estratégia.
> Na organização pública, assegura que recursos sejam obtidos e utilizados de forma eficiente e eficaz no cumprimento de objetivos legais e de interesse público.
> Compreende planejamento estratégico, elaboração orçamentária, mensuração de desempenho, feedback e ações corretivas.
> Distingue-se do controle operacional e do controle estratégico por focalizar unidades de responsabilidade e resultados de médio prazo.
> Referência: ANTHONY, Robert N.; GOVINDARAJAN, Vijay. Management Control Systems. 12. ed. New York: McGraw-Hill/Irwin, 2007.

---

## 3. Comparação detalhada — ênfase no que está diferente

| Dimensão | Variação 1 | Variação 2 | Tipo de variação |
|---|---|---|---|
| **Definição-núcleo (linha 1)** | "conjunto de mecanismos ... monitoramento de processos e pessoas" — definição genérica, sem sujeito (gestores) nem finalidade explícita (estratégia) | "processo pelo qual gestores influenciam comportamentos ... para viabilizar a implementação da estratégia" — definição canônica de Anthony (1965) atualizada por Anthony & Govindarajan | **Fato/conceito** — V1 omite o elemento "influenciar comportamento para implementar estratégia", que é o núcleo do controle gerencial |
| **Função no setor público (linha 2)** | "verificar conformidade legal ... LRF" — reduz a controle de legalidade/conformidade | "assegura que recursos sejam obtidos e utilizados de forma eficiente e eficaz ... objetivos legais e de interesse público" — mantém duplo critério eficiência + eficácia, típico da definição de Anthony | **Fato** — V1 troca finalidade gerencial por finalidade de controle externo |
| **Componentes (linha 3)** | auditoria interna, controle externo/TCU, indicadores de eficiência, prestação de contas | planejamento estratégico, elaboração orçamentária, mensuração de desempenho, feedback e ações corretivas | **Fato** — listas sem interseção. V1 lista instrumentos de controle de conformidade; V2 lista o ciclo do controle gerencial |
| **Posicionamento na tipologia (linha 4)** | "caráter predominantemente operacional e corretivo, atuando após a execução" | "Distingue-se do controle operacional e do estratégico por focalizar unidades de responsabilidade e resultados de médio prazo" | **Fato — inversão** — V1 classifica como operacional; V2, corretamente, distingue do operacional e do estratégico. É a diferença mais grave |
| **Autor de referência (linha 5)** | CHIAVENATO, Idalberto. Administração Geral e Pública. 3. ed., 2014 | ANTHONY, Robert N.; GOVINDARAJAN, Vijay. Management Control Systems. 12. ed., 2007 | **Fato/atribuição** — ambos os livros existem, mas a adequação ao tema é oposta (ver §4) |
| **Estrutura e tom** | 5 frases completas, vocabulário de auditoria/controle externo | 5 frases completas, vocabulário de MCS (unidades de responsabilidade, médio prazo, eficiente/eficaz) | **Redação** — variação de ênfase e léxico, esperada entre execuções |
| **Extensão** | ~78 palavras | ~82 palavras | **Redação** — equivalente, cumpre "cinco linhas" |

### O que permaneceu igual

- Cumprimento formal do pedido: 5 linhas, 1 definição + 1 contextualização pública + 1 lista de componentes + 1 delimitação + 1 referência.
- Tom assertivo e estrutura paralela.
- Nenhuma variação vem com aviso de incerteza (comportamento previsto no slide 7 — "não sabe que não sabe").

### O que mudou — e por que importa

Toda a variação substantiva é **de fato, não de redação**. Não é sinônimo trocado ou ordem diferente; é conceito, tipologia e bibliografia diferentes. Isso corresponde exatamente ao alerta do roteiro `roteiro-modulo3.md:46`: "variação de redação não é o problema; variação de fato é. O exercício serve para separar as duas."

Em teste com o mesmo prompt, o modelo produziu duas conceituações mutuamente incompatíveis do mesmo termo técnico — uma o define como controle de conformidade *ex post* e outra como processo gerencial de implementação estratégica. Um estudante que copiasse sem conferir entregaria, a cada execução, um trabalho diferente e, em um dos casos, conceitualmente errado.

---

## 4. Julgamento — qual está mais correta e por quê

**Variação 2 está mais correta, com margem clara.**

Justificativa em 3 critérios verificáveis:

1. **Aderência à literatura de referência.** A definição de V2 reproduz literalmente a tradição Anthony (1965) → Anthony & Govindarajan (2007): controle gerencial = processo de influenciar membros da organização para implementar a estratégia. É a definição ensinada nos manuais de MCS e cobrada em provas da área. V1 não encontra respaldo nessa literatura.

2. **Tipologia.** V2 distingue controle gerencial de controle operacional (foco em tarefas, curto prazo, eficiência de execução) e de controle estratégico (ambiente, longo prazo). V1 faz o inverso: afirma que o controle gerencial "tem caráter predominantemente operacional", o que contradiz a tipologia padrão (Anthony; Merchant & Van der Stede; Simons). Conferível em qualquer manual de controle gerencial, cap. 1.

3. **Autor citado.** `ANTHONY & GOVINDARAJAN, Management Control Systems, 12. ed., McGraw-Hill/Irwin, 2007` existe, é a edição vigente à data e é referência canônica para o tema — título, editora, ano e coautoria conferem (ver WorldCat / doi.org). `CHIAVENATO, Administração Geral e Pública, 3. ed., Elsevier, 2014` também existe, mas é manual generalista, não obra de referência em controle gerencial; citá-lo para sustentar definição de MCS é atribuição trocada (erro tipo 3 do slide 15). O DOI não se aplica a livro, mas a existência da obra é verificável em catálogo da editora.

V1 não é "totalmente falsa" — descreve corretamente *controle interno/externo* e conformidade com LRF — mas **responde ao termo errado**. Em avaliação de Administração, V1 seria corrigida como confusão entre controle gerencial (management control) e controle administrativo/externo (compliance/controle da legalidade).

**Placar:** V2 = confirmada nos 4 pontos centrais; V1 = plausível na forma, incorreta no conteúdo central.

---

## 5. Implicação para uso em trabalho aplicado — em uma linha

**Variação de redação é tolerável, variação de fato não é: toda definição, tipologia ou referência gerada por IA precisa ser conferida na fonte primária (manual/capítulo/artigo) antes de entrar em trabalho avaliado, sob pena de entregar conceito trocado com aparência de correto.**

Extensão prática: usar a IA para rascunho é válido (ciclo 3.3 — papel, contexto, instrução, formato), mas a entrega final deve citar a fonte que *você* abriu e leu — Google Acadêmico com título entre aspas, doi.org para DOI, ou o próprio livro — conforme slide 17 "Onde se confere cada tipo de afirmação"; autorizar o "NÃO SEI" no prompt reduz, mas não elimina, essa conferência obrigatória.

---

## 6. Registro de verificação

- Variação 2 verificada: título `Management Control Systems` + autores + 12. ed. + 2007 + McGraw-Hill/Irwin — confere no catálogo WorldCat e na ficha da editora.
- Variação 1 verificada: `CHIAVENATO` 3. ed. 2014 existe como manual geral; inadequado como fonte primária de MCS — ver sumário da obra (capítulos de funções administrativas, não de MCS).
- Instrução e procedimento de comparação conforme `roteiro-modulo3.md:42-47` e `modulo3-ia-e-engenharia-de-prompt.html:509-585` (ciclos 3.1 e critério de correção: "Resposta que aponta apenas diferenças de redação, sem julgar correção, vale metade").

---
*Gerado em 15/09/2026 — comparação das duas execuções em `saida/teste-variacao-*.md`.*
