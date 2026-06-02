<!DOCTYPE html>
<html lang="ru">
<head>
<!-- Yandex.Metrika counter -->
<script type="text/javascript">
    (function(m,e,t,r,i,k,a){
        m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
       m[i].l=1*new Date();
        for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
        k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)
    })(window, document,'script','https://mc.yandex.ru/metrika/tag.js?id=109598254', 'ym');

    ym(109598254, 'init', {ssr:true, webvisor:true, clickmap:true, ecommerce:"dataLayer", referrer: document.referrer, url: location.href, accurateTrackBounce:true, trackLinks:true});
</script>
<noscript><div><img src="https://mc.yandex.ru/watch/109598254" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter --> 

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DrayvMoto | Премиум мотосалон</title>
    <style>  
    * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #111;
            color: #eee;
            line-height: 1.6;
        }

        /* Header с изображением */
        header {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1568772585407-9361f9bf3a87?ixlib=rb-4.0.3&auto=format&fit=crop&w=2070&q=80');
            background-size: cover;
            background-position: center 40%;
            height: 85vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }

        header h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.3rem;
            max-width: 700px;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background-color: #e63946;
            color: white;
            padding: 12px 30px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            transition: transform 0.3s, background-color 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            background-color: #c1121f;
            transform: scale(1.05);
        }

        /* Навигация */
        nav {
            background-color: #1a1a1a;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            flex-wrap: wrap;
        }

        nav ul li a {
            display: block;
            padding: 15px 25px;
            color: #ddd;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s, background 0.3s;
        }

        nav ul li a:hover {
            background-color: #e63946;
            color: white;
        }

        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        section {
            margin-bottom: 60px;
            background: #1e1e1e;
            border-radius: 15px;
            padding: 40px 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            scroll-margin-top: 70px;
        }

        h2 {
            font-size: 2.2rem;
            margin-bottom: 30px;
            border-left: 5px solid #e63946;
            padding-left: 20px;
            color: #fff;
        }

        /* Карточки мотоциклов */
        .bike-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .bike-card {
            background: #2a2a2a;
            border-radius: 12px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .bike-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.5);
        }

        .bike-card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }

        .bike-info {
            padding: 20px;
        }

        .bike-info h3 {
            font-size: 1.6rem;
            margin-bottom: 10px;
        }

        .bike-specs {
            color: #bbb;
            margin: 10px 0;
            font-size: 0.9rem;
        }

        .price {
            font-size: 1.5rem;
            color: #e63946;
            font-weight: bold;
            margin: 15px 0;
        }

        .btn-small {
            background-color: #e63946;
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 30px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s;
        }

        .btn-small:hover {
            background-color: #c1121f;
        }

        /* Услуги сеткой */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .service-item {
            background: #2a2a2a;
            padding: 25px;
            text-align: center;
            border-radius: 12px;
            transition: all 0.3s;
        }

        .service-item:hover {
            background: #e63946;
            transform: scale(1.02);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 15px;
        }

        /* Акции */
        .offers-banner {
            background: linear-gradient(135deg, #e63946, #ff6b6b);
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            margin-top: 20px;
        }

        .offers-banner h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
        }

        /* Новости */
        .news-list {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .news-item {
            background: #2a2a2a;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #e63946;
        }

        .news-date {
            color: #e63946;
            font-size: 0.8rem;
            margin-bottom: 8px;
        }

        /* Форма тест-драйва */
        .testdrive-form {
            background: #2a2a2a;
            padding: 30px;
            border-radius: 15px;
            margin-top: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        input, select {
            width: 100%;
            padding: 12px;
            border-radius: 8px;
            border: 1px solid #444;
            background: #333;
            color: white;
            font-size: 1rem;
        }

        input:focus, select:focus {
            outline: none;
            border-color: #e63946;
        }

        .success-message {
            background: #2ecc71;
            color: white;
            padding: 12px;
            border-radius: 8px;
            margin-top: 20px;
            text-align: center;
            display: none;
        }

        /* Футер */
        footer {
            background: #0a0a0a;
            padding: 50px 20px 30px;
            margin-top: 60px;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
        }

        .footer-section h3 {
            margin-bottom: 20px;
            color: #e63946;
        }

        .footer-section p {
            margin-bottom: 10px;
            color: #aaa;
        }

        .social-links a {
            color: #ddd;
            margin-right: 15px;
            font-size: 1.5rem;
            text-decoration: none;
        }

        .copyright {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #222;
            color: #777;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            nav ul li a {
                padding: 10px 15px;
                font-size: 0.9rem;
            }
            section {
                padding: 25px 20px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>DrayvMoto</h1>
        <p>Скорость, стиль и свобода. Официальный дилер лучших мировых брендов.</p>
        <a href="#test-drive" class="btn">🔥 Записаться на тест-драйв</a>
    </header>

    <nav>
        <ul>
            <li><a href="#about">О нас</a></li>
            <li><a href="#bikes">Мотоциклы</a></li>
            <li><a href="#services">Услуги</a></li>
            <li><a href="#offers">Акции</a></li>
            <li><a href="#news">Новости</a></li>
            <li><a href="#contact">Контакты</a></li>
        </ul>
    </nav>

    <main>
        <section id="about">
            <h2>О нас</h2>
            <p>DrayvMoto — это не просто мотосалон, это место, где рождаются мечты о дорогах. Более 10 лет мы помогаем райдерам найти идеальный мотоцикл. Наши преимущества: гарантия качества, сертифицированные механики, тест-драйв любой модели и лучшие условия кредитования. Присоединяйтесь к семье DrayvMoto!</p>
        </section>

        <section id="bikes">
            <h2>🏍️ Наши мотоциклы</h2>
            <div class="bike-grid">
                <div class="bike-card">
                    <img src="https://images.unsplash.com/photo-1558981806-ec527fa84c39?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Спортбайк">
                    <div class="bike-info">
                        <h3>FireStorm X900</h3>
                        <div class="bike-specs">998 см³, 210 л.с., 199 кг</div>
                        <div class="price">₽1 450 000</div>
                        <button class="btn-small test-ride-btn" data-model="FireStorm X900">Записаться на тест</button>
                    </div>
                </div>
                <div class="bike-card">
                    <img src="https://images.unsplash.com/photo-1568772585407-9361f9bf3a87?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Круизер">
                    <div class="bike-info">
                        <h3>NightCruiser 1800</h3>
                        <div class="bike-specs">1832 см³, 95 л.с., 340 кг</div>
                        <div class="price">₽2 100 000</div>
                        <button class="btn-small test-ride-btn" data-model="NightCruiser 1800">Записаться на тест</button>
                    </div>
                </div>
                <div class="bike-card">
                    <img src="https://images.unsplash.com/photo-1631635589499-afd87d52bf64?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Эндуро">
                    <div class="bike-info">
                        <h3>Enduro Pro 701</h3>
                        <div class="bike-specs">692 см³, 75 л.с., 145 кг</div>
                        <div class="price">₽1 190 000</div>
                        <button class="btn-small test-ride-btn" data-model="Enduro Pro 701">Записаться на тест</button>
                    </div>
                </div>
                <div class="bike-card">
                    <img src="https://avatars.mds.yandex.net/get-autoru-vos/5232626/4c2b9fd1d3cdb0dfabd84dc551d70756/1200x900" alt="Туристический">
                    <div class="bike-info">
                        <h3>RoadGlide GT</h3>
                        <div class="bike-specs">1250 см³, 105 л.с., 280 кг</div>
                        <div class="price">₽2 250 000</div>
                        <button class="btn-small test-ride-btn" data-model="RoadGlide GT">Записаться на тест</button>
                    </div>
                </div>
            </div>
        </section>

        <section id="services">
            <h2>🛠️ Наши услуги</h2>
            <div class="services-grid">
                <div class="service-item">
                    <div class="service-icon">🔧</div>
                    <h3>Профессиональный ремонт</h3>
                    <p>Диагностика и ремонт любой сложности</p>
                </div>
                <div class="service-item">
                    <div class="service-icon">🛡️</div>
                    <h3>Тюнинг и стайлинг</h3>
                    <p>Индивидуальные доработки под ваш стиль</p>
                </div>
                <div class="service-item">
                    <div class="service-icon">📦</div>
                    <h3>Оригинальные запчасти</h3>
                    <p>Более 5000 наименований в наличии</p>
                </div>
                <div class="service-item">
                    <div class="service-icon">👕</div>
                    <h3>Экипировка и аксессуары</h3>
                    <p>Шлемы, куртки, перчатки премиум-брендов</p>
                </div>
            </div>
        </section>

        <section id="offers">
            <h2>🎁 Специальные предложения</h2>
            <div class="offers-banner">
                <h3>🔥 Скидка до 20% на все мотоциклы 2024 года!</h3>
                <p>При покупке в рассрочку 0% на 12 месяцев + бесплатное ТО-1 в подарок.</p>
                <p style="margin-top: 15px;">*Предложение действует до 31 декабря*</p>
            </div>
        </section>

        <section id="news">
            <h2>📰 Новости салона</h2>
            <div class="news-list">
                <div class="news-item">
                    <div class="news-date">15 ноября 2025</div>
                    <h3>Презентация нового FireStorm X900</h3>
                    <p>Ультрасовременный спортбайк с турбонаддувом. Приходите на тест-драйв в эти выходные!</p>
                </div>
                <div class="news-item">
                    <div class="news-date">5 ноября 2025</div>
                    <h3>Мотопарад DrayvMoto 2025</h3>
                    <p>Приглашаем всех райдеров на ежегодный мотопарад 20 ноября. Регистрация открыта!</p>
                </div>
                <div class="news-item">
                    <div class="news-date">28 октября 2025</div>
                    <h3>Новая услуга: выездной сервис</h3>
                    <p>Ремонтируем мотоциклы прямо у вас дома или в офисе. Удобно и быстро!</p>
                </div>
            </div>
        </section>

        <section id="test-drive">
            <h2>🏁 Запись на тест-драйв</h2>
            <p>Почувствуйте мощь и комфорт наших мотоциклов лично! Заполните форму, и наш менеджер свяжется с вами.</p>
            <div class="testdrive-form">
                <form id="testDriveForm">
                    <div class="form-group">
                        <label for="name">Ваше имя *</label>
                        <input type="text" id="name" required placeholder="Иван Петров">
                    </div>
                    <div class="form-group">
                        <label for="phone">Телефон *</label>
                        <input type="tel" id="phone" required placeholder="+7 (999) 123-45-67">
                    </div>
                    <div class="form-group">
                        <label for="model">Выберите модель *</label>
                        <select id="model" required>
                            <option value="">-- Выберите мотоцикл --</option>
                            <option value="FireStorm X900">FireStorm X900 (спорт)</option>
                            <option value="NightCruiser 1800">NightCruiser 1800 (круизер)</option>
                            <option value="Enduro Pro 701">Enduro Pro 701 (эндуро)</option>
                            <option value="RoadGlide GT">RoadGlide GT (туристический)</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="date">Удобная дата</label>
                        <input type="date" id="date">
                    </div>
                    <button type="submit" class="btn">📅 Записаться сейчас</button>
                    <div id="formSuccess" class="success-message">✅ Спасибо! Мы свяжемся с вами в ближайшее время для подтверждения тест-драйва.</div>
                </form>
            </div>
        </section>
    </main>

    <footer id="contact">
        <div class="footer-content">
            <div class="footer-section">
                <h3>DrayvMoto</h3>
                <p>Премиум мотосалон с 2014 года.</p>
                <p>Доверие и качество — наш девиз.</p>
            </div>
            <div class="footer-section">
                <h3>Контакты</h3>
                <p>📞 +7 (495) 777-88-99</p>
                <p>✉️ info@drayvmoto.ru</p>
                <p>📍 Москва, пр-т Мира, 125</p>
            </div>
            <div class="footer-section">
                <h3>Режим работы</h3>
                <p>Пн-Пт: 10:00 – 21:00</p>
                <p>Сб-Вс: 11:00 – 19:00</p>
            </div>
            <div class="footer-section">
                <h3>Мы в соцсетях</h3>
                <div class="social-links">
                    <a href="#">📘</a>
                    <a href="#">📸</a>
                    <a href="#">🎥</a>
                </div>
            </div>
        </div>
        <div class="copyright">
            © 2025 DrayvMoto. Все права защищены. Ваши мечты о дороге начинаются здесь.
        </div>
    </footer>

    <script>
        // Плавная прокрутка для навигационных ссылок
        document.querySelectorAll('nav a[href^="#"], header .btn[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const targetId = this.getAttribute('href');
                if (targetId === "#") return;
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    e.preventDefault();
                    targetElement.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Автоматическая подстановка модели мотоцикла в форму при клике на кнопки в карточках
        const testRideBtns = document.querySelectorAll('.test-ride-btn');
        const modelSelect = document.getElementById('model');
        
        testRideBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                const modelName = btn.getAttribute('data-model');
                if (modelSelect) {
                    for(let i = 0; i < modelSelect.options.length; i++) {
                        if(modelSelect.options[i].value === modelName) {
                            modelSelect.selectedIndex = i;
                            break;
                        }
                    }
                    document.getElementById('test-drive').scrollIntoView({
                        behavior: 'smooth',
                        block: 'center'
                    });
                }
            });
        });

        // Обработка отправки формы тест-драйва
        const form = document.getElementById('testDriveForm');
        const successDiv = document.getElementById('formSuccess');
        
        if (form) {
            form.addEventListener('submit', function(event) {
                event.preventDefault();
                
                const name = document.getElementById('name').value.trim();
                const phone = document.getElementById('phone').value.trim();
                const model = document.getElementById('model').value;
                
                if (!name || !phone || !model) {
                    alert('Пожалуйста, заполните все обязательные поля (*)');
                    return;
                }
                
                if (phone.length < 10) {
                    alert('Введите корректный номер телефона');
                    return;
                }
                
                successDiv.style.display = 'block';
                form.reset();
                
                setTimeout(() => {
                    successDiv.style.display = 'none';
                }, 5000);
                
                console.log('Заявка на тест-драйв DrayvMoto:', { name, phone, model });
            });
        }

        window.addEventListener('load', () => {
            document.body.style.opacity = '0';
            document.body.style.transition = 'opacity 0.5s';
            document.body.style.opacity = '1';
        });
    </script>
</body>
</html>
