Задание для ElectronJS разработчика.
Форкнуть данный репозиторий на свою машину.
Написать решение.
Кинуть пулл-реквест.
Срок выполнения - два дня - хорошо, один день - отлично!
Используя фреймворк electronjs написать fullstack-приложение два-в-одном *"Интернет банк финансовой грамотности для родителя/ребенка"*

на странице авторизации необходимо реализовать выбор следующего интрефейса (ребенок или родитель), в зависимости от введенных авторизациооных данных (бекенд должен возвращать тип авторизуемого пользователя)

если авторизуется родитель, приложение должно иметь:
- авторизационную часть
- главную страницу с отображением послежних 10 транзакций последнего просмотренного ребенка, ниже список детей, при клике на каждого должен быть редирект на страницу ребенка с аналитикой по этому ребенку, если это не первый выход, если первичный вход и родитель еще никого из детей не просматривал - просто пустая страница с баллансом родителя
- страницу запросов от ребенка на оплату выбранных им товаров
- страницу заданий для ребенка (вымыть пол, убрать в квартире и тд), с прогрессом их выполнения датой начала выполнения задания, дедлайном и ценой на данное задание, с возможностью перехода на страницу создания задания для ребенка
- страницу перевода средств ребенку
- страницу лимитов на суточные транзакции ребенка с виртуализированным списком (элемент не должен быть отрендерен если он находится вне поля зрения)

если авторизуется ребенок, приложение для ребенка должно иметь:
- авторизаионную часть
- главную страницу в которой будут три секции - верхняя - активное задание с наибольшим процентом выполнения, по клику на которое, ребенок попадает на описание данного задания; среднюю - горизонтальный скролл-лист с 10 и более наиболее выгодными (время на выполнение и цена) заданиями от родителя, при клике на плитку любого из таких заданий ребенок попадает на описание данного задания; нижнюю - история выполненных и невыполненных заданий с возможностью фильтрации по сатусу
- страница принятия/ просмотра задания от родителя
- страницу запросов, созданных ребенком ранее с возможностью создавать запросы ( например хочу кроссовки, цена, фото и кнопка запросить), данные запросы ребенок отсылает родителю, который в последствии может прикрепить этот запрос к любому из существующих заданий или к новому заданию
- страницу статистики по заданиям ( общее число заданий выполнено, сколько денег заработано, какие вещи куплены ( с секцией предложений "вам так же могут понравиться" и далее горионтальный список вещей, аналогичных тем, которых больше всего в категории выполнено раньше дедлайна(например если ребенок получил в награду телефон - то должны быть аксессуары к нему или ноутбук и тд)))
- страницу друзей/братьев/сестер, в которой можно поделиться своими достижениями и посмотреть кто что сейчас выполняет

фронт должен быть написан на ReactJS с использованием typescript, никакого редакса
вся логика и запросы к бэкенду - должны быть реализованы в главном потоке

сам бекенд писать не нужно, все запросы к бэку просто замокать.

