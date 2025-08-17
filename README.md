# Banco API Tests

## 🎯 Objetivo
Este projeto tem como objetivo automatizar testes para a API REST do projeto [Banco API](https://github.com/juliodelimas/banco-api).  
A automação contribui a validação de seus endpoints e funcionalidades, facilitando a detecção de falhas e a manutenção contínua.

## 🛠️ Stack Utilizada
- **Linguagem**: JavaScript (Node.js)
- **Framework de Testes**: [Mocha](https://mochajs.org/)
- **Biblioteca de Asserções**: [Chai](https://www.chaijs.com/)
- **Cliente HTTP para Testes**: [Supertest](https://github.com/visionmedia/supertest)
- **Relatórios de Teste**: [Mochawesome](https://github.com/adamgruber/mochawesome)
- **Gerenciamento de Dependências**:dotenv

## 📂 Estrutura de Diretórios
```
.
├── test/                  # Contém os arquivos de testes automatizados
│   └── exemplo.test.js    # Exemplo de teste automatizado
├── mochawesome-report/    # Relatórios HTML gerados automaticamente
├── package.json           # Lista de dependências e scripts do projeto
└── .env                   # Arquivo de variáveis de ambiente (não incluído no repositório)
```

## ⚙️ Formato do Arquivo `.env`
Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:
```env
BASE_URL=http://localhost:3000
```
> ⚠️ **Importante:** Ajuste o valor de `BASE_URL` para o endereço da API que deseja testar.

## 🚀 Execução dos Testes
Instale as dependências do projeto:
```bash
npm install
```

Execute os testes automatizados:
```bash
npm test
```

Gerar relatório em HTML com Mochawesome:
```bash
npx mocha test --reporter mochawesome
```

O relatório será gerado no diretório `mochawesome-report`.

## 📚 Documentação das Dependências
- [Mocha](https://mochajs.org/)
- [Chai](https://www.chaijs.com/)
- [Supertest](https://github.com/visionmedia/supertest)
- [Mochawesome](https://github.com/adamgruber/mochawesome)
