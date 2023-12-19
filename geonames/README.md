# Сопоставление названий городов
[ipynb](https://github.com/tkachuk45/portfolio/blob/main/geonames/geonames_project.ipynb)

## Описание проекта
Нужно находить название города максимально похожее на произвольное введеное название. Название должно быть унифицировано по общепринятому стандарту geonames. Решение задачи поможет заказчику улучшить пользовательский опыт при заполнении форм. Все данные должны храниться в БД PostgreSQL.

Для валидации решения заказчик предоставил размеченный тестовый датасет с произвольными запросами и правильно сопоставленными названиями городов из geonames.

## Использованные библиотеки
- **pandas**
- **numpy**
- sqlalchemy.**create_engine**
- sqlalchemy.engine.url.**URL**
- transliterate.**translit**
- sklearn.feature_extraction.text.**TfidfVectorizer**
- sklearn.metrics.pairwise.**cosine_similarity**
- pathlib.**Path**


## Общий итог
Мы создали базу данных PostgreSQL и поместили в нее данные. Далее сформировали срез данных, провели обработку и векторизацию. Затем создали рабочее решение, которое находит нужное название города из geonames. Мы проверили качество решения - алгоритм показал хороший уровень accuracy. Мы составили рекомендации по дальнейшему улучшению алгоритма.