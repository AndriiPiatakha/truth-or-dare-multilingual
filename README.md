# 🎉 Multilingual Truth or Dare FREE API – Global Fun Game for Any Occasion

Bring your app, game, or chatbot to life with endless, original Truth or Dare questions — **customized by vibe, audience, and language**. Perfect for date nights, parties with friends, or fun ice-breakers anywhere in the world.

<p align="center">
  🆓 <b>FREE API</b> — use instantly on 
  <a href="https://rapidapi.com/vintarok-vintarok-default/api/multilingual-truth-or-dare-party-date-game-api" target="_blank"><b>RapidAPI</b></a> 🚀
</p>

<p align="center">
  <a href="https://rapidapi.com/vintarok-vintarok-default/api/multilingual-truth-or-dare-party-date-game-api">
    <img src="logo.png" width="120" alt="Truth or Dare API Logo">
  </a>
</p>
---

## 🌍 Why Choose This API?

### 💬 Multilingual by Design
Generate truths and dares in **100+ languages** — from English, Spanish, and French to Russian, Korean, or Arabic. No manual translation needed. Just pass the `lang` parameter (full language name) and get localized fun instantly.

### 🧠 AI-Powered Originality
Each response is generated dynamically by a powerful language model, ensuring **unique**, natural, and context-appropriate prompts — never repeated, never boring.

### 🧩 Flexible Customization
Set the context, mood, or theme using the `notes` field (up to 200 characters):
- Add **inside jokes** or **custom scenarios** for personal flavor.
- Guide tone and style (e.g., “family-safe”, “flirty”, or “wild party”).

### ❤️ Multiple Relationship or Social Modes
Adapt the experience for any audience:
- **Date mode:** sweet or daring prompts for couples (`game=date`)
- **Party mode:** fun, silly, or bold challenges for groups (`game=party`)

Within each game type, select a stage or vibe:
- **Party:** `chill`, `party`, `wild`
- **Date:** `new`, `steady`, `forever`

### ⚙️ Simple to Use
Just one API call — no sign-up, no setup. Works perfectly for:
- Mobile or web games
- Chatbots or Discord bots
- Dating apps or friendship apps
- Ice-breaker widgets and event tools

---

## 🚀 Example Request

```bash
GET https://api.it-bulls.com/truth-or-dare/v1/truth-or-dare.php?game=party&mode=dare&stage=chill&notes=family%20gathering%20safe%20content&lang=Spanish
```

### Parameters
| Name | Type | Description |
|------|------|-------------|
| `game` | string | `party` or `date` — type of experience |
| `mode` | string | `truth` or `dare` |
| `stage` | string | Context level: `chill`, `party`, `wild` (party) or `new`, `steady`, `forever` (date) |
| `notes` | string | Optional personal or contextual hints (≤200 chars) |
| `lang` | string | Full language name (e.g., `English`, `Spanish`, `Russian`) |

### Example Response
```json
{
  "ok": true,
  "text": "Tell us about the funniest thing that ever happened during a family dinner!"
}
```

---

## 💎 Highlights
- 🌍 Works in 100+ languages
- 🧠 AI ensures every prompt is original
- 💬 Customizable with personal notes or themes
- 💕 Separate logic for date and party modes
- ⚡ Instant JSON responses, easy to integrate
- 🔒 Safe, moderated output

---

## 📚 Use Cases
- Party or drinking game apps
- Romantic couple games
- Friendship or travel social apps
- Chatbots with interactive challenges
- Ice-breaker web widgets for events

---

# 📘 API Documentation – Multilingual Truth or Dare

Easily integrate **Truth or Dare generation** into your app, game, or chatbot. This API produces dynamic, language-aware prompts for friends, couples, or party groups.


---

## 🔸 Endpoint
**GET /truth-or-dare.php** – Generate a new Truth or Dare prompt

### Description
Creates one AI-generated Truth or Dare prompt, customized by language, context, and type of game (party or date).

---

## 🧾 Query Parameters

| Name | Type | Required | Default | Description |
|------|------|-----------|----------|--------------|
| `mode` | string | ✅ Yes | — | What to generate: `truth` or `dare`. |
| `game` | string | No | `party` | Game context: `party` for friends, `date` for couples. |
| `stage` | string | No | `chill` (party) / `new` (date) | Vibe or relationship stage.<br>**Party:** `chill`, `party`, `wild`.<br>**Date:** `new`, `steady`, `forever`. |
| `notes` | string | No | — | Optional short personal context (≤200 chars). Example: “family friendly” or “funny only”. |
| `lang` | string | No | `English` | Output language. Full name, ≤20 chars. Example: `Spanish`, `Russian`, `German`. |

---

## 💡 Example Request
```bash
GET /truth-or-dare.php?game=party&mode=dare&stage=chill&notes=family%20gathering%20safe%20content&lang=Spanish
```

---

## ✅ Example Success Response
```json
{
  "ok": true,
  "text": "Describe the funniest moment from your first trip together."
}
```

---

## ⚠️ Error Responses

| Code | Example | Description |
|------|----------|-------------|
| 400 | `{ "ok": false, "error": "Missing parameter: mode" }` | Required parameter missing or invalid. |
| 403 | `{ "ok": false, "error": "Forbidden: invalid proxy secret" }` | Invalid or missing RapidAPI security header. |
| 429 | `{ "ok": false, "error": "Daily quota reached" }` | Free usage limit exceeded. |
| 500 | `{ "ok": false, "error": "Server error" }` | Unexpected internal issue. |

---

## 🧠 Notes
- All responses include the keys `ok` and `text` (or `error` on failure).
- Prompts are AI-generated and filtered through moderation for safe content.
- Each call produces an original question or challenge — never reused.

---

## 🧩 Example Use Cases
- Chatbots & conversation starters
- Dating and couple apps
- Party and drinking games
- Ice-breaker tools
- Multilingual learning or cultural games

---

## 🏷️ Category
**Entertainment** – Games, Fun, and Social Interaction.




## 🧩 Example Ideas
- **Dating App:** Ask playful questions to spark chemistry
- **Party Game:** Generate wild dares in multiple languages
- **Friendship Bot:** Keep things light with chill truth prompts
