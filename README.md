
# OPTES — Ontologia do Portal da Transparência do ES

A **OPTES** é uma ontologia desenvolvida no âmbito do projeto *Melhoria da Maturidade das Bases de Dados Abertos do Portal da Transparência do Poder Executivo Estadual* (NEMO/UFES). Seu objetivo é promover a interoperabilidade semântica, a integração e a reutilização dos dados governamentais abertos do Estado do Espírito Santo segundo os princípios de **Linked Open Data**.

## Resultados Produzidos

Construída a partir do método **SABiOx** (*Extended Systematic Approach for Building Ontologies*), a ontologia é estruturada de forma modular em três subdomínios principais:

1. **Núcleo (`nucleo`):** O subdomínio nucleo reúne requisitos relacionados a conceitos que podem ser compartilhados por diferentes conjuntos de dados do Portal da Transparência..
2. **Receitas (`base-receitas`):** O subdomínio base-receitas visa estabelecer os conceitos centrais necessárias para compreender o que é uma receita pública e como conceitos relacionados estão envolvidos, especialmente as Unidades Gestoras..
3. **Despesas (`base-despesas`):** O subdomínio base-despesas visa estabelecer os conceitos centrais necessárias para compreender o que é uma despesa pública, quais são seus subtipos e como conceitos relacionados estão envolvidos.

Como artefatos principais, o repositório entrega:
* **Ontologia de Referência:** Modelos conceituais fundamentados na **UFO** (*Unified Foundational Ontology*), especificados na linguagem **OntoUML** por meio da sintaxe textual **Tonto**.
* **Ontologia Operacional (T-Box):** Implementação computacional em **OWL**, utilizando o vocabulário **gUFO** e serializada em **Turtle (`.ttl`)**, acompanhada de documentação navegável em HTML.
* **Dados Transformados (A-Box):** Instâncias em formato **RDF/Turtle** geradas a partir da transformação semântica dos conjuntos de dados abertos (com recorte piloto no exercício financeiro de 2025).
* **Documentação Metodológica e Técnica:** Relatórios completos de especificação de requisitos (questões de competência), ontologia de referência, ontologia operacional e entrega de resultados.



### Descrição dos Diretórios

* **`docs/`**: Contém os arquivos estáticos utilizados pelo GitHub Pages para disponibilizar a documentação navegável da ontologia, bem como os arquivos `.ttl` correspondentes à ontologia operacional (T-Box) gerados em OWL/gUFO.


* **`documentacaoOntologia/`**: Reúne os documentos em PDF que formalizam o desenvolvimento da ontologia:
  * **`sabiox/`**: Artefatos das etapas do método SABiOx — Especificação da Ontologia (requisitos funcionais e não funcionais), Ontologia de Referência (modelos, axiomas e dicionários) e Ontologia Operacional (regras de codificação e arquitetura).

  * **`metodo/`**: Documentos de síntese metodológica, entrega de resultados e orientações de integração e reúso.



* **`tonto/`**: Armazena o código-fonte da ontologia de referência escrito em Tonto, organizado modularmente entre o pacote compartilhado (`nucleo/`) e os pacotes específicos de domínio (`bases/receitas/` e `bases/despesas/`).


* **`ontologiaDados/`**: Destinado aos arquivos RDF serializados em Turtle (`.ttl`) resultantes do mapeamento e transformação dos dados abertos do Portal da Transparência (A-Box).

