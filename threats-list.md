КЛАССИФИКАЦИЯ УГРОЗ
# По цели воздействия
## Нарушение [конфиденциальности](cia-triad.md)
## Нарушение [целостности](cia-triad.md)
1. [SQL-инъекции](owasp-10.md)
## Нарушение [доступности](cia-triad.md)
1. DDOS-атаки (англ. Distributed Denial of Service — распределенный отказ в обслуживании)
	1. флуд-атака — одна из разновидностей
# По характеру возникновения
## Случайные 
## Преднамеренные (По характеру воздействия)
### Активные 
влияют на работу всей системы
1. вирус virus
	 прикрепляется к хосту (например, файлу или программному обеспечению) и размножается при запуске хоста. Вирусы могут повреждать, удалять или модифицировать данные и снижать производительность системы.
2. вирус-вымогатель (шифровальщик) ransomware
	шифрует файлы своих жертв и требует выкуп, как правило, в виде криптовалюты, за ключ для расшифровки. Если жертва откажется или не сможет заплатить в течение указанного срока, зашифрованные данные могут быть потеряны навсегда.
	примеры: Wanna Cry, Bad Rabbit, Petya.
3. черви worms
	самореплицирующееся вредоносное ПО, которое распространяется по сетям без вмешательства человека. Они используют уязвимости системы, потребляя пропускную способность, а иногда и несут полезную нагрузку для заражения целевых компьютеров.
4. трояны trojan horse
	 замаскированы под законную программу, но содержат вредоносный код. они могут использоваться для кражи данных, создания бэкдора или запуска дополнительных вредоносных атак.
5. шпионское по spyware
	предназначен для сбора и передачи информации о пользователях или организации без их согласия. может перехватывать нажатия клавиш, записывать историю посещенных страниц и получать доступ к личным данным, таким как имена пользователей и пароли.
6. [SQL-инъекции](owasp-10.md)
### Пассивные
могут быть подготовкой к активной атаке. как правило, лишь собирают не санкционировано информацию.
1. кей-логгеры keylogger
	фиксируюn ввод данных с клавиатуры, позволяя злоумышленникам получать конфиденциальную информацию, такую как учетные данные для входа в систему или финансовая информация, введенная с клавиатуры.
2. руткит rootkit
	тип вредоносного ПО, предназначенный для сокрытия присутствия других вредоносных программ в компьютерной системе. позволяет ему поддерживать постоянный несанкционированный доступ к системе и может затруднить пользователям или программному обеспечению безопасности обнаружение и удаление зараженных файлов.
3. рекламное ПО adware
	автоматически отображает или загружает рекламные материалы, часто в виде всплывающих окон, на компьютер пользователя. не всегда является вредоносным, оно может быть навязчивым и открывать путь для заражения другими вредоносными программами.
4. снифферы
5. несанкционированные RDP
# По способу реализации
## [Несанкционированный доступ](unauthorized-access.md)
## [Утечка информации по техническим каналам связи](info-leakage.md)
# По длительности
## Кратковременные
## Долговременные
1. целенаправленные (англ. Advanced Persistent Threat)
# По природе возникновения
## Антропогенные
связаны с действиями человека
## Техногенные 
связаны с недостатками технических средств или ПО в инф. системе
## Стихийные
# По принципу воздействия
часто исходит из-за наличия не устраненных уязвимостей, в том числе «нулевого дня», в операционных системах или прикладном ПО, позволяющих получить привилегированный доступ к рабочей станции
## С использованием скрытых каналов
## С использованием доступа субъекта к объекту
# По типу злоумышленника
## Внешние
## Внутренние
как правило, часто именно изнутри исходят угрозы. такой злоумышленник может быть как шпионом от конкурента, так и ленивым администратором в компании. 
# По объекту атаки
## На субъекты информационных систем 
## На объекты информационных систем
# По наличию обратной связи с атакуемым объектом
## Без обратной связи
## С обратной связью
# источники
1. Гродзенский Я. С. «Информационная безопасность : учебное пособие» – Москва : РГ-Пресс, 2020. стр. 12-14
2. https://roadmap.sh/cyber-security