# Gerador de Modelos Inteligentes com IA 🤖📄

Um aplicativo web desenvolvido em Python que utiliza Inteligência Artificial Generativa para automatizar a criação e o preenchimento de documentos e contratos.

O sistema recebe múltiplos documentos semelhantes (PDF ou Word), compara o conteúdo, identifica padrões e gera um **Documento Modelo (Template)** padronizado. A partir desse modelo, o usuário pode preencher as variáveis através de um formulário dinâmico na própria interface e baixar o documento final pronto para uso.

## 🚀 Funcionalidades

*   **Processamento Multi-formato:** Leitura e extração de texto em arquivos `.pdf` e `.docx`.
*   **Comparação Inteligente (IA):** Integração com o modelo Gemini 1.5 Flash para cruzar dados de múltiplos documentos e identificar textos fixos e variáveis.
*   **Geração Dinâmica de Formulários:** Detecção automática de variáveis (ex: `[CNPJ]`, `[NOME]`) utilizando Expressões Regulares (Regex) para criar campos de preenchimento na interface.
*   **Geração de Word (.docx):** Criação de arquivos Word estruturados e formatados com fonte Arial, tamanho 11 pt, prontos para download.
*   **Duas vias de exportação:** O usuário pode baixar o Template em branco com as tags, ou preencher os dados no app e baixar o arquivo final.

## 🛠️ Tecnologias Utilizadas

*   **[Python 3](https://www.python.org/):** Linguagem base do projeto.
*   **[Streamlit](https://streamlit.io/):** Criação da interface web (Frontend).
*   **[Google Generative AI](https://aistudio.google.com/):** Comunicação com a API do Gemini.
*   **PyPDF2 & python-docx:** Bibliotecas para manipulação e leitura de arquivos.
*   **python-dotenv:** Gerenciamento seguro de variáveis de ambiente.

## ⚙️ Como Executar o Projeto

**1. Clone o repositório:**
```bash
git clone [https://github.com/Michelbvp/gerador-documentos.git](https://github.com/Michelbvp/gerador-documentos.git)
cd gerador-documentos
