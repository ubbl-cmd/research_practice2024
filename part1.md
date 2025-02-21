# Задание 1

## Статья
Название: SMORE: Knowledge Graph Completion and Multi-hop Reasoning in Massive Knowledge Graphs

Для цитирования: Ren H. et al. Smore: Knowledge graph completion and multi-hop reasoning in massive knowledge graphs //Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining. – 2022. – С. 1472-1482.

URL: [https://dl.acm.org/doi/10.1145/3534678.3539405](https://dl.acm.org/doi/10.1145/3534678.3539405)

## Поставленная цель и задачи

Целью исследования является разработка и представление SMORE - первой общей платформы для одно- и многошагового логического вывода на базе знаний. Авторы стремились создать инструмент, способный масштабироваться на крупные графы знаний и служить основой для будущих исследований в области многопутевого логического вывода на масштабах крупных графов.
> В статье была явно сформулирована цель исследования: "Develop SMORE - the first general framework for both single- and multi-hop logical reasoning that scales up to large knowledge graphs and provides algorithm-system co-optimization for scalability."

Для достижения поставленной цели перед авторами возникают следующие задачи:

- Разработка алгоритмно-системной платформы для логического вывода:
`"In this paper, we present SMORE, the first general framework for both single- and multi-hop reasoning that scales up to large knowledge graphs and provides algorithm-system co-optimization for scalability." (Introduction)`
> В разделе "Introduction" представлена общая постановка проблемы и необходимость разработки платформы для логического вывода на графах знаний.
- Оптимизация алгоритмов и системной архитектуры для обеспечения масштабируемости:
`"As shown in Figure 2, the computation plan of a query consists of nodes V𝑞 ∪ {𝑉1, . . . , 𝑉𝑘 , 𝑉?}." (Computation Plan of a Query)`
> Раздел "Computation Plan of a Query" описывает план вычислений для обработки запросов, учитывая масштаб графа знаний и сложность операций.
- Разработка и реализация алгоритмов для эффективного выполнения логического вывода:
`"Embedding-based reasoning methods avoid explicit KG traversal." (Embedding-based 'traversal' of the KG)" Our SMORE covers three published works, i.e., GQE [7], Q2B [19] and BetaE [ 20 ]." (Multi-hop reasoning models and neural logical operators)`
> Раздел "Embedding-based 'traversal' of the KG" представляет методы встроенного логического вывода на основе эмбеддингов.
> Раздел "Multi-hop reasoning models and neural logical operators" описывает модели GQE, Q2B и BetaE для логического вывода в эмбеддинговом пространстве.
- Оптимизация процесса выполнения запросов для повышения эффективности и масштабируемости:
`"We propose to solve the above optimization problem in Eqn (2) with dynamic programming (DP)." (Dynamic programming for optimal node cut) "Sharing negative samples." (Further optimization of SMORE) "Figure 10 shows the speed-up of bidirectional rejection sampler over exhaustive samplers on several more query structures." (Additional results on bidirectional rejection sampler)`
> В разделе "Dynamic programming for optimal node cut" представлено использование динамического программирования для оптимизации выполнения запросов.
> Разделы "Further optimization of SMORE" и "Additional results on bidirectional rejection sampler" описывают дополнительные методы оптимизации и результаты экспериментов, направленные на улучшение эффективности SMORE.

## Тематика статьи
Тематика статьи принадлежит области искусственного интеллекта и обработки знаний. Это подтверждается разработкой платформы для логического вывода на графах знаний с использованием методов встроенных логических операций и эмбеддингов.

## Методы обоснования

Авторы используют различные методы для обоснования результатов и выводов:

- Эмпирические эксперименты:
`"Figure 10 shows the speed-up of bidirectional rejection sampler over exhaustive samplers on several more query structures." (Additional results on bidirectional rejection sampler)`
> Авторы провели эксперименты для сравнения производительности различных методов логического вывода на различных запросах и структурах данных. Эти эксперименты были направлены на демонстрацию эффективности и масштабируемости предложенной платформы SMORE.
> Результаты экспериментов, такие как скорость выполнения запросов, точность ответов и использование ресурсов, были использованы для обоснования преимуществ предложенного подхода по сравнению с существующими методами.

- Анализ сложности алгоритмов:
`"After solving the above DP, we can construct the node cut from solution 𝑜 (·) in a top-down direction." (Dynamic programming for optimal node cut)`
> В разделе "Dynamic programming for optimal node cut" авторы провели анализ сложности алгоритма динамического программирования, применяемого для оптимизации выполнения запросов. Этот анализ помогал понять, как алгоритм работает и обосновать его применимость для оптимизации выполнения запросов на графах знаний.