# Observability in Microservices Architectures: Leveraging Logging, Metrics, and Distributed Tracing in Large-Scale Systems

**Madupati, Bhanuprakash.** "Observability in Microservices Architectures: Leveraging Logging, Metrics, and Distributed Tracing in Large-Scale Systems," in *European Journal of Advances in Engineering and Technology*, vol. 10, no. 11, pp. 24-31, 2023.

## 1. Fichamento de Conteúdo

O artigo aborda a importância da observabilidade em sistemas baseados em microsserviços, destacando os desafios de monitoramento e depuração em ambientes distribuídos de grande escala. O autor explora os três pilares da observabilidade: logging (registros de eventos), métricas (indicadores de desempenho) e rastreamento distribuído (monitoramento de fluxos de requisições entre serviços).  

Ferramentas como **Prometheus**, **Grafana** e **Jaeger** são apresentadas como soluções essenciais para coleta de métricas, visualização de dados e rastreamento de requisições, respectivamente.  

O artigo também discute os desafios comuns, como o **volume excessivo de dados**, a **complexidade de instrumentação** e os **custos associados à manutenção de uma plataforma de observabilidade centralizada**.  

Como práticas recomendadas, o autor sugere:
- **Otimização da coleta e retenção de dados**  
- **Padronização da instrumentação**  
- **Uso eficaz de alertas e dashboards**  
- **Automação de processos**  

Conclui-se que a observabilidade é crucial para a confiabilidade e desempenho de sistemas de microsserviços, e que a integração de ferramentas como **Prometheus, Grafana e Jaeger** pode melhorar significativamente a capacidade de monitoramento e depuração.  

---

## 2. Fichamento Bibliográfico

- **Observabilidade:** Conceito que engloba **logging, métricas e rastreamento distribuído**, essencial para monitorar e depurar sistemas de microsserviços (p. 24).  

- **Logging:** Registros detalhados de eventos gerados por microsserviços, utilizados para depuração e diagnóstico. Em grande escala, é recomendado o uso de **logging estruturado e centralizado**, como o **ELK Stack (Elasticsearch, Logstash, Kibana)** (p. 25).  

- **Métricas:** Indicadores numéricos que descrevem o comportamento dos microsserviços, como uso de **CPU e memória**.  
  - **Prometheus** é a ferramenta mais utilizada para coleta de métricas.  
  - **Grafana** é usado para visualização (p. 25-26).  

- **Rastreamento Distribuído:** Técnica que monitora o fluxo de requisições entre microsserviços, identificando **gargalos e falhas**.  
  - **Jaeger** é uma ferramenta popular para rastreamento distribuído (p. 26-27).  

- **Desafios:** Volume alto de dados, complexidade de instrumentação, manutenção de uma plataforma centralizada e gerenciamento de custos são os principais obstáculos para a observabilidade em microsserviços (p. 29).  

---

## 3. Fichamento de Citações

> "Observability is a crucial aspect of understanding how microservices-based systems are running healthily" (p. 29).  

> "Prometheus is an open-source monitoring and alerting system used mostly when microservices architecture comes along to collect metrics in this distributed space" (p. 27).  

> "Grafana enhances the features of Prometheus by offering advanced visualization tools, allowing developers to build high-level overview dashboards for real-time understanding of system status" (p. 27).  

> "Jaeger provides visibility into how requests flow through different services, helping engineers get an overall picture of service-cross communication for performance tracking and failure analysis" (p. 26).  

> "The three major aspects of observability regarding microservices architectures are Logging, Metrics, and Distributed Tracing" (p. 24).  

> "Best practices for observability include optimizing data collection and retention, ensuring consistent instrumentation, and securing observability data" (p. 30).  
