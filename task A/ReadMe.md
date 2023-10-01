# Rucode2023 Задача A

*Требуется:* реализовать регрессионную модель, которая будет по имеющимся данным восстановливать данные из столбца "Доля сигнала в ВП"


--------------------------------------------------------
Решение:
- VotingClassifier:
  - СatBoostClassifier
  - XGBClassifier

Ключевой аспект решения:
- отдельная модель для каждого *№ испытания*

Метрика: *30 * F1_macro*

|public|privat|
|------|------|
|29.78 |29.93 |

Директории:
- models - веса моделей
- data - предоставленные данные