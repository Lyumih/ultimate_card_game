# ultimate_card_game
Движок ККИ, в которой можно за 1 минуту создать карту с нужной механикой. Цель: скопировать все карты со всех кки

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
8. Общее: есть основные черты (карты: жизнь, атака, стоимость; механика: ресурс, смена хода, победа, сдаться) и второстепенные(защита, название фаз и т.п.).


# Конструктор
1. Цепь: конструктор представляет собой цепочки механик.
2. Последовательность: цепочки представляют из себя упорядоченный набор свойств.

# Карты
1. Основа карт: ЖИЗНЬ, АТАКА, СТОИМОСТЬ маны для вызова.
2. Основной контракт карт: основные свойства карт будут обязательно обработаны в механики игры.
3. Свойства карты: вложенная структура класса.

# Механика игры
1. Основа механики: ресурс, смена хода, победа, сдаться.
2. Основной контракт механики: основные механики игры будут обязатально обрабатывать основу карт.
