

<h1 align="center"> МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>

<p align="center">Лабораторная работа №5 "JavaScript" </p>

<p align="right">Выполнил: Морошкин Максим Александрович</p>
<p align="right">Проверил: Соболев Е. И.</p>

<p align="center">г. Южно-Сахалинск <br> 2023 год</p>

<h2 align="center">Введение</h2>
<p align="justify">Лабораторная работа по созданию скриптов на языке JavaScript.</p>

<h2>Цели и задачи</h2>
1.	Создайте переменную str и присвойте ей значение 'hdfgv'. Обращаясь к отдельным символам этой строки выведите на экран символ 'h', символ 'd', символ 'v'.
2.	Напишите скрипт, который считает количество секунд в часе.
3.	Переделайте приведенный код так, чтобы в нем использовались операции +=, -=, *=, /=, ++, --. Количество строк кода при этом не должно измениться. Код для переделки:
var num = 1;
num = num + 12;
num = num - 14;
num = num * 5;
num = num / 7;
num = num + 1;
num = num - 1;
alert(num);

4.	Создайте переменную num и присвойте ей значение 3. Выведите значение этой переменной на экран с помощью метода alert.
5.	Создайте переменные a=10 и b=2. Выведите на экран их сумму, разность, произведение и частное (результат деления).
6.	Создайте переменные c=15 и d=2. Просуммируйте их, а результат присвойте переменной result. Выведите на экран значение переменной result.
7.	Создайте переменные a=10, b=2 и c=5. Выведите на экран их сумму.
8.	Создайте переменные a=17 и b=10. Отнимите от a переменную b и результат присвойте переменной c. Затем создайте переменную d, присвойте ей значение 7. Сложите переменные c и d, а результат запишите в переменную result. Выведите на экран значение переменной result.
9.	Напишите скрипт, который считает количество секунд в часе, в сутках, в месяце.
10.	Создайте три переменные - час, минута, секунда. С их помощью выведите текущее время в формате 'час:минута:секунда'.
11.	Создайте переменную, присвойте ей число. Возведите это число в квадрат. Выведите его на экран.
12.	Напишите однострочное решение, которое вычисляет сумму квадратных корней для всех чётных чисел целочисленного массива.
13.	Яблоко стоит 1.15, апельсин стоит 2.30. Сколько они стоят вместе – чему равна сумма 1.15 + 2.30 с точки зрения JavaScript?
14.	Какое будет выведено значение: let x = 5; alert(x++); ?
15.	Чему равно такое выражение: [ ] + false - null + true ?
16.	Что выведет этот код: let y = 1; let x = y = 2; console.log(x); ?
17.	Чему равна сумма [ ] + 1 + 2?
18.	Создайте переменные a6, a7, a8, a9, a10. Поместите в них результат выражений:
5 % 3,
3 % 5,
5 + '3',
'5' - 3,
75 + 'кг'
19.	Напишите скрипт, который находит площадь прямоугольника высота 23см. (в числовую переменную height), шириной 10см (в числовую переменную width), значение площади должно хранится в числовой переменной s.
20.	Напиши скрипт, который находит объем цилиндра высотой 10м (переменная heightC) и диаметром основания 4м (dC), результат поместите в переменную v.
21.	Даны размер ипотечного кредита (S — 2 млн.руб), процентная ставка (p  — 10%), кол-во лет (years — 5). Найти переплату по кредиту, значение переплаты должно содержаться в переменной perepl.
22.	Определите переменные str, num, flag и txt со значениями «Привет», 123, true, «true». При помощи оператора определения типа убедитесь, что переменных принадлежат типам: string, number, boolean.
23.	Дано число, необходимо вернуть противоположное число.


