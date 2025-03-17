# Exploring Tools for Flaky Test Detection, Correction, and Mitigation: A Systematic Mapping Study

**MARTINS, Pedro Anderson Costa; ALVES, Victor Anthony; LIMA, Iraneide; BEZERRA, Carla; MACHADO, Ivan.** "Exploring Tools for Flaky Test Detection, Correction, and Mitigation: A Systematic Mapping Study." SBES’24, September 30 – October 04, 2024, Curitiba, PR.

## 1. Fichamento de Conteúdo

O artigo realiza um mapeamento sistemático de ferramentas para detecção, correção e mitigação de testes flaky (não determinísticos) em testes automatizados. Os autores identificaram 30 ferramentas a partir de 37 estudos, analisando suas características, técnicas e abordagens. O estudo destaca que 70% das ferramentas são voltadas para a linguagem Java, com foco em dependência de ordem de execução (46% das ferramentas). A técnica mais comum é a reexecução de testes, utilizada por 83% das ferramentas. O artigo também discute desafios como a complexidade de identificar testes flaky e a necessidade de abordagens preventivas. A taxonomia proposta ajuda pesquisadores e profissionais a escolher ferramentas adequadas para seus contextos específicos.

## 2. Fichamento Bibliográfico

- **Testes Flaky:** Testes que podem passar ou falhar ao serem executados no mesmo código, sem alterações (p. 1).
- **Reexecução de Testes:** Técnica de executar testes múltiplas vezes para identificar inconsistências (p. 4).
- **Dependência de Ordem:** Quando o resultado de um teste depende da ordem de execução de outros testes (p. 2).
- **Cobertura Diferencial:** Técnica que analisa mudanças na cobertura de código entre versões para detectar testes flaky (p. 5).
- **Aprendizado de Máquina:** Uso de modelos de aprendizado de máquina para prever testes flaky com base em características estáticas e dinâmicas (p. 5).

### Sistemas, Ferramentas e Bibliotecas Mencionadas
- **DeFlaker:** Ferramenta que utiliza cobertura diferencial para detectar testes flaky.
- **FlakeFlagger:** Ferramenta que usa aprendizado de máquina para prever testes flaky sem reexecução.
- **NonDex:** Ferramenta que explora comportamentos não determinísticos em APIs para detectar testes flaky.
- **iDFlakies:** Framework para detectar e classificar testes flaky dependentes de ordem.
- **Shaker:** Ferramenta que introduz tarefas de estresse para revelar testes flaky causados por concorrência.

### Teorias e Métodos Aplicados
- **Mapeamento Sistemático:** Metodologia para identificar, avaliar e sintetizar estudos relevantes sobre um tema específico.
- **Técnicas de Detecção de Testes Flaky:** Incluem reexecução de testes, cobertura diferencial e aprendizado de máquina.
- **Análise de Causas de Testes Flaky:** Identificação de causas como espera assíncrona, concorrência e dependência de ordem.

## 3. Fichamento de Citações

- "A técnica de reexecução de testes é predominante para a detecção, mitigação e reparo de testes flaky, destacando que a maioria das ferramentas busca identificar testes inconsistentes que falham intermitentemente." (p. 7)
- "Ferramentas como Shaker e NonDex abordam especificamente problemas relacionados à espera assíncrona, concorrência e dependência de implementação." (p. 6)
- "A taxonomia proposta ajuda pesquisadores e profissionais a selecionar ferramentas adequadas com base em suas necessidades específicas, facilitando a tomada de decisão no gerenciamento de testes flaky." (p. 8)
- "O estudo identificou que 70% das ferramentas analisadas são voltadas para a linguagem Java, com suporte predominante para frameworks como JUnit e Maven." (p. 8)
- "A dependência de ordem é uma causa significativa de testes flaky, influenciando o foco das ferramentas desenvolvidas nesse contexto." (p. 8)
- "O uso de técnicas preventivas, como o aprendizado de máquina, pode reduzir a incidência de testes flaky desde o início do desenvolvimento." (p. 7)

---

**Data do fichamento:** 12/03/2025  
**Autor do fichamento:** Gabriel Augusto