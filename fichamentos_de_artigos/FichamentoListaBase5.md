# Detecting False Alarms from Automatic Static Analysis Tools: How Far are We?

**Referência completa:**  
Kang, Hong Jin; Aw, Khai Loong; Lo, David. "Detecting False Alarms from Automatic Static Analysis Tools: How Far are We?" In *44th International Conference on Software Engineering (ICSE ’22)*, May 21–29, 2022, Pittsburgh, PA, USA. ACM, New York, NY, USA, 12 pages. https://doi.org/10.1145/3510003.3510214

---

## 1. Fichamento de Conteúdo

O artigo aborda o problema das altas taxas de falsos positivos gerados por ferramentas de análise estática automática (ASATs), como o FindBugs, que são amplamente utilizadas para detectar bugs em código Java. Apesar de serem úteis, essas ferramentas geram muitos alertas que não são relevantes, o que dificulta sua adoção pelos desenvolvedores. Para mitigar esse problema, pesquisas anteriores propuseram o uso de técnicas de aprendizado de máquina para classificar os alertas como "acionáveis" (que os desenvolvedores corrigiriam) ou "falsos alarmes". Estudos anteriores identificaram um conjunto de "Golden Features" que, quando usados em modelos de aprendizado de máquina, alcançaram desempenho quase perfeito. No entanto, este artigo revela que esses resultados podem ser superestimados devido a problemas como vazamento de dados e duplicação de dados nos experimentos. O estudo analisa esses problemas e mostra que, quando corrigidos, o desempenho dos modelos cai significativamente. Além disso, o artigo questiona a robustez do "closed-warning heuristic", um método usado para rotular os alertas como acionáveis ou falsos alarmes, mostrando que ele não é consistente e pode gerar rótulos que não concordam com a avaliação humana. O artigo conclui que ainda há muito espaço para melhorias na detecção de alertas acionáveis e sugere a necessidade de um benchmark mais confiável e a comparação com baselines simples.

---

## 2. Fichamento Bibliográfico

1. **Golden Features**: Conjunto de 23 características identificadas como as mais importantes para detectar alertas acionáveis em ferramentas de análise estática. Essas características incluem métricas como a proporção de alertas acionáveis em um arquivo, histórico de alterações no código e características do próprio alerta (página 2).

2. **Closed-warning heuristic**: Método heurístico usado para determinar se um alerta é acionável ou um falso alarme. Ele compara se um alerta presente em uma revisão do código ainda aparece em uma revisão futura (referência). Se o alerta não aparecer na revisão futura, ele é considerado acionável; caso contrário, é considerado um falso alarme (página 2).

3. **Vazamento de dados (Data Leakage)**: Ocorre quando informações do conjunto de teste são inadvertidamente usadas no treinamento do modelo, levando a resultados superestimados. No artigo, isso acontece porque as "Golden Features" usam informações da revisão futura para calcular métricas, o que não seria possível em um cenário real (página 4).

4. **Duplicação de dados (Data Duplication)**: Problema em que os mesmos alertas aparecem tanto no conjunto de treinamento quanto no conjunto de teste, o que infla artificialmente o desempenho do modelo. O artigo mostra que a remoção desses dados duplicados reduz significativamente a precisão do modelo (página 6).

5. **AUC (Area Under the Curve)**: Métrica usada para avaliar a capacidade de um modelo de distinguir entre alertas acionáveis e falsos alarmes. Um valor de AUC próximo a 1 indica um bom desempenho, enquanto um valor próximo a 0.5 indica que o modelo não é melhor que um chute aleatório (página 4).

6. **LIME (Local Interpretable Model-agnostic Explanations)**: Ferramenta usada para explicar as previsões de modelos de aprendizado de máquina, identificando quais características contribuíram mais para uma previsão específica. No artigo, o LIME foi usado para entender por que as "Golden Features" funcionam bem (página 4).

---

## 3. Fichamento de Citações

1. "The large number of false alarms produced poses a barrier to adoption. Researchers have proposed the use of machine learning to prune false alarms and present only actionable warnings to developers." (página 1).

2. "We found that several studies used an experimental procedure that results in data leakage and data duplication, which are subtle issues with significant implications." (página 1).

3. "The closed-warning heuristic produces labels that do not agree with human oracles. Hence, the strong performance of these techniques previously seen is overoptimistic of their true performance if adopted in practice." (página 2).

4. "Our results show that the use of the Golden Features do not substantially outperform a strawman baseline that predicts all warnings are actionable." (página 2).

5. "Only 47% of closed warnings were labelled actionable by human annotators, implying that many closed warnings are not actionable." (página 8).

6. "Our study highlights the need for deeper study of the warning oracle to determine ground-truth labels. By changing the reference revision, different conclusions about performance of the Golden Features can be reached." (página 11).
