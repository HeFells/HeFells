```markdown
# HeFells / HeFells

![GitHub repo size](https://img.shields.io/github/repo-size/HeFells/HeFells)
![GitHub stars](https://img.shields.io/github/stars/HeFells/HeFells?style=social)
![GitHub last commit](https://img.shields.io/github/last-commit/HeFells/HeFells)
![License](https://img.shields.io/badge/License-Apache%202.0-blue)

> **"API brasileira que roteia pergunta entre modelo, tudo na moral e sem firula."**

---

## 🧠 Resumo (pra quem tá com pressa)

Isso aqui é o **hub da HeFells** — uma API **gratuita**, **brasileira** e **efetuativa** que:

- Escolhe o modelo certo pra cada pergunta (FAST, SMART, ULTRA)
- Roda sozinha (Router Pro)
- Tem console ao vivo, métrica, log e chave `hfl_`
- É grátis, mas não é bagunça

Se tu é dev, curte IA ou só quer testar algo novo, **tu tá no lugar certo, parça**.

---

## 🚀 O que tem nesse repositório?

```

HeFells/
├── README.md            # isso aqui (gigante, útil e com zoeira)
├── docs/                # doc véia e boa (HTML + OpenAPI)
├── examples/            # código pra rodar (curl, Python, JS)
├── ui/                  # HeFellsCloud (console bonitinho)
└── LICENSE              # Apache 2.0 (sério, mas sem estresse)

```

📌 **Nota importante:** o código do backend (Router Pro, modelos, orquestração) **não tá aqui** — esse é o tesouro da HeFells. Aqui é a vitrine e a doc.

---

## ⚡ Modos de roteamento (o coração da parada)

| Modo | Gatilho | Modelo usado | Resumão |
|------|---------|--------------|---------|
| **FAST** | Pergunta curta (tipo "oi", "que horas são") | DeepSearch-v2-32b | Resposta rápida, modo econômico |
| **SMART** | Pergunta média (explicação, dúvida técnica) | Compound | O famoso "não muito, não pouco" |
| **ULTRA** | Pergunta longona (textão, código complexo) | Compound+DeepSearch+Kimi k2| Pega pesado, mas resolve |

O sistema detecta sozinho o tamanho da pergunta e escolhe o modo. VOCÊ não precisa fazer nada. **Mágica? Não. Router Pro V2.**

---

## 📦 Endpoint

```http
POST /v1/chat/completions
Authorization: Bearer sua_chave_hfl_
Content-Type: application/json
```

```json
{
  "messages": [
    { "role": "user", "content": "Opa, bão?🐧👍" }
  ]
}
```

---

🧪 Exemplo na prática

cURL

```bash
curl -X POST https://sherman-highland-variation-modify.trycloudflare.com/v1/chat/completions \
  -H "Authorization: Bearer hfl_xxxxxxxx" \
  -H "Content-Type: application/json" \
  -d '{"messages":[{"role":"user","content":"Quem é você?"}]}'
```

JavaScript (frontend puro)

```javascript
const res = await fetch("https://sherman-highland-variation-modify.trycloudflare.com/v1/chat/completions", {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
    "Authorization": "Bearer sua_chave_hfl_"
  },
  body: JSON.stringify({
    messages: [{ role: "user", content: "Fala ai, ThinkSearch!" }]
  })
});

const data = await res.json();
console.log(data.choices[0].message.content);
```

---

🎮 Console ao vivo (testa agora)

👉 https://sherman-highland-variation-modify.trycloudflare.com

· Gera sua chave hfl_
· Faz pergunta no modo que quiser
· Vê os logs, as métricas, a resposta na hora

Sério. Testa. É grátis e é rápido.

---

🧙 Sobre a HeFells (a história, pra quem gosta)

A HeFells não é uma empresa gigante com nome em inglês e time de marketing. O backend é fechado (tesouro nacional), mas a doc, UI e exemplos são abertos pra quem quiser aprender, usar ou só zuar junto.

---

📄 Licença

Este repositório (README, docs, exemplos, UI) está sob a Apache License 2.0.

Isso significa que tu pode:

· Copiar
· Modificar
· Usar comercialmente (se quiser)

Mas com responsabilidade: dê os créditos, não remove o aviso de copyright, e entende que não tem garantia (tá no "as is", né?).

O backend da API continua sendo serviço fechado e gratuito — sem planos de cobrar, mas também sem planos de abrir o código.

---

🤝 Contribuição (ou como ajudar)

Quer contribuir?

· Usa a API e dá feedback
· Abre issue com sugestão ou bug
· Compartilha com outros devs

Não precisa saber programar. Só precisa não ser cuzão.

---

🗿 Considerações finais

A HeFells não é:

· ❌ A próxima OpenAI
· ❌ Um modelo de 1 trilhão de parâmetros (mentira)
· ❌ Um projeto com fins lucrativos (por enquanto)

A HeFells é:

· ✅ Uma API honesta
· ✅ Feita por um brasileiro
· ✅ Gratuita
· ✅ Funcional
· ✅ Com zoeira, mas que funciona de verdade

---

🌐 Links úteis

O que é Link
Console ao vivo beacons.ai/hefells
GitHub do projeto github.com/HeFells/HeFells
Documentação HTML (em breve)
YouTube @HeFells (se criou)

---

Feito com café, código e falta de paciência pra burocracia.

🇧🇷 HeFells — porque IA de ponta não precisa ser cara, complicada ou em inglês.

```

# HeFellsCloud 🇧🇷

API brasileira que roteia perguntas entre modelos de forma inteligente e Efetuativa!🤓

## 🧠 Como funciona

| Modo | Gatilho | Modelo |
|------|---------|--------|
| FAST | Perguntas curtas |  Modelo com think📚
| SMART | Perguntas médias | Modelo Compound^^☃️
| ULTRA | Perguntas longas | 2 modelos Juntos!⚡

## 📦 Endpoint

```

POST /v1/chat/completions
Authorization: Bearer sua_chave_hfl_
```

## 🚀 Exemplo rápido

```
   try {
        const res = await fetch("https://sherman-highland-variation-modify.trycloudflare.com/v1/chat/completions", {
            method: "POST",
            headers: {
                "Content-Type": "application/json",
                "Authorization": "Bearer sua_api_hfl
            },
```

🌐 Console ao vivo

https://sherman-highland-variation-modify.trycloudflare.com — gere sua chave e teste Agora Mesmo!😉

📄 Responsabilidade

Use Com responsabilidade,  e aproveite ao Máximo!

---

🤖Feito pela HeFells Cloud — a Melhor API que Você vai achar grátis no mercado!🛰
