# dop_zadanie
Дополнительное задание команды Сириус ИИ (лидер/капитан Михальченко Э. С).
В рамках дополнительного задания наша команда разработала прототип определения мошеннических кошельков.
Мы анализировали только криптовалюту Ethereum.
С помощью открытых источников (в том числе с платформы Kaggle) был получен размеченный датасет кошельков пользователей, в котором имелась разметка на мошеннические и добросовестные кошельки.

Была проведена подготовка данных для дальнейшего обучения модели машинного обучения.

Затем была обучена модель LGBMClassifier - это классификатор, основанный на градиентном бустинге над деревьями решений, реализованный в библиотеке LightGBM. LightGBM (Light Gradient Boosting Machine) - это быстрая и эффективная библиотека для градиентного бустинга, разработанная Microsoft. Данная модель была обучена до высокого уровня точности.

Далее был написан код для получения данных о всех транзакциях кошелька. После этого определяется, являются ли транзакции мошенническими или нет, и пользователю выводится процент мошеннических транзакций на кошельке. Он может самостоятельно принять решение о совершении транзакции.

Автоматические системы могут установить порог мошеннических транзакций на кошельке для признания его мошенническим.
