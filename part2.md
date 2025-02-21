# Задание 2

## Статья
Название: SMORE: Knowledge Graph Completion and Multi-hop Reasoning in Massive Knowledge Graphs

Для цитирования: Ren H. et al. Smore: Knowledge graph completion and multi-hop reasoning in massive knowledge graphs //Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining. – 2022. – С. 1472-1482.

URL: [https://dl.acm.org/doi/10.1145/3534678.3539405](https://dl.acm.org/doi/10.1145/3534678.3539405)

## Характеристика используемых данных

### Методы исследования и обработки данных

- В статье использовались графы знаний в качестве исходных данных для разработки и оценки алгоритмов логического вывода. Процесс использования этих данных был описан следующим образом:

`"SMORE is designed to be scalable to large-scale knowledge graphs, which allows us to use any standard benchmarks for graph-based reasoning tasks. We chose benchmarks designed for one-hop or multi-hop reasoning on the Freebase and Wikidata datasets, such as SimpleQuestions, ComplexWebQuestions, WebQSP, and PathQuestions." (Introduction)`

> Это подтверждает использование стандартных наборов данных для графов знаний, таких как Freebase и Wikidata, а также выбор конкретных наборов данных для проверки эффективности алгоритмов логического вывода, таких как SimpleQuestions (фактологические вопросы), ComplexWebQuestions (сложные вопросы, требующие рассуждений), WebQSP (вопросы, требующие одношаговых и многошаговых рассуждений), and PathQuestions (вопросы, требующие анализа путей в графе знаний).

- Процесс обработки данных включал в себя подготовку данных и выполнение логического вывода на основе разработанных алгоритмов:

`"To demonstrate the effectiveness and scalability of our proposed platform, we evaluate it on multiple benchmarks of graph-based reasoning tasks. In particular, we test SMORE on two datasets, namely, SimpleQuestions and PathQuestions." (Introduction)`

> Это указывает на то, что данные были предварительно подготовлены для оценки платформы SMORE на конкретных наборах данных для логического вывода.

### Правомерность выводов

> Правомерность выводов обеспечивается использованием стандартных наборов данных и общепринятых метрик оценки, эффективности алгоритмов логического вывода:

`"To evaluate the effectiveness and efficiency of SMORE, we compare it with state-of-the-art baselines and report both the accuracy and efficiency of different methods." (Introduction)`

> Это говорит о том, что результаты оценивались с использованием сравнения с существующими методами и оценки как точности, так и эффективности алгоритмов.

### Направления дальнейших исследований
В заключении авторы утверждают, что SMORE — это первая платформа, позволяющая выполнять многопереходные рассуждения на очень больших графах знаний, и она может служить эталоном для будущих исследований.

## Характеристика выводов

### Сравнение результата и цели/задачам статьи

Результаты статьи полностью соответствуют цели и задачам, поставленным во введении:

`"We present SMORE, the first general framework for both single- and multi-hop reasoning that scales up a plenty of different embedding methods with multi-GPU support to KGs with 86M nodes and 338M edges. It performs the algorithm-system co-optimization for scalability." (Conclusion)` 

> Это подтверждает, что разработанный в статье фреймворк SMORE полностью соответствует поставленным задачам и целям.

### Достигнутый результат

#### Чем является результат
Результатом является разработанный алгоритмно-системный фреймворк SMORE для логического вывода на графах знаний.
`"Here we evaluate SMORE on KG completion and multi-hop reasoning tasks on KGs using various query embeddings."`

#### Характер результата
Результат является прикладным, так как представляет собой инструмент для выполнения логического вывода на реальных графах знаний.
`"The task is to answer multi-hop complex logical queries on KGs using various query embeddings."`

#### Характеристики результата
Фреймворк SMORE обладает высокой эффективностью и масштабируемостью при выполнении логического вывода на графах знаний.
`"We first demonstrate the scalability of SMORE on query sampling, multi-gpu speedup, GPU utilization over the three large KGs where all existing implementations fail."`

#### Границы применимости результата и степень его универсальности
SMORE может применяться для широкого спектра задач логического вывода на графах знаний, но его применимость может быть ограничена сложностью и структурой конкретных графов знаний.
`"The KGs we use here are up to 1500× larger than those considered by prior work."`

#### Технические ограничения полученного результата
Возможны ограничения производительности при работе с крупными и сложными графами знаний, а также технические сложности при интеграции с другими системами и платформами.
`"Various prior large-scale KG embedding systems consider graph partitioning. However, since our system focuses on complex queries, with graph partitioning, a large number of queries will thus span multiple partitions."`

#### Недостатки полученного решения
Возможны недостатки в эффективности и точности логического вывода в определенных условиях, а также сложности в настройке и использовании фреймворка.
`"As shown in Table 5, SMORE achieves significantly faster runtime in 1-GPU setting than PBG, while being slightly slower than Marius."`
> Этот анализ демонстрирует как результаты соответствуют поставленным задачам и целям, так и характеристики и ограничения разработанного фреймворка.

#### Вопросы касательно результата автору
1) Какие минимальные/рекомендуемые конфигурации CPU, GPU и памяти необходимы для работы с огромными графами (например, Freebase)?
2) Как SMORE обрабатывает пропущенные или ошибочные связи в KG?
