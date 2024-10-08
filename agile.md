Для того, чтобы контролировать качество кода и отслеживать грубые ошибки или бэкдоры созданы специальные программы — анализаторы кода и исполняемых файлов.
# learn production бережливое производство
В 1950-е годы Т. Оно теоретически обосновал концепцию Lean production («Бережливое производство»), а его коллега С. Синго помог ее практически осуществить. Выделено пять шагов:
1. определить, что есть ценность для клиента;
2. организовать поток создания ценности;
3. организовать движение этого потока;
4. создать механизм вытягивания;
5. непрерывно совершенствовать созданную систему («кайдзен»).[^1]
# agile enterprise активное предприятие
активным можно считать такое предприятие, организационная структура и процессы администрирования которого способны быстро и гибко перестраиваться с учетом необходимости действовать в интересах потребителей.
так как изменения могут происходить на даже последних стадиях работы, важно встроить процесс анализа кода в сам процесс разработки ПО и управления версиями разрабатываемого продукта.
# сканеры кода
способы проверки:
1. лексический, семантический и синтаксический анализ;
2. taint-анализ;
3. анализ распространения типов и констант;
4. анализ синонимов и прочие;
5. проверять только то, что изменилось, или проверять код ПО от версии к версии.
сканеры не только указывают на ошибки и не декларированные возможности (НДВ) в коде, но предлагают методы устранения. ошибки могут быть [1-го и 2-го рода](true-false.md), когда есть риск пропустить ошибку в коде, с одной стороны, и выявить ошибку там, где ее на самом деле нет. для борьбы с ними существуют оптимальные статистические критерии вальдовского типа. некоторые сканеры обладают функцией декомпиляции уже готовых приложений, что означает можно проследить логику работы приложения (часто лицензионные соглашения запрещают реверс-инжиниринг и его частный случай - декомпиляцию).
## статический SAST и динамический DAST
два основных вида анализа программного обеспечения на наличие уязвимостей. статический SAST проверяет исходный код, а динамический DAST проверяет программу в процессе её выполнения.
в идеале использовать оба вида анализа. в одних ситуациях динамический метод определит, что значения уходят за пределы массива или цикл длится бесконечно, в другом случае статический метод укажет на ошибку в синтаксисе, когда нет скобки или символ стоит не на своём месте.
# сканеры веб-приложений и возможности обычного браузера
Современные сканеры кода веб-приложений содержат как статический анализ кода, так и динамический и при этом могут интегрироваться с [WAF](firewall.md) для обеспечения безопасности приложений. Некоторые из сканеров кода веб-приложений поддерживают возможность генерации эксплойтов на лету, что позволяет протестировать реальную опасность уязвимостей, и загружают готовый патч для исправления в [WAF](firewall.md), который создает соответствующее правило для блокировки атаки.[^2]

Встроенные средства разработчика в браузере полезны тем, что можно увидеть код html-страницы, даже если при загрузке была пустая страница. В скрытых от глаз данных могут содержаться URL на внутренние ресурсы, «скрытый» frame с формой входа и т.д. Можно не увидеть перехода на сайт, при этом будет загружаться вредоносное ПО.[^3]

[^1]: Гродзенский Я. С. «Информационная безопасность : учебное пособие» – Москва : РГ-Пресс, 2020. стр. 67
[^2]: Гродзенский Я. С. … стр. 71
[3]: Гродзенский Я. С. … стр. 72