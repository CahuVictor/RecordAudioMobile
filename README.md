# 🎙️ RecordAudioMobile

**RecordAudioMobile** é uma aplicação web leve e responsiva, criada para dispositivos móveis, que permite gravar áudios diretamente no navegador sem necessidade de instalar nenhum aplicativo externo.

## ✅ Funcionalidades

- Gravação de áudio utilizando o microfone do dispositivo
- Geração automática de nomes de arquivos com timestamp + identificações personalizadas
- Leitura de arquivo `.txt` com 3 linhas de identificação (ex: nome, turma, atividade)
- Armazenamento das informações no `localStorage` para reaproveitamento entre sessões
- Interface adaptada para uso em celulares
- Download local do áudio gravado no formato `.webm`
- Envio da gravação via e-mail com corpo e assunto preenchidos
- Compatível com instalação como PWA (Progressive Web App)
- Funciona offline após o primeiro acesso (via Service Worker)

## 🚀 Como usar

1. Abra a página `index.html` no navegador (ou publique via GitHub Pages / Vercel)
2. Envie um arquivo `.txt` com 3 linhas contendo as informações identificadoras
3. Inicie e pare a gravação normalmente
4. Baixe o áudio gerado com nome automático
5. Opcionalmente, envie por e-mail com um clique

## 📁 Estrutura do projeto

```
RecordAudioMobile/
├── index.html
├── manifest.json
├── service-worker.js
├── assets/
│   └── icons/
│       ├── icon-192.png
│       └── icon-512.png
└── README.md
```

## 📱 PWA (Progressive Web App)

Este projeto pode ser instalado como aplicativo no Android/iOS:

- Android/Chrome: Clique em "Adicionar à Tela Inicial"
- iOS/Safari: Use o botão "Compartilhar" e selecione "Adicionar à Tela de Início"

## 🧪 Tecnologias utilizadas

- HTML5, CSS3, JavaScript
- MediaRecorder API
- localStorage
- Service Worker
- Manifest Web App
- mailto:

## ⚠️ Limitações

- A gravação será interrompida se você sair da aba ou trocar de aplicativo (limitação dos navegadores)
- O envio por e-mail não anexa automaticamente o áudio (o link é incluído no corpo da mensagem)

## 📄 Licença

Este projeto está licenciado sob a licença MIT.
