# Calculadora IMC - React + Vite

Uma calculadora de Índice de Massa Corporal (IMC) desenvolvida com React e Vite, migrada do projeto original em HTML/CSS/JavaScript vanilla.

## 🚀 Funcionalidades

- **Cálculo de IMC**: Interface intuitiva para inserir altura e peso
- **Classificação Automática**: Tabela com faixas de classificação do IMC
- **Integração com API**: Requisições para API local (com fallback para cálculo local)
- **Design Responsivo**: Layout adaptável para mobile e desktop
- **Validação de Campos**: Validação em tempo real dos inputs
- **Tratamento de Erros**: Mensagens de erro claras e informativas
- **Loading States**: Indicadores visuais durante processamento

## 🛠️ Tecnologias Utilizadas

- **React 18** - Biblioteca para interface de usuário
- **Vite** - Build tool e servidor de desenvolvimento
- **Axios** - Cliente HTTP para requisições
- **CSS Modules** - Estilização modular
- **Custom Hooks** - Lógica de estado reutilizável

## 📁 Estrutura do Projeto

```
src/
├── components/
│   ├── CalculatorForm/          # Formulário de entrada
│   ├── IMCTable/               # Tabela de classificação
│   └── Layout/                 # Container principal
├── services/
│   └── imcService.js           # Serviços de API
├── hooks/
│   └── useIMC.js              # Hook customizado para IMC
├── utils/
│   └── imcUtils.js            # Utilitários e validações
├── styles/
│   └── globals.css            # Estilos globais
└── App.jsx                    # Componente principal
```

## 🚀 Como Executar

### Pré-requisitos
- Node.js (versão 16 ou superior)
- npm ou yarn

### Instalação
```bash
# Instalar dependências
npm install

# Executar em modo de desenvolvimento
npm run dev

# Build para produção
npm run build

# Preview do build de produção
npm run preview
```

### API Local (Opcional)
Para usar a API local, certifique-se de que o servidor esteja rodando em `http://localhost:3000`. Se a API não estiver disponível, o sistema automaticamente usará o cálculo local.

## 🎯 Como Usar

1. Acesse a aplicação no navegador
2. Insira sua altura em metros (ex: 1.75)
3. Insira seu peso em quilogramas (ex: 70)
4. Clique em "Calcular IMC"
5. Veja o resultado destacado na tabela de classificação

## 📱 Responsividade

A aplicação é totalmente responsiva e se adapta a diferentes tamanhos de tela:
- **Mobile** (até 768px): Layout compacto com elementos empilhados
- **Desktop** (acima de 768px): Layout centralizado com melhor espaçamento

## 🔧 Configuração

### Variáveis de Ambiente
Crie um arquivo `.env` na raiz do projeto para configurar a URL da API:

```env
VITE_API_URL=http://localhost:3000
```

### Proxy de Desenvolvimento
O Vite está configurado para fazer proxy das requisições `/api` para `http://localhost:3000`.

## 🧪 Testes

```bash
# Executar testes (quando implementados)
npm run test

# Executar testes com coverage
npm run test:coverage
```

## 📦 Build e Deploy

### Build de Produção
```bash
npm run build
```

Os arquivos otimizados serão gerados na pasta `dist/`.

### Deploy
A aplicação pode ser facilmente deployada em plataformas como:
- **Vercel**: `vercel --prod`
- **Netlify**: Conecte o repositório Git
- **GitHub Pages**: Use o GitHub Actions

## 🔄 Migração do Projeto Original

Este projeto foi migrado do projeto original em HTML/CSS/JavaScript vanilla, mantendo todas as funcionalidades e melhorando a experiência do usuário com:

- **Componentização**: Código mais organizado e reutilizável
- **Estado Gerenciado**: Uso de hooks para gerenciamento de estado
- **Melhor UX**: Loading states, validação e tratamento de erros
- **Manutenibilidade**: Código mais fácil de manter e estender
- **Performance**: Otimizações do React e Vite

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## 🤝 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para:
1. Fazer fork do projeto
2. Criar uma branch para sua feature
3. Fazer commit das mudanças
4. Abrir um Pull Request
