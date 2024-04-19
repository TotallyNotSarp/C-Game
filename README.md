<h1>Дизайн-документ:
  No Brake Knight</h1>

<h3>Платформа:</h3> ПК

<h3>Технологии:</h3> Monogame/Godot

<h3>Язык:</h3> Русский

<h3>Жанры:</h3> Runner, Аркада, Hack n slash

<h3>Настроение:</h3> Интерес/страх перед неизвестным

<h3>Сеттинг:</h3> Динамичный раннер, действия которого разворачиваются в альтернативной реальносиь, где людям пришлось переселиться на другую планету, наполненную инопланетной живностью.

<h3>Длительность игры:</h3> Среднее время игровой сессии 5-15 минут

<h2>1. Сюжет</h2>

Люди уже давно начали колонизировать другие планеты, но не все из них оказались безопасными. Вы - опытный страж базы на одной из таких планет, но есть одно "но", ______, поэтому вам нельзя тормозить во время зачистки!

<h2>2. Игровой мир</h2>

Другая планета со своей флорой и фауной. Главный, в том числе по визуалу, пример - Return. https://www.youtube.com/watch?v=dUCDpCevjmk

<h2>3. Геймплей</h2>

Раннер, целью которого добежать из точки А в точку Б, победив ВСЕХ врагов (можно пропустить до 3 - условно 3 жизни). Но если игрок сталкивается со стеной или получает урон от врага, забег проигран. Игрок должен отслеживать: состояние персонажа (чтобы ни во что не врезаться и не получить урон от врагов), положение врагов на экране (чтобы никого не пропустить). В распоряжении игрока есть меч (ближний бой) и пистолет (дальний бой, для летающих целей). Причем в пистолете ограничены патроны, что исключает возможность беспорядочной стрельбы в воздух в надежде попасть по врагу. Боезапас пополняется со временем/после подбора патрон, выпадающих из врагов/ящиков). Также есть щит, который нужно использовать в определенных ситуациях, например, когда враг стреляет в игрока (так как он длится 1 секунду и имеет перезарядку), и перекат (чтобы проходить через узкие пространства)

Основные механики: Прыжок, Перекат, Щит, Удар мечом, Выстрел
*Щит под вопросом, возможно стоит переработать.

<h2>4. Объекты, предметы</h2>

<h3>Окружение:</h3> Земля, Сплошные блоки, Разрушаемые блоки (рушатся при ударе/выстреле), Разрушаемые ящики (если будут), Шипы (Техническое название, на деле это любой объект, убивающий врага при контакте, кроме врагов.)

<h3>Враги (пока без названий, не все могут дойти до реализации):</h3>
Базовый враг - погибает от удара мечом/выстрелом

Базовый летающий враг - погибает от выстрела, так как недосягаем

Большой враг - для победы над ним необходимо сначала выстрелить, затем ударить мечом (так как 2 удара обычным мечом не успеть)

Летающий враг, который при получении урона отлетит назад и изменит свое положение (соответственно необходимо 2 выстрела)

Летающий и стреляющий враг - как только заметит врага, сделает один выстрел. Умирает с 1 удара.

Предметы: С врагов/ящиков периодически будут выпадать заряды, пополняющие боезапас.

<h3>Другие сущности: </h3>
Пуля игрока, пули врага 

<h2>5. Взаимодействия</h2>

<h3>Ввод игрока:</h3> space - прыжок
shift - перекат
Лкм - удар мечом
Колесо мыши - щит
Пкм - выстрел

<h3>Игро-враги:</h3>
Удар мечом по врагу убивает его/наносит урон + использует способность врага (если есть)
Выстрел по врагу убивает его/наносит урон + использует способность врага (если есть)
Игрок касается врага - смерть, перезапуск игры.
Игрок пропускает врага - повышенип счётчика пропусков. Если счётчик достиг 3 - поражение, перезапуск игры.

<h3>Игрок-окружение:</h3>
Удар/выстрел по разрашаемому объекту - разрушает объект
Удар/выстрел по ящику - разрушает ящик, спавнит заряд.
Попадание снаряда по игроку - смерть, перезапуск игры
Столкновения со стеной - смерть, перезапуск игры
