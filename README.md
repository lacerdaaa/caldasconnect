# 🚛 Rastreamento de Caminhões - Next.js + AWS + WebSockets

## 📌 Sobre o Projeto
Este projeto é um sistema de rastreamento de caminhões em tempo real, desenvolvido com **Next.js**, utilizando **AWS** para infraestrutura e **WebSockets** para conexão em tempo real. O objetivo é permitir a monitoria da localização dos caminhões em um painel dinâmico.

## 🛠️ Tecnologias Utilizadas
- **Next.js** - Framework React para aplicações web
- **AWS Lambda** - Para processamento serverless
- **AWS API Gateway** - Para gestão das conexões WebSocket
- **AWS DynamoDB** - Para armazenamento de localização em tempo real
- **AWS IoT Core** - Para gerenciamento dos dispositivos conectados
- **WebSockets** - Para comunicação em tempo real entre frontend e backend
- **Mapbox / Google Maps API** - Para renderização do mapa

## 🚀 Como Executar o Projeto
### 🔧 Requisitos
- Node.js instalado (versão 16+ recomendada)
- Conta AWS configurada com permissões adequadas
- Chave de API para Mapbox ou Google Maps

### 🏗️ Instalação
1. Clone o repositório:
   ```sh
   git clone https://github.com/lacerdaaa/caldasconnect.git
   ```
2. Acesse o diretório do projeto:
   ```sh
   cd caldasconnect
   ```
3. Instale as dependências:
   ```sh
   npm install
   # ou
   yarn install
   ```
4. Configure as variáveis de ambiente:
   Crie um arquivo `.env.local` e adicione:
   ```env
   NEXT_PUBLIC_MAP_API_KEY=SUACHAVE
   AWS_REGION=us-east-1
   AWS_IOT_ENDPOINT=wss://xxxxx.iot.us-east-1.amazonaws.com/mqtt
   ```
5. Inicie o projeto em modo de desenvolvimento:
   ```sh
   npm run dev
   # ou
   yarn dev
   ```
6. Acesse no navegador:
   ```
   http://localhost:3000
   ```

## 📡 Estrutura do Projeto
```
├── components/       # Componentes reutilizáveis do Next.js
├── pages/            # Páginas principais da aplicação
├── services/         # Serviços para comunicação com AWS e WebSockets
├── utils/            # Funções auxiliares
├── public/           # Arquivos estáticos
├── styles/           # Estilização do projeto
└── .env.local        # Configuração de variáveis sensíveis
```

## 📡 Fluxo de Comunicação
1. O cliente (Next.js) se conecta ao **AWS API Gateway WebSocket**.
2. O backend (AWS Lambda) recebe e processa os eventos de localização.
3. As coordenadas dos caminhões são armazenadas no **DynamoDB**.
4. O frontend escuta as atualizações e exibe os caminhões no mapa.

## 📌 Funcionalidades
✅ Rastreamento em tempo real via WebSockets
✅ Mapa interativo para visualização da frota
✅ Integração com AWS para escalabilidade
✅ Interface responsiva com Next.js
✅ Suporte para vários dispositivos

## 🤝 Contribuição
Fique à vontade para contribuir! Basta seguir os passos:
1. Fork este repositório
2. Crie um branch com sua funcionalidade: `git checkout -b minha-feature`
3. Commit suas alterações: `git commit -m 'Adicionando funcionalidade X'`
4. Envie para o branch principal: `git push origin minha-feature`
5. Abra um Pull Request 🚀

---

Desenvolvido por [Lacerda](https://github.com/lacerdaaa) 🚀

# 🚛 Rastreamento de Caminhões - Next.js + AWS + WebSockets

## 📌 Sobre o Projeto
Este projeto é um sistema de rastreamento de caminhões em tempo real, desenvolvido com **Next.js**, utilizando **AWS** para infraestrutura e **WebSockets** para conexão em tempo real. O objetivo é permitir a monitoria da localização dos caminhões em um painel dinâmico.

## 🛠️ Tecnologias Utilizadas
- **Next.js** - Framework React para aplicações web
- **AWS Lambda** - Para processamento serverless
- **AWS API Gateway** - Para gestão das conexões WebSocket
- **AWS DynamoDB** - Para armazenamento de localização em tempo real
- **AWS IoT Core** - Para gerenciamento dos dispositivos conectados
- **WebSockets** - Para comunicação em tempo real entre frontend e backend
- **Mapbox / Google Maps API** - Para renderização do mapa

## 🚀 Como Executar o Projeto
### 🔧 Requisitos
- Node.js instalado (versão 16+ recomendada)
- Conta AWS configurada com permissões adequadas
- Chave de API para Mapbox ou Google Maps

### 🏗️ Instalação
1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/rastreamento-caminhoes.git
   ```
2. Acesse o diretório do projeto:
   ```sh
   cd rastreamento-caminhoes
   ```
3. Instale as dependências:
   ```sh
   npm install
   # ou
   yarn install
   ```
4. Configure as variáveis de ambiente:
   Crie um arquivo `.env.local` e adicione:
   ```env
   NEXT_PUBLIC_MAP_API_KEY=SUACHAVE
   AWS_REGION=us-east-1
   AWS_IOT_ENDPOINT=wss://xxxxx.iot.us-east-1.amazonaws.com/mqtt
   ```
5. Inicie o projeto em modo de desenvolvimento:
   ```sh
   npm run dev
   # ou
   yarn dev
   ```
6. Acesse no navegador:
   ```
   http://localhost:3000 ( verifique a possibilidade da porta estar sendo usada )
   ```

## 📡 Estrutura do Projeto
```
src/
└───├── components/       # Componentes reutilizáveis do Next.js
    ├── pages/            # Páginas principais da aplicação
    ├── services/         # Serviços para comunicação com AWS e WebSockets
    ├── utils/            # Funções auxiliares
    ├── public/           # Arquivos estáticos
    ├── styles/           # Estilização do projeto
    └── .env.local        # Configuração de variáveis sensíveis
```

## 📡 Fluxo de Comunicação
1. O cliente (Next.js) se conecta ao **AWS API Gateway WebSocket**.
2. O backend (AWS Lambda) recebe e processa os eventos de localização.
3. As coordenadas dos caminhões são armazenadas no **DynamoDB**.
4. O frontend escuta as atualizações e exibe os caminhões no mapa.

## 📌 Funcionalidades
✅ Rastreamento em tempo real via WebSockets
✅ Mapa interativo para visualização da frota
✅ Integração com AWS para escalabilidade
✅ Interface responsiva com Next.js
✅ Suporte para vários dispositivos

## 🤝 Contribuição
Para a contribuição da equipe, siga os passos abaixo:
1. Fork este repositório
2. Crie um branch com sua funcionalidade: `git checkout -b minha-feature`
3. Commit suas alterações: `git commit -m 'Adicionando funcionalidade X'`
4. Envie para o branch principal: `git push origin minha-feature`
5. Abra um Pull Request 🚀

## 📜 Licença
Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

Desenvolvido por [Lacerda](https://github.com/lacerdaaa) 🚀

