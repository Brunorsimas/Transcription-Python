# Transcription-Python

Assistente de voz multi-idiomas desenvolvido em Python que combina tecnologias de reconhecimento de fala, processamento de linguagem natural e síntese de voz.

## 🎯 Funcionalidades

- **Gravação de Áudio**: Captura de voz do usuário através do navegador
- **Transcrição com Whisper**: Reconhecimento de fala usando OpenAI Whisper
- **Processamento com Gemini**: Geração de respostas usando Google Gemini 2.5 Flash
- **Síntese de Voz**: Conversão de texto em fala com gTTS
- **Suporte Multi-idiomas**: Configurável para diferentes idiomas

## 🛠️ Tecnologias Utilizadas

- **OpenAI Whisper**: Transcrição de áudio para texto
- **Google Gemini 2.5 Flash**: Processamento de linguagem natural
- **gTTS (Google Text-to-Speech)**: Síntese de voz
- **Python**: Linguagem principal
- **JavaScript**: Gravação de áudio no navegador

## 📋 Pré-requisitos

- Python 3.7+
- Conta Google Cloud com API Gemini ativada
- Navegador web com suporte a MediaStream Recording API

## 🚀 Instalação

1. Clone o repositório:
```bash
git clone https://github.com/Brunorsimas/Transcription-Python.git
cd Transcription-Python
```

2. Instale as dependências:
```bash
pip install openai-whisper gtts google-generativeai
```

## ⚙️ Configuração

1. Obtenha sua API Key do Google Gemini:
   - Acesse [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Crie uma nova API Key
   - Copie a chave gerada

2. Configure a API Key no código:
   - Substitua `'AIzaSyCqeiQdU5dT5dSJUNjE92N9AqDit98_oMU'` pela sua chave
   - Ou defina como variável de ambiente: `export GOOGLE_API_KEY=sua_chave`

## 📖 Como Usar

O projeto foi originalmente desenvolvido para Google Colab e consiste em um fluxo completo:

1. **Gravação**: O sistema grava áudio do usuário através do navegador
2. **Transcrição**: Whisper converte o áudio em texto
3. **Processamento**: Gemini analisa o texto e gera uma resposta
4. **Síntese**: gTTS converte a resposta em áudio

### Para uso local:

Modifique o arquivo para adaptar às necessidades locais, removendo dependências do Google Colab e ajustando os caminhos dos arquivos.

## 📁 Estrutura do Projeto

```
Transcription-Python/
├── cópia_de_assistente_de_voz_multi_idiomas_com_whisper_e_chatgpt.py
└── README.md
```

## 🔧 Variáveis Configuráveis

- `language`: Idioma para transcrição e síntese (padrão: 'pt')
- `record_file`: Caminho do arquivo de áudio de entrada
- `response_audio`: Caminho do arquivo de áudio de saída

## 📝 Notas

- O código atual contém referências ao Google Colab que precisam ser adaptadas para uso local
- A gravação de áudio utiliza JavaScript e funciona melhor em ambiente de notebook
- O modelo Whisper "small" oferece bom equilíbrio entre velocidade e precisão

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## 📄 Licença

Este projeto está sob licença MIT.