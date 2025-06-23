# Laboratório de Azure AI Search: Indexação Inteligente de Documentos

## 📖 Descrição
Este projeto, desenvolvido para o bootcamp "XP Inc. - Cloud com Inteligência Artificial" da DIO, demonstra a implementação de uma solução de pesquisa inteligente utilizando o **Azure AI Search**. O objetivo foi ingerir um conjunto de documentos não estruturados, enriquecê-los com habilidades de Inteligência Artificial e disponibilizá-los através de um índice pesquisável.

## ⚙️ Ferramentas e Tecnologias Utilizadas
- **Azure AI Search:** Orquestração do fluxo de indexação e pesquisa.
- **Azure Blob Storage:** Armazenamento dos documentos de origem.
- **Azure AI Services:** Fornecimento das habilidades cognitivas (OCR, extração de entidades, etc.).
- **GitHub:** Para versionamento e documentação do projeto.
- **Markdown:** Para a criação deste README.

---

## 🚀 Etapas do Laboratório

### 1. Configuração do Ambiente no Azure
Para iniciar o projeto, foram provisionados os seguintes recursos no portal do Azure:
1.  **Conta de Armazenamento (Storage Account):** Para hospedar os arquivos base do laboratório.
2.  **Serviço de IA do Azure (Azure AI Services):** Para habilitar as funcionalidades de enriquecimento.
3.  **Serviço do Azure AI Search:** O serviço central para a criação do índice.

*(📸 Adicione aqui um screenshot mostrando os recursos criados no seu grupo de recursos do Azure. Ex: `![Recursos no Azure](images/01-recursos-azure.png)`)*

### 2. Ingestão de Dados e Enriquecimento com IA
O processo de ingestão foi realizado utilizando o assistente "Importar dados" do Azure AI Search. Os principais passos foram:

- **Conexão com a Fonte de Dados:** Conectado ao contêiner de Blob Storage onde os documentos foram previamente carregados.
- **Configuração do "Skillset" (Habilidades de IA):** Foi configurado um conjunto de habilidades para enriquecer os dados durante a indexação. As habilidades aplicadas foram:
  - **Habilitar OCR e mesclar todo o texto:** Para extrair texto de arquivos PDF e imagens.
  - **Extrair nomes de pessoas, organizações e locais.**
  - **Detectar idioma.**
  - **Extrair frases-chave.**

*(📸 Adicione aqui um screenshot da sua configuração de habilidades de IA. Ex: `![Configuração do Skillset](images/03-config-habilidades-ia.png)`)*

### 3. Exploração e Consulta do Índice
Com o índice populado, utilizei a ferramenta "Search Explorer" para validar a solução. As consultas demonstraram a eficácia do enriquecimento de IA:

- **Busca por palavra-chave:** Uma busca simples retornou os documentos relevantes.
- **Busca por entidade:** Foi possível buscar por nomes de organizações extraídos pela IA, que não seriam pesquisáveis em uma busca tradicional.

*(📸 Adicione aqui um screenshot mostrando um exemplo de busca bem-sucedida no Search Explorer. Ex: `![Resultado da Busca](images/05-resultado-busca-simples.png)`)*

---

## 💡 Conclusão
Este laboratório foi uma excelente demonstração prática do poder do Azure AI Search para transformar dados não estruturados em conhecimento acionável. A capacidade de enriquecer documentos com IA e criar um índice inteligente abre um leque de possibilidades para aplicações corporativas, como sistemas de gestão de conhecimento, análise de contratos e muito mais. A principal dificuldade encontrada foi [descreva um desafio, se houver] e o principal aprendizado foi [descreva o que mais te marcou].

## 👨‍💻 Autor
**[Seu Nome]**
- [Seu LinkedIn](https.linkedin.com/in/seu-usuario)
- [Seu Perfil da DIO](https://www.dio.me/users/seu-usuario)
