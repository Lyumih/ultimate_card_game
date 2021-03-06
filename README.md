# Ultimate Card Game (Mutation Game Engine)
ККИ - Коллекционная Карточная Игра. Например, Hearthstone.  
*Наш проект* - это движок ККИ, в котором можно за 1 минуту создать карту с нужной механикой.  
*Цель*: скопировать практически все карты и механики с существующих ККИ

# С чего начать
1. Скачать архив и запустить index.html
2. Открыть CONTRIBUTING.md - там задания, с чего можно начать
3. Посмотреть Issues
4. В папке "mechanics_and_cards" посмотреть примерный результат работы конструктора

# Цель создать удобный конструктор, в котором можно будет перенести карты из других игр
Максимальный акцент:
1. Скорость перенесения свойств и механик карты.
2. Способ добавления новой карты.
3. Поиск по текущим картам.
4. Добавление изображения карт к текущей карте через url.  
Минимальный акцент:
1. Дизайн карт.



# Особенности
1. Наследие: Большинство особенностей происходят из-за различный механик других кки.
2. Конструктор: Чтобы описать механику игры, нужно набрать свойств особенностей данной игры (через конструктор).
3. Изолированность: Карты и механика игры изолированны друг от друга.
4. Множественность имён: одно имя свойста может быть разным из разных игр.
5. Совпадение имён: если одно свойство повторяется в разных играх, то можно перечислить несколько игр.
6. Пары: "имя карты/механики - главная игра". 
7. Историчность: всегда есть ссылка на игру, откуда была взята карта/механика.
8. Общее: есть основные черты (карты: имя, жизнь, атака, стоимость; механика: ресурс, смена хода, герой, победа, сдаться) и второстепенные(защита, название фаз и т.п.).
9. Инстинкт: каждое свойство механики или карты знает как себя вести по умолчанию, если отсутвуют конкретные параметры


# Конструктор
1. Цепь: конструктор представляет собой цепочки елементов для карт/механик
2. Последовательность: цепочки представляют из себя упорядоченный набор свойств.
4. Каждое поле предоставляет checkbox с наличием этих свойств и строку ввода с значением свойства
3. Зарезервированные слова: void, true, false.
5. Если основа не указана, берутся значения по умолчанию

# Карты
1. Основа карт: ИМЯ, ЖИЗНЬ, АТАКА, СТОИМОСТЬ маны для вызова.
2. Основной контракт карт: основные свойства карт будут обязательно обработаны в механики игры.
3. Свойства карты: вложенная структура класса.

# Механика игры
1. Основа механики: РЕСУРС, ХОД, ГЕРОЙ, ПОБЕДА, СДАТЬСЯ.
2. Основной контракт механики: основные механики игры будут обязатально обрабатывать основу карт.
