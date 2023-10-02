# Rucode2023 Задача A

*Требуется:* реализовать регрессионную модель, которая будет по имеющимся данным восстановливать данные из столбца "Доля сигнала в ВП"

--------------------------------------------------------
Решение:
- CatBoostRegressor
- LGBMRegressor
- XGBRegressor
- RandomForestRegressor x2
- ExtraTreesRegressor x2
  - BaggingRegressor:
- DecisionTreeRegressor
- VotingRegressor:
  - DecisionTreeRegressor
  - ExtraTreesRegressor
  - RandomForestRegressor
  - CatBoostRegressor
  - XGBRegressor
  - LGBMRegressor
- BaggingRegressor: x2
  - ExtraTreesRegressor
- BaggingRegressor:
- RandomForestRegressor
- LinearRegression


Ключевой аспект решения:
- удалены мусорные признаки
- использование базовых моделей наряду с ансамблями моделей

Метрика: *70 * R2*

|public|privat|
|------|------|
|58.98 |51.49 |

Директории:
- models - веса моделей
- data - предоставленные данные
- params - подобранные гиперапараметры моделей
