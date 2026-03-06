# Sistema de Perguntas e Respostas com RAG e LLM

Este projeto implementa um **sistema de perguntas e respostas baseado em Retrieval-Augmented Generation (RAG)** utilizando modelos de linguagem e embeddings para recuperar informações relevantes e gerar respostas contextualizadas.

O objetivo é demonstrar como integrar **modelos de linguagem, embeddings e recuperação de documentos** para construir aplicações inteligentes capazes de responder perguntas a partir de uma base de conhecimento.

---

## Arquitetura do Projeto

O sistema segue o padrão **RAG (Retrieval-Augmented Generation)**:

1. **Indexação de Documentos**
   - Os documentos são processados e convertidos em **vetores de embeddings**.

2. **Busca Semântica**
   - A pergunta do usuário é transformada em embedding.
   - O sistema busca os **documentos mais relevantes**.

3. **Geração de Resposta**
   - O contexto recuperado é enviado para o **modelo de linguagem (LLM)**.
   - O modelo gera a resposta baseada nas informações encontradas.

---

## Tecnologias Utilizadas

- Python
- Transformers
- Sentence Transformers
- PyTorch
- FAISS / Busca Vetorial
- Hugging Face Models
- Jupyter Notebook

---

## Modelo de Embeddings

O projeto utiliza o modelo:

```
sentence-transformers/all-mpnet-base-v2
```

Este modelo é responsável por converter textos em **vetores semânticos**, permitindo busca contextual e recuperação de informações relevantes.

---

## Estrutura do Projeto

```
projeto-rag/
│
├── Projeto3.ipynb        # Notebook com implementação do pipeline RAG
├── README.md             # Documentação do projeto
└── requirements.txt      # Dependências do projeto
```

---

## Como Executar o Projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/projeto-rag.git
cd projeto-rag
```

### 2. Instalar as dependências

```bash
pip install -r requirements.txt
```

### 3. Executar o Notebook

Abra o **Jupyter Notebook** ou **Google Colab** e execute:

```
Projeto3.ipynb
```

---

## Exemplo de Uso

Pergunta enviada ao sistema:

```
What is Schistosomiasis?
```

O pipeline executa:

1. Conversão da pergunta em embedding  
2. Busca de contexto relevante  
3. Geração de resposta usando LLM  

---

## Objetivo do Projeto

Este projeto foi desenvolvido como parte de estudos em **Inteligência Artificial Generativa e Engenharia de Dados**, demonstrando na prática:

- Implementação de RAG
- Uso de LLMs
- Busca semântica com embeddings
- Construção de pipelines de IA

---
