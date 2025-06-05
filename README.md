# 💼 Board de Contas Automatizado

Sistema pessoal para controle automatizado de contas, focado em centralizar boletos recebidos por e-mail e organizá-los visualmente em um painel inteligente com notificações, uploads de comprovantes e categorização.

## 🎯 Objetivo

Evitar perda de prazos e facilitar o controle de pagamentos e comprovantes de forma automatizada, com uma interface organizada e funcional.

## 👥 Público-alvo

- Pessoas físicas ou MEIs que recebem contas por e-mail, portais ou informalmente
- Quem busca controle centralizado e automatizado de vencimentos e pagamentos

## ⚙️ Funcionalidades Principais

- 📥 **Leitura automática de e-mails (Gmail API)**
- 📎 **Download e organização de boletos (PDF)**
- 🧾 **Extração automática de valor e vencimento**
- 🧩 **Painel visual em React com filtros e status**
- ➕ **Adição manual de contas (ex: dívidas pessoais)**
- 📁 **Upload de comprovantes por conta**
- 🔔 **Notificações por WhatsApp sobre vencimentos**
- 🏷️ **Categorização e controle por status e data**

## 🚀 Tecnologias

| Camada | Tecnologia |
|--------|------------|
| Front-end | React.js + TailwindCSS |
| Back-end | FastAPI (Python) |
| Automação | Gmail API, pdfplumber |
| Banco | PostgreSQL |
| Notificações | Twilio API (WhatsApp) |
| Armazenamento | Firebase ou local |
| Deploy | Vercel (frontend) + Render/Railway (API) |

## 🗃️ Estrutura esperada

**Tabela: `contas`**
- id, descricao, valor, vencimento, categoria, status, origem, comprovante_url, user_id, created_at

**Tabela: `usuarios`**
- id, nome, email, senha (hash), whatsapp

## 📊 Painel

- Cards com: nome, valor, vencimento, status, categoria, comprovante
- Filtros por status, categoria e mês
- Upload de comprovante diretamente no card
- Controle por mês e relatório simples

## ✅ Roadmap

- [x] Definir escopo geral
- [x] Criar board no Trello (desenvolvimento)
- [ ] Script: Gmail → PDF
- [ ] Extração de dados do boleto
- [ ] Adição manual de conta
- [ ] Interface React: cards e filtros
- [ ] Upload de comprovante
- [ ] Notificações por WhatsApp
- [ ] Deploy do sistema

## 👨‍💻 Autor

Kauã Vicente Domingos — [LinkedIn](https://www.linkedin.com/in/kaua676) | [GitHub](https://github.com/Kaua676)

