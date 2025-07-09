# 🧪 banco-api-tests
# 🔍 Objetivo
Este projeto realiza testes automatizados na API REST do [banco-api](https://github.com/juliodelimas/banco-api), validando suas funcionalidades e contribuindo a qualidade de suas operações.

# 💻 Stack Tecnológica

Linguagem: JavaScript (Node.js)
Frameworks de testes: [Mocha](https://mochajs.org/)
Biblioteca de requisições HTTP: [Supertest](https://github.com/ladjs/supertest)
Biblioteca de asserções: [Chai](https://www.chaijs.com/)
Relatórios de testes: [Mochawesome](https://github.com/adamgruber/mochawesome)
Gerenciamento de variáveis de ambiente: [dotenv](https://github.com/motdotla/dotenv)

# 🗂️ Estrutura de diretórios
banco-api-tests/
├── test/                         # Testes organizados por funcionalidades
│   ├── login.test.js
│   └── tranferencias.test.js
├── mochawesome-report/           # Diretório gerado automaticamente com o relatório HTML dos testes
├── .env                          # Arquivo para configuração da variável BASE_URL
├── .gitignore
├── package.json
├── README.md

# Formato do arquivo .env

Antes de rodar os testes, crie um arquivo chamado .env na raiz do projeto com o seguinte conteúdo:

BASE_URL=http://localhost:3000

Substitua `http://localhost:3000` pela URL onde a API `banco-api` está rodando.

Onde:

BASE_URL deve apontar para o endpoint base da API banco-api (ajuste hostname e porta conforme seu ambiente).

Também é possível incluir outras variáveis caso seu projeto evolua, como tokens de autenticação ou parâmetros de timeout.

# 🚀 Comandos principais
Comando	Descrição
npm install	Instala todas as dependências do projeto
npm test	Executa todos os testes com relatório no console
npm run test:report	Executa testes e gera relatório HTML via mochawesome
Relatórios
Após npm run test:report, os arquivos estarão em mochawesome/mochawesome.html. Basta abrir no navegador para visualizar.

# 📚 Documentação das dependências
Mocha

Chai

Supertest

mochawesome

Consulte os links acima para aprofundar o uso, opções de configuração e melhores práticas.

# ✅ Como contribuir
Faça um fork do repositório

Crie uma branch: git checkout -b minha-feature

Faça as alterações e commit: git commit -m "Descrição da feature"

Envie para o seu fork: git push origin minha-feature

Abra um Pull Request descrevendo as mudanças

# 📄 Licença
Este projeto está sob a MIT License. Veja o arquivo LICENSE para detalhes.

# 🎯 Próximas melhorias sugeridas
Integração com CI/CD (GitHub Actions, Travis, etc.)

Cobertura de testes automatizada (com nyc / istanbul)

Testes de contrato e testes de performance (ex: Pact, Artillery)

Rotas autenticadas com simulação de tokens JWT

