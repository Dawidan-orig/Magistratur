![[Архитектура - Clean Architecture по Мартину.png]]

Clean Architecture объединила в себе идеи нескольких других архитектурных подходов, которые сходятся в том, что архитектура должна:
- быть тестируемой;
- не зависеть от UI;
- не зависеть от БД, внешних фреймворков и библиотек.



Нейро:
**Fernando Cejas Clean Architecture** — это адаптация Clean Architecture Роберта Мартина для Android/Django, организованная в 3 слоя с зависимостями от внешнего к внутреннему
```
project/
├── presentation/     # UI: Views, Controllers, Forms, Serializers
├── domain/           # Бизнес-логика: Use Cases, Domain Models (POCO)
└── data/             # Инфраструктура: Repositories, DB, API

```