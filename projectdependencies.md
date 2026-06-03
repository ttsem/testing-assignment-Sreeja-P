                +----------------------+
                |   ICalculator        |
                +----------------------+
                         ▲
                         │
                 +---------------+
                 |  Calculator   |
                 +---------------+

                +-------------------------+
                | IHistoryRepository      |
                +-------------------------+
                         ▲
                         │
         +-------------------------------------+
         | XmlHistoryRepository                |
         +-------------------------------------+

                +----------------------+
                | ICalculatorService   |
                +----------------------+
                        ▲
                        │
                +------------------------------+
                | CalculatorService            |
                |------------------------------|
                | - ICalculator                |
                | - IHistoryRepository         |
                +------------------------------

                        │
                        ▼
                +----------------------+
                | CalculationRecord    |
                +----------------------+

Calculator implements ICalculator
XmlHistoryRepository implements IHistoryRepository
CalculatorService implements ICalculatorService
CalculationRecord is a model
CalculatorService depends on ICalculator and IHistoryRepository