<h2>Решение задач</h2>
code
Код решения задач = https://github.com/MovingX/lab5/blob/main/index1.html <br>
<script>
		function task1() {
			var str = 'hdfgv';
			document.getElementById("result").innerHTML =str[0] + " " + str[2] + " " + str[str.length - 1]; // выводим первый символ
		}

		function task2() {
			var secondsInHour = 60 * 60;
			document.getElementById("result").innerHTML ="В одном часе " + secondsInHour + " секунд";
		}

		function task3() {
			var num = 1;
			num += 12;
			num -= 14;
			num *= 5;
			num /= 7;
			num++;
			num--;
			alert(num);
		}

		function task4() {
			var num = 3;
			alert(num);
		}

		function task5() {
			var a = 10;
			var b = 2;
			document.getElementById("result").innerHTML ="Сумма a и b: " + (a + b) + "<br>" +
                                               "Разность a и b: " + (a - b) + "<br>" +
                                               "Произведение a и b: " + (a * b) + "<br>" +
                                               "Частное a и b: " + (a / b) + "<br>";
		}

		function task6() {
			var c = 15;
			var d = 2;
			var result = c + d;
			document.getElementById("result").innerHTML = result;
		}

		function task7() {
			var a = 10;
			var b = 2;
			var c = 5;
			document.getElementById("result").innerHTML = "Сумма a, b и c: " + (a + b + c);
		}

		function task8() {
			var a = 17;
			var b = 10;
			var c = a - b;
			var d = 7;
			var result = c + d;
			document.getElementById("result").innerHTML = result;
		}
		function task9() {
			var secondsInHour = 60 * 60;
			var secondsInDay = secondsInHour * 24;
			var secondsInMonth = secondsInDay * 30;
			document.getElementById("result").innerHTML = "Секунд в часе " + secondsInHour + "<br>" + "Секунд в дне: " + secondsInDay + "<br>" + "Секунд в месяце: " + secondsInMonth;
		}

		function task10() {
			var date = new Date();
			var hour = date.getHours();
			var minute = date.getMinutes();
			var second = date.getSeconds();
			var time = hour + ":" + minute + ":" + second;
			document.getElementById("result").innerHTML = "Текущее время: " + time;
		}

		function task11() {
			var num = prompt("Введите число:");
			var square = num * num;
			document.getElementById("result").innerHTML = "Число: " + num + " = в квадрате: " + square;
		}

		function task12() {
			var resultDiv = document.getElementById("result");
			var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]; // Замените этот массив на свой собственный
			resultDiv.innerHTML = arr.reduce((acc, curr) => curr % 2 === 0 ? acc + Math.sqrt(curr) : acc, 0);
		}

		function task13() {
			var applePrice = 1.15;
			var orangePrice = 2.30;
			var totalPrice = applePrice + orangePrice;
			document.getElementById("result").innerHTML = "Сумма яблока и апельсина =" + totalPrice;
		}

		function task14() {
			var x = 5;
			alert(x++);
			//Будет выведено значение 5, так как оператор ++ увеличивает значение переменной после того, как она была выведена.
		}

		function task15() {
			document.getElementById("result").innerHTML = [] + false - null + true;
			//неопределенное значение NaN
		}

		function task16() {
			let y = 1;
			let x = (y = 2);
			var text = "чтобы увидеть результат откройте консоль ctrl + shift + i Ответом будет 2"
			console.log(x);
			document.getElementById("result").innerHTML = text;
		}

		function task17() {
			document.getElementById("result").innerHTML = [] + 1 + 2;
			//Результатом будет строка "12", так как при сложении массива и числа 1 получится строка "1"
			//А затем при сложении строк "1" и "2" получится строка "12"
		}
		
		function task18() {
			var a6 = 5 % 3;
			var a7 = 3 % 5;
			var a8 = 5 + '3';
			var a9 = '5' - 3;
			var a10 = 75 + 'кг';

			var result = "a6: " + a6 + "<br>" +
						"a7: " + a7 + "<br>" +
						"a8: " + a8 + "<br>" +
						"a9: " + a9 + "<br>" +
						"a10: " + a10 + "<br>";

			document.getElementById("result").innerHTML = result;
		}


		function task19() {
			var height = 23;
			var width = 10;
			var s = height * width;
			document.getElementById("result").innerHTML = "Площадь прямоугольника: " + s;
		}

		function task20() {
			var heightC = 10;
			var dC = 4;
			var r = dC / 2;
			var v = 3.14 * r * r * heightC;
			document.getElementById("result").innerHTML = "Объем цилиндра: " + v;
		}

		function task21() {
			var S = 2000000;
			var p = 0.1;
			var years = 5;
			var perepl = S * p * years;

			document.getElementById("result").innerHTML = "Переплата по кредиту: " + perepl + " руб.";
		}	

		function task22() {
			var str = "Привет";
			var num = 123;
			var flag = true;
			var txt = "true";

			var result = "str: " + typeof str + "<br>" +
						"num: " + typeof num + "<br>" +
						"flag: " + typeof flag + "<br>" +
						"txt: " + typeof txt + "<br>";

			document.getElementById("result").innerHTML = result;
		}

		function task23() {
			var num = prompt("Введите число:");
			var opposite = -num;

			document.getElementById("result").innerHTML = "Противоположное число: " + opposite;
		}
		
		function task1CW() {
			var sperm = prompt("Введите хромосомы:");
			var resultDiv = document.getElementById("result");
			if (sperm == "XY") {
				return resultDiv.innerHTML = "Congratulations! You're going to have a son.";
			} else if (sperm == "XX") {
				return resultDiv.innerHTML = "Congratulations! You're going to have a daughter.";
			} else {
				return resultDiv.innerHTML = "not value";
			}
		}
		
		function task2CW() {
			var number = prompt("Введите число:");
			var resultDiv = document.getElementById("result");
			if (number % 2 == 0)
			{
			resultDiv.innerHTML = number * 8;
			} else resultDiv.innerHTML = number*9;
		}
		
		function task3CW(){
			var n = prompt("Введите число:");
			var resultDiv = document.getElementById("result");
			var temp = Math.round(Math.sqrt(n))
			var result = Math.pow(temp, 2)
			resultDiv.innerHTML = result;
		}
		
		function task4CW(){
			var cuts = prompt("Введите число:");
			var resultDiv = document.getElementById("result");
			if (cuts == 0) return resultDiv.innerHTML = 1;
			var temp = Math.pow(cuts + 1, 3);
			var temp1 = Math.pow(cuts - 1, 3);
			resultDiv.innerHTML = temp - temp1;
		}
		
		function periodIsLate(last, today, cycleLength) {
			var temp = Math.ceil((today - last)/(1000*60*60*24));
			if (temp > cycleLength) return true; else return false;
		}
		
		function task6CW(){
			var x = prompt("Введите строку:");
			var resultDiv = document.getElementById("result");
			resultDiv.innerHTML = x.replaceAll(" ", "");
		}
		
		</script>		

Задачи на codewars.com  = https://www.codewars.com/users/MovingX/completed_solutions <br>
<h2>Вывод</h2>
Я научился работать с JavaScript, GitHub, CodeWars
