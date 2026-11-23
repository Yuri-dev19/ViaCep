# 📮 ViaCep: Consulta de CEP

Aplicação web em **Angular** que busca o endereço completo a partir de um CEP, usando a API pública [ViaCEP](https://viacep.com.br/).

![Demonstração do projeto](./docs/screenshot.png)

🔗 **Demo:** [link do deploy]

## ✨ Funcionalidades

- Busca de endereço por CEP (8 números)
- Validação do campo com Reactive Forms (obrigatório e exatamente 8 dígitos)
- Estado de carregamento durante a consulta
- Mensagens de erro claras: CEP inválido, CEP não encontrado e falha na API
- Exibição de CEP, rua, bairro, cidade e UF

## 🛠️ Tecnologias

- Angular 21 (componentes standalone, Signals e a nova sintaxe de controle de fluxo `@if`)
- TypeScript
- RxJS e `HttpClient`
- Reactive Forms
- HTML e CSS

## 📁 Estrutura

```
src/app/
├── models/
│   └── cep.ts          # interface Cep (formato da resposta da API)
├── services/
│   └── cep.ts          # CepService: consulta a API do ViaCEP via HttpClient
├── app.ts              # componente principal (formulário e estados da tela)
├── app.html            # template
└── app.config.ts       # configuração da aplicação (provideHttpClient)
```

## ▶️ Como rodar

Pré-requisitos: [Node.js](https://nodejs.org/) e npm.

```bash
git clone https://github.com/Yuri-dev19/ViaCep.git
cd ViaCep
npm install
npm start
```

Depois, abra `http://localhost:4200` no navegador.

## 🧪 Testes e build

```bash
npm test        # testes unitários
npm run build   # build de produção
```

## 👤 Autor

**Yuri Machado**: [LinkedIn](https://www.linkedin.com/in/yuri-machado-tech/) · [GitHub](https://github.com/Yuri-dev19)
