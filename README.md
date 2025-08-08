# 👋 Olá! Eu sou o Marco (@marcozmz) - Desenvolvedor Back-end

[![IFSP Badge](https://img.shields.io/badge/Análise_e_Desenvolvimento_de_Sistemas-IFSP_Araraquara-blue?logo=bookstack&style=for-the-badge)](https://www.ifsp.edu.br/)
[![Monitoria](https://img.shields.io/badge/Monitor-IFSP_Araraquara-green?style=for-the-badge&logo=graduation-cap)](https://www.ifsp.edu.br/)

## 🚀 Sobre Mim

Estudante de **Análise e Desenvolvimento de Sistemas** no IFSP - Araraquara e Técnico em Informática formado. Apaixonado por arquitetura back-end e soluções de automação inteligente.

## 🌟 Projeto em Destaque: Sistema de Autenticação e Gerenciamento de Pedidos

[![Node.js](https://img.shields.io/badge/Node.js-14.x+-339933?logo=nodedotjs&style=flat-square)](https://nodejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.x+-007ACC?logo=typescript&style=flat-square)](https://www.typescriptlang.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.x+-4479A1?logo=mysql&style=flat-square)](https://www.mysql.com/)
[![RabbitMQ](https://img.shields.io/badge/RabbitMQ-3.x+-FF6600?logo=rabbitmq&style=flat-square)](https://www.rabbitmq.com/)

### 📌 Visão Geral
Sistema completo com:
- **Autenticação JWT** segura
- **Recuperação de senha** via e-mail
- **Dashboard** de gerenciamento
- **Processamento assíncrono** com RabbitMQ
- **API documentada** com Swagger

🔗 **[Acesse o Repositório](https://github.com/marcozmz/Sistema-de-Autentica-o-e-Gerenciamento-de-Pedidos-ts-node)**

### 🛠️ Principais Funcionalidades

| Módulo | Tecnologias | Features |
|--------|------------|----------|
| **🔐 Autenticação** | JWT, Bcrypt | Registro, Login, Recuperação de senha |
| **📦 Pedidos** | RabbitMQ, MySQL | CRUD completo, Processamento assíncrono |
| **📊 Dashboard** | HTML5, CSS3, JS | Visualização em tempo real |

### 🚀 Como Executar

```bash
# Clone o repositório
git clone https://github.com/marcozmz/Sistema-de-Autentica-o-e-Gerenciamento-de-Pedidos-ts-node.git

# Instale as dependências
npm install

# Configure o .env
cp .env.example .env

# Inicie o servidor
npm run dev
```

## 🛠️ Tecnologias que Domino

<div align="center">
  
**Back-end**  
[![Node.js](https://img.shields.io/badge/Node.js-Expert-339933?logo=nodedotjs&style=for-the-badge)](https://nodejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Advanced-007ACC?logo=typescript&style=for-the-badge)](https://www.typescriptlang.org/)
[![Express](https://img.shields.io/badge/Express.js-Pro-000000?logo=express&style=for-the-badge)](https://expressjs.com/)

**Banco de Dados**  
[![MySQL](https://img.shields.io/badge/MySQL-Expert-4479A1?logo=mysql&style=for-the-badge)](https://www.mysql.com/)
[![SQLite](https://img.shields.io/badge/SQLite-Advanced-003B57?logo=sqlite&style=for-the-badge)](https://www.sqlite.org/)

**Automação**  
[![n8n](https://img.shields.io/badge/n8n-Intermediate-4B63EA?logo=data:image/png;base64,...&style=for-the-badge)](https://n8n.io/)
</div>

## 📌 Outros Projetos

- **🔑 [Gerador de Senhas e QR Code](https://github.com/marcozmz/gerador-de-senhas-e-qrcode-Nodejs)**  
  Aplicação Node.js para gerar credenciais seguras

- **📦 [Gerenciador de Almoxarifado](https://github.com/marcozmz/Gerenciador-de-Almoxarifado---Node.js)**  
  Sistema completo para controle de estoque

## 📞 Contato

[![LinkedIn](https://img.shields.io/badge/Conecte--se_no_LinkedIn-0077B5?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/marcoazanchettamontagna/)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&style=for-the-badge)](mailto:mamontagna100@gmail.com)

---

⭐ **Destaque do Projeto**: Sistema implementa arquitetura modular com:
- Middlewares de autenticação
- Filas RabbitMQ para processamento assíncrono
- Validação de dados com Zod
- Documentação Swagger automática

```typescript
// Exemplo de código do projeto
import { authenticate } from './middlewares/auth';
import { createOrderQueue } from './queues/orderQueue';

app.post('/orders', authenticate, async (req, res) => {
  await createOrderQueue.add({ ...req.body });
  res.status(202).json({ message: 'Pedido em processamento' });
});
```
