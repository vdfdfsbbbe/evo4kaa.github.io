<!DOCTYPE html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>С днем влюбленных!</title>
</head>
    <style>
	overflow: hidden;    
	/* Общий контейнер для фото */
.photo-gallery {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
    margin-top: 20px;
    opacity: 0; /* Скрываем, пока не появится */
    animation: fadeIn 2s ease-in-out forwards;
}

/* Верхний ряд (фото слева и справа) */
.photo-row {
    display: flex;
    justify-content: space-between;
    width: 100%;
    max-width: 500px;
}

/* Фото слева */
.left-photo {
    align-self: flex-start;
}

/* Фото справа */
.right-photo {
    align-self: flex-end;
}

/* Нижнее фото (по центру) */
.photo-row.center {
    justify-content: center;
}

/* Стиль для фото */
.photo-gallery img {
    width: 250px; /* Размер фото */
    height: auto;
    border-radius: 15px; /* Закруглённые углы */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* Тень */
    transition: transform 0.3s ease-in-out;
}

/* Эффект увеличения при наведении */
.photo-gallery img:hover {
    transform: scale(1.2);
}

/* Анимация плавного появления */
@keyframes fadeIn {
    0% { opacity: 0; transform: translateY(20px); }
    100% { opacity: 1; transform: translateY(0); }
}

	.love-box {
    background: #ffdde1; /* Нежно-розовый фон */
    border: 5px solid #ff4d6d; /* Розовая рамка */
    padding: 20px;
    border-radius: 15px;
    max-width: 500px;
    text-align: center;
    margin: 20px auto;
    box-shadow: 0 0 15px rgba(255, 77, 109, 0.6); /* Красивое свечение */
    opacity: 0;
    animation: fadeIn 2s ease-in-out forwards;
}

/* Стиль для текста */
.love-message {
    font-size: 20px;
    color: #ff1654; /* Красивый розовый цвет */
    font-weight: bold;
    text-shadow: -2px -2px 0 #fff, 2px -2px 0 #fff, -2px 2px 0 #fff, 2px 2px 0 #fff; /* Белая обводка */
    line-height: 1.6;
}

/* Анимация плавного появления */
@keyframes fadeIn {
    0% { opacity: 0; transform: scale(0.9); }
    100% { opacity: 1; transform: scale(1); }
}

@keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
}
	.love-card {
    background: #ff4d4d;
    color: white;
    padding: 20px;
    border-radius: 10px;
    font-size: 24px;
    font-weight: bold;
    box-shadow: 0 0 15px rgba(255, 0, 0, 0.7);
    animation: popIn 1.5s ease-in-out;
}

@keyframes popIn {
    0% { transform: scale(0); opacity: 0; }
    100% { transform: scale(1); opacity: 1; }
}

	

@keyframes explode {
    0% { transform: scale(1); opacity: 1; }
    100% { transform: scale(10); opacity: 0; }
}
	#hearts-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    pointer-events: none; /* Сердечки не мешают кликам */
    z-index: -1; /* Помещаем слой под основное окно */
}

.heart {
    position: absolute;
    color: red;
    font-size: 24px;
    animation: fall linear infinite;
}

@keyframes fall {
    0% { transform: translateY(-100px); opacity: 1; }
    100% { transform: translateY(100vh); opacity: 0; }
}
	@keyframes fall {
    0% { transform: translateY(-100px); opacity: 1; }
    100% { transform: translateY(100vh); opacity: 0; }
}

.heart {
    position: absolute;
    color: red;
    font-size: 24px;
    animation: fall linear infinite;
} 
button {
    transition: 0.3s ease-in-out;
}

button:hover {
    transform: scale(1.1);
    box-shadow: 0 0 10px rgba(255, 77, 77, 0.8);
}
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            background: lavenderblush;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
			border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border: 5px solid HotPink;
        }
		h1 {
    opacity: 0;
    transform: translateY(-20px);
    animation: fadeIn 2s ease-in-out forwards;
}

@keyframes fadeIn {
    0% { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
}
        h1 {
    color: #ff4d4d; /* Основной цвет текста */
    text-shadow:  
        -2px -2px 0 #000,  
         2px -2px 0 #000,  
        -2px  2px 0 #000,  
         2px  2px 0 #000; /* Чёрная обводка вокруг текста */
    font-size: 28px;
    font-weight: bold;
	}
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            margin: 10px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #ccc;
        }
        button:hover {
            opacity: 0.8;
        }
        #loveMessage {
            display: none;
			}
    </style>
	
</head>
<body>
<audio autoplay loop>
    <source src="music.mp3" type="audio/mpeg">
</audio>
<div class="container" id="question1">
    <h1>Приветик Евочка! Есть очень важный вопрос, а ты меня любишь?❤️</h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(2)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<!-- Остальные вопросы (изначально скрыты) -->
<div class="container" id="question2" style="display: none;">
    <h1>Ты уверена? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(3)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question3" style="display: none;">
    <h1>А если подумать? </h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(4)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question4" style="display: none;">
    <h1>Ну точно-точно? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(5)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question5" style="display: none;">
    <h1>Это твоё окончательное решение? </h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(6)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question6" style="display: none;">
    <h1>Обещаешь? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(7)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question7" style="display: none;">
    <h1>Не передумаешь? </h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(8)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question8" style="display: none;">
    <h1>Уверена на 100%? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(9)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question9" style="display: none;">
    <h1>Это не шутка? </h1>
    <div class="buttons">
        <button class="yes" onclick="nextQuestion(10)">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<div class="container" id="question10" style="display: none;">
    <h1>Ты даёшь клятву? 💍</h1>
    <div class="buttons">
        <button class="yes" onclick="showLoveMessage()">Да</button>
        <button class="no" onclick="moveNoButton(this)">Нет</button>
    </div>
