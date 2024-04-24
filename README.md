# RPG-game-test-project
 пет-проект

Описание проекта
Данный проект был создан для того что бы протестировать свои навыки во владении Unity и мною было установлен чёткий промежуток времени за который была завершена его разработка а именно 4 месяца.

Проект включает в себя

1) Процедурная генерация локации с использованием LeoECS framework
    а) Построение синусоиды и её проекция на 2D текстуру (генерация первой карты высот для
ландшафта реки)
    b) Генерация реки по карте высот с применением SimplyfyMeshFilter для уменьшения
количества полигонов на модели реки и её проекция на местность
    c) Построение карты высот для холмов и низменостей на местности методом шумов
Перлина
    d) Комбинирование карт высот реки и холмов в одну единую карту высот и поекция её на
местность
    e) Генерация слоёв текстур и их кобенирование
    f) Применение созданных комбенированых тексту на местность в зависимости от заданых
высот
    g) Генерация объектов (трава, деревья, камни) на местности с маркерами для будующей
мини карты,
для объектов котрые без маркеров применяется MeshCombiner для снижения количествов
вызовов к рендерингу и уменьшению нагрузки на CPU и GPU
    h) Запикание местности для NavMesh

2) Создание анимированного персонажа
    a) Реализация управления вводом с использованием framework Imput system
    b) Реализация animator с использованием State Empty и Blend tree
    c) Реализация характеристик персонажа
    d) Реализация взаимодействия с окружением а именно добыча ресурсов и бой с
противником

3) Создание анимированного противника
    a) Реализация NavMeshAgent а именно патрулирование, преследование при входе игрока
    в) пределы видимости противника, поиск пути к игроку
    b) Реализация характеристик противника и выпадение предметов после смерти с
реализацией RagDoll
    c) Реализация animator с использованием State Empty и Blend tree
    
4) Графический интерфейс и Post-processing
    a) Настройки:
 громкость аудио и его сохранение в PlayerPrefs;
 улучшение или ухудшение графики с помощью Quality
 включение и выключение визуальных эффектов таких как Grain, Color Grading, Depth of
field, Auto Exposure, Ambient Occlusion
    b) Мини карта с маркерами противников и ресурсов по близости
    c) Инвентарь персонажа с механикой одевания персонажа
    d) Реализация системы крафта предметов
    e) Реализация дерева талантов и прокачки персонажа