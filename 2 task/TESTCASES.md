<?xml version="1.0" encoding="UTF-8"?>
<suite>
	<id>S2</id>
	<name>Master</name>
	<description></description>
	<sections>
		<section>
		<name>Проверка отображения экосчетчиков</name>
		<description>Без авторизации пользователя, с общими результатами</description>
						<cases>
												<case>
				<id>C1</id>
				<title>Счетчик сохранённого объёма воды</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
								<status>Design</status>
<assignedto>Evgeniy Vlad</assignedto>
												<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;, счетчик сохранённого объёма воды, в миллионах кубических метров</expected></step>
</steps_separated>
									</custom>
							</case>
															<case>
				<id>C2</id>
				<title>Счетчик предотвращённого объёма выброса CO2</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
								<status>Design</status>
<assignedto>Evgeniy Vlad</assignedto>
												<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>Кликнуть 1 раз на стрелку &quot;вправо&quot;, для переключения на счетчик предотвращённого объёма выброса CO2, в миллионах тонн</content><expected>Отображается счетчик предотвращённого объёма выброса CO2, в миллионах тонн</expected></step>
</steps_separated>
									</custom>
							</case>
															<case>
				<id>C3</id>
				<title>Счетчик сэкономленной электроэнергии</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
								<status>Design</status>
<assignedto>Evgeniy Vlad</assignedto>
												<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>Кликнуть 2 раза на стрелку &quot;вправо&quot;, для отображения счетчика сэкономленной электроэнергии, в миллиардах киловатт-часов</content><expected>Отображается счетчик сэкономленной электроэнергии, в миллиардах киловатт-часов</expected></step>
</steps_separated>
									</custom>
							</case>
								</cases>
								<sections>
		<section>
		<name>Тестирование верстки</name>
		<description>Без авторизации пользователя, с общими результатами</description>
						<cases>
												<case>
				<id>C4</id>
				<title>Тестирование верстки счетчиков на странице сайта</title>
												<template>Test Case (Steps)</template>
																<type>Other</type>
																<priority>Medium</priority>
																				<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>1) Кликнуть несколько раз на стрелку &quot;вправо&quot;, для сравнения дизайна счетчиков (цвет текста, шрифт, расположение на странице сайта, скорость отклика на нажатие стрелки &quot;вправо&quot;). 
2) Убедиться, что на каждом счетчике разная анимация. 
3) Удостовериться, что текст и анимация соответствуют контексту каждого счетчика.</content><expected>1) Все счетчики выполнены в одном стиле. Скорость отклика на переключение между счетчиками одинаковая.
2) На каждом счетчике разная анимация.
3) Текст и анимация соответствуют контексту каждого счетчика.</expected></step>
</steps_separated>
									</custom>
							</case>
								</cases>
								<sections>
		<section>
		<name>Авторизация/регистрация</name>
		<description></description>
						<cases>
												<case>
				<id>C5</id>
				<title>Регистрация</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
																				<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>Проскроллить до кнопки &quot;Авторизоваться&quot; и кликнуть на нее</content><expected>Открывается окно с возможностью авторизоваться или зарегистрироваться на сайте</expected></step>
<step>
<content>Под кнопкой &quot;Зарегистрироваться&quot;, кликнуть на надписи: &quot;ознакомиться с условиями использования Авито&quot; и &quot;политикой конфиденциальности&quot; и ознакомиться с ними</content><expected>Открываются  &quot;условия использования Авито&quot; и &quot;политика конфиденциальности.</expected></step>
<step>
<content>Нажать кнопку &quot;Зарегистрироваться&quot;</content><expected>Открывается окно &quot;Введите номер телефона&quot;</expected></step>
<step>
<content>В поле ввода номера телефона ввести свой номер телефона, в формате +7, и нажать кнопку &quot;продолжить&quot;</content><expected>На телефон придет смс с кодом, для регистрации. Открывается  окно &quot;Подтвердите номер&quot;</expected></step>
<step>
<content>В поле код из смс, ввести код и нажать кнопку &quot;подтвердить&quot;</content><expected>Новый пользователь зарегистрирован на сайте</expected></step>
</steps_separated>
									</custom>
							</case>
															<case>
				<id>C6</id>
				<title>Авторизация</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
																				<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<preconds>C5</preconds>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>Проскроллить до кнопки &quot;Авторизоваться&quot; и кликнуть на нее</content><expected>Открывается окно с возможностью авторизоваться или зарегистрироваться на сайте</expected></step>
<step>
<content>Ввести валидный номер телефона/e-mail и пароль, в соответствующих полях и нажать кнопку &quot;войти&quot;</content><expected>Открывается сайт с учетной записью пользователя</expected></step>
</steps_separated>
									</custom>
							</case>
								</cases>
							</section>
	</sections>
			</section>
	</sections>
			</section>
			<section>
		<name>Скриншот счетчиков</name>
		<description></description>
						<cases>
												<case>
				<id>C7</id>
				<title>Тест работы скриншота</title>
												<template>Test Case (Steps)</template>
																<type>Functional</type>
																<priority>Medium</priority>
								<status>Design</status>
												<estimate></estimate>
																								<references></references>
																				<custom>
										<automation_type><id>1</id><value> Ranorex</value></automation_type>
										<steps_separated><step>
<content>Открыть сайт Авито https://www.avito.ru/avito-care/eco-impact</content><expected>Открывается сайт Авито, раздел &quot;экосчетчик&quot;</expected></step>
<step>
<content>Проскроллить вниз до счетчиков</content><expected>Отображаются счетчики</expected></step>
<step>
<content>Открыть SublimeText и написать код для вывода скриншота счетчиков в папку &quot;output&quot;</content><expected>В папке &quot;output&quot; появляется скриншот счетчиков</expected></step>
</steps_separated>
									</custom>
							</case>
								</cases>
							</section>
	</sections>
</suite>