</div>

<!-- Экран с поздравлением (изначально скрыт) -->
 <div class="container" id="loveMessage"> <div class="love-card">
    ❤️ И я тебя люблю, Ева ❤️  
</div>
        <h1> Поздравляю с нашим днем! С Днём влюблённых! </h1>
    </div>
<div id="hiddenText" class="love-box" style="display: none;">
    <p class="love-message">  ❤️ Дорогая Ева,  
        <br><br>
        Ты – самое прекрасное, что есть в этом мире! 💖  
        Каждый день с тобой — это волшебство ✨,  
        каждая твоя улыбка — это счастье 😊.  
        <br><br>
        Ты наполняешь мой мир светом,  
        твоя доброта и нежность бесценны.  
        <br><br>
        Пусть наша любовь будет вечной,   
        <br><br>
        С тобой я хочу провести всю жизнь… 💍  
        <br><br>
        Я люблю тебя всем сердцем! ❤️  
   
Ты сделала меня самым счастливым. Принесла много ярких моментов в мою жизнь, спасибо тебе за все. Ты самая милая, добрая и красивая! Спасибо, что ты есть! 💖</p>
</div>
<div id="photoGallery" class="photo-gallery" style="display: none;">
    <div class="photo-row">
        <img src="photo1.jpg" alt="Фото 1" class="left-photo">
        <img src="photo2.jpg" alt="Фото 2" class="right-photo">
    </div>
    <div class="photo-row center">
        <img src="photo3.jpg" alt="Фото 3" class="bottom-photo">
    </div>
</div>

    <script>
        function showLoveMessage() {
            document.getElementById('questionContainer').style.display = 'none';
            document.getElementById('loveMessage').style.display = 'block';
        }

        function moveNoButton(button) {
    let x = Math.random() * (window.innerWidth - button.clientWidth);
    let y = Math.random() * (window.innerHeight - button.clientHeight);

    button.style.position = "absolute";
    button.style.transition = "0.2s ease-in-out"; 
    button.style.left = x + "px";
    button.style.top = y + "px";
}
    </script>

<script>
document.addEventListener("click", function(e) {
    let heart = document.createElement("div");
    heart.innerHTML = "❤️";
    heart.style.position = "absolute";
    heart.style.left = e.clientX + "px";
    heart.style.top = e.clientY + "px";
    heart.style.fontSize = "24px";
    heart.style.transition = "all 0.8s ease-out";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.style.transform = "translateY(-50px)";
        heart.style.opacity = "0";
    }, 100);

    setTimeout(() => heart.remove(), 1000);
});
</script>
<div id="hearts-container"></div>
<script>
    function createHeart() {
        const heart = document.createElement("div");
        heart.classList.add("heart");
        heart.innerHTML = "❤️";
        heart.style.left = Math.random() * 100 + "vw"; // Рандомная позиция по ширине
        heart.style.animationDuration = Math.random() * 2 + 3 + "s"; // Разная скорость
        document.getElementById("hearts-container").appendChild(heart);
        
        setTimeout(() => heart.remove(), 5000); // Удаление сердечка
    }
    
    setInterval(createHeart, 100); // Создание сердечек каждые 300 мс
</script>
<script>
function nextQuestion(num) {
    // Скрываем текущее окно
    let current = num - 1;
    document.getElementById("question" + current).style.display = "none";
    
    // Показываем следующее окно
    document.getElementById("question" + num).style.display = "block";
}

function showLoveMessage() {
    document.getElementById("question10").style.display = "none";
    document.getElementById("loveMessage").style.display = "block";
}

function moveNoButton(button) {
    let x = Math.random() * (window.innerWidth - button.clientWidth);
    let y = Math.random() * (window.innerHeight - button.clientHeight);

    button.style.position = "absolute";
    button.style.transition = "0.2s ease-in-out"; 
    button.style.left = x + "px";
    button.style.top = y + "px";
}
</script>
<script>
function showLoveMessage() {
    document.getElementById("question10").style.display = "none";
    document.getElementById("loveMessage").style.display = "block";

    // Показываем текст через 2 секунды (2000 мс)
    setTimeout(() => {
        document.getElementById("hiddenText").style.display = "block";
    }, 4000);
}

function moveNoButton(button) {
    let x = Math.random() * (window.innerWidth - button.clientWidth);
    let y = Math.random() * (window.innerHeight - button.clientHeight);

    button.style.position = "absolute";
    button.style.transition = "0.2s ease-in-out"; 
    button.style.left = x + "px";
    button.style.top = y + "px";
}

</script>
<script>
function showLoveMessage() {
    document.getElementById("question10").style.display = "none";
    document.getElementById("loveMessage").style.display = "block";

    // Показываем красивый текст через 2 секунды
    setTimeout(() => {
        document.getElementById("hiddenText").style.display = "block";
    }, 6000);

    // Показываем фото через 3 секунды
    setTimeout(() => {
        document.getElementById("photoGallery").style.display = "flex";
    }, 6000);
}

function moveNoButton(button) {
    let x = Math.random() * (window.innerWidth - button.clientWidth);
    let y = Math.random() * (window.innerHeight - button.clientHeight);

    button.style.position = "absolute";
    button.style.transition = "0.2s ease-in-out"; 
    button.style.left = x + "px";
    button.style.top = y + "px";
}
</script>

</body>
</html>
