# 🍽️ FIAP Kitchenet

Aplicativo mobile de pedidos para a cantina da FIAP, desenvolvido como projeto avaliativo da disciplina de **Mobile Development with IoT** — turma MDI.

---

## 📋 Sobre o Projeto

O **FIAP Kitchenet** permite que alunos realizem pedidos de lanches, bebidas e doces diretamente pelo celular, acompanhem seus pedidos no perfil e retirem no balcão usando um código gerado automaticamente.

---

## ✅ Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| Login | Autenticação com RM e senha (simulado) |
| Cardápio | Visualização de itens por categoria com carrinho |
| Finalizar Pedido | Modal com resumo e opções de pagamento (PIX, Crédito, Débito) |
| Histórico | Seção "Perfil" com todos os pedidos realizados |
| Retirada | Código de 4 dígitos gerado para retirada no balcão |

---

## 🛠️ Tecnologias Utilizadas

- [React Native](https://reactnative.dev/) `0.83.2`
- [Expo](https://expo.dev/) `~55.0.8`
- [Expo Router](https://expo.github.io/router/) `~55.0.7` — navegação por abas
- [@expo/vector-icons](https://icons.expo.fyi/) — ícones da interface
- JavaScript (ES6+)

---

## 📁 Estrutura do Projeto

```
fiap-mdi-cp1-FIAP-Kitchenet/
├── app/
│   ├── _layout.js      # Configuração das abas de navegação
│   ├── index.js        # Tela de Login
│   ├── pedir.js        # Cardápio, Carrinho e Modal de Pagamento
│   ├── perfil.js       # Perfil do usuário e histórico de pedidos
│   ├── retirada.js     # Código de retirada do pedido
│   ├── auth.js         # Controle de autenticação
│   └── pedidos.js      # Armazenamento compartilhado de pedidos
├── assets/             # Ícones e imagens do app
├── app.json            # Configuração do Expo
└── package.json        # Dependências do projeto
```

---

## 🚀 Como Executar

### Pré-requisitos

- [Node.js](https://nodejs.org/) instalado
- Aplicativo **Expo Go** no celular ([Android](https://play.google.com/store/apps/details?id=host.exp.exponent) / [iOS](https://apps.apple.com/app/expo-go/id982107779))
- Ou um emulador Android/iOS configurado

### Passo a passo

**1. Clone o repositório**
```bash
git clone https://github.com/fernmoraes/fiap-mdi-cp1-FIAP-Kitchenet.git
cd fiap-mdi-cp1-FIAP-Kitchenet
```

**2. Instale as dependências**
```bash
npm install --legacy-peer-deps
```

> A flag `--legacy-peer-deps` é necessária devido a conflitos de versão entre dependências internas do Expo SDK 55.

**3. Inicie o servidor de desenvolvimento**
```bash
npx expo start
```

**4. Abra o aplicativo**

- **Celular físico:** Escaneie o QR Code com o app Expo Go
- **Emulador Android:** Pressione `a` no terminal
- **Emulador iOS:** Pressione `i` no terminal
- **Navegador:** Pressione `w` no terminal

### Credenciais de teste

O login é simulado — qualquer RM e senha preenchidos permitem o acesso.

---

## 👥 Equipe e Contribuições

| Integrante | Branch | Contribuição |
|---|---|---|
| Fernando Moraes | `master` | Estrutura base, Login, Cardápio e Carrinho |
| Weslley | `Weslley` | Seção "Finalizar Pedido" com modal de pagamento |
| Guilherme | `Guilherme` | Integração dos pedidos com a seção "Perfil" |
| Bruna | `Bruna` | Seção "Retirada" com código do pedido |
| Gabriel | `Gabriel` | Documentação |

---

## 📚 Contexto Acadêmico

> Projeto desenvolvido para o **Checkpoint 1** da disciplina de Mobile Development with IoT — FIAP, 2025.
