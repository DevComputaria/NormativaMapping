# Normativa Mapping - IN BCB nº 589/2025

Este repositório contém a estrutura semântica e representação formal da **Instrução Normativa BCB nº 589, de 4 de fevereiro de 2025**, que divulga a versão 7.1 dos *Requisitos Mínimos para a Experiência do Usuário* no contexto do Pix, incluindo o **Pix Automático**.

O projeto visa representar regras de negócio e conceitos descritos na normativa utilizando padrões da Web Semântica: **SBVR**, **OWL**, **RDF**, **SKOS** e **SHACL**.

---

## 📁 Estrutura do Projeto

```
normativa-mapping/
├── docs/                          # Documentos originais e referências
├── ontology/                      # Ontologias OWL e vocabulário SKOS
├── rules/                         # Regras de negócio em SBVR e OWL
├── validation/                    # Shapes SHACL para validação
├── data-samples/                  # Exemplos de dados RDF
├── queries/                       # Consultas SPARQL
├── scripts/                       # Scripts de automação e transformação
├── outputs/                       # Logs e relatórios de conformidade
└── README.md                      # Documentação do projeto
```

---

## 🔍 Objetivos

- Modelar conceitos do Pix e Pix Automático como ontologias OWL.
- Representar regras da IN 589/2025 em SBVR e OWL.
- Criar vocabulários SKOS para termos técnicos.
- Validar dados RDF com SHACL.
- Permitir consultas SPARQL sobre conformidade e estrutura.

---

## 🧩 Tecnologias Utilizadas

- [OWL](https://www.w3.org/OWL/)
- [RDF](https://www.w3.org/RDF/)
- [SKOS](https://www.w3.org/TR/skos-reference/)
- [SHACL](https://www.w3.org/TR/shacl/)
- [SBVR (OMG)](https://www.omg.org/spec/SBVR/)
- [Protégé](https://protege.stanford.edu/) para edição de ontologias
- [PySHACL](https://github.com/RDFLib/pySHACL) para validação

---

## 🚀 Como começar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/normativa-mapping.git
   cd normativa-mapping
   ```

2. Abra os arquivos `.ttl` no Protégé para explorar a ontologia.

3. Use o PySHACL para validar os dados de exemplo:
   ```bash
   pyshacl -s validation/bcb/pix-shapes.ttl -d data-samples/bcb/exemplo-transacao-pix.ttl
   ```

---

## 📌 Próximos Passos

- Expandir regras do Pix Automático
- Adicionar exemplos reais de conformidade
- Integrar com motor de inferência e análise temporal
- Exportar dados em JSON-LD para APIs de compliance

---

## 🧠 Autores

Desenvolvido por especialistas em Ontologias, RegTech e Web Semântica.

---

## 📄 Licença

Este projeto está licenciado sob os termos da [Licença MIT](LICENSE).
