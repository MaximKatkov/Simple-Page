<html>
 <head>
<meta name ="viewport" content="width=device-width,initial-scale=1">
 <style>
    #slides{
         position: relative;
          height: 30px; 
          padding: 10px;
          text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue; 
          top:60px; 
          left: 405px;
         
    }
    .slide{
         position: absolute;
          left: 0px;
           top: 0px; 
           width: 850px;
           height: 180px;
            opacity: 0; 
            z-index: 1;
             filter: drop-shadow(0 0 13px rgba(61, 244, 198, 0.5)); 
             -webkit-transition: opacity 1s;
              -moz-transition: opacity 1s;
               -o-transition: opacity 1s;
                transition: opacity 1s;
             }
             .showing{ 
                opacity: 1; 
                z-index: 2; 
            }
            .slide{ 
                box-sizing: border-box;
             }


body{
        margin:0;
        background-color:lightcyan;
    }
    .navbar{
        overflow: hidden;
        background-color: rgb(152, 226, 255);
        position: fixed;
        top:0;
        width: 100%;
    }
    .navbar a{
        float:left;
        margin-left:40px;
        display: block;
        color: blue;
        text-align:center;
        padding:14px 16 px;
        text-decoration:none;
        font-size:25px;
    }
    .navbar a:hover{
        background:cyan;
        color:black;
    }
    .topnav-right{
        float:right;
        margin-right: 40px;
    }
    .topnav-centre{
        float:left;
        margin-left:400px;

    }
    .main{
        text-decoration-color: #4CAF50;
        padding:25px;
        margin-top:30px;
        height:1500px;
    }
    .toc{
     padding:0 20px;
     background:#f0f0f0 ;
     display: inline-block;
    }
    

 </style>
 <script>
    window.onload = function () { 
        var slides = document.querySelectorAll('#slides .slide');
         var currentSlide = 0;
          var slideInterval = setInterval(nextSlide,2000); 
          function nextSlide() { 
            slides[currentSlide].className = 'slide';
             currentSlide = currentSlide + 1;
             if (slides.length == currentSlide) {
                 currentSlide = 0;
                 } 
                 slides[currentSlide].className = 'slide showing'; 
                } 
            }
 </script>
<script>
     $("[data-scroll]").on("click", function(event) {
        event.preventDefault();

        var $this = $(this),
            blockId = $this.data('scroll'),
            blockOffset = $(blockId).offset().top;

        $("#nav a").removeClass("active")
        $this.addClass("active");

        $("html, body").animate({
            scrollTop: blockOffset
        }, 500);
    });
</script>
</head>   
<body>

    <div class="navbar">

        <a href="contact" data-scroll="#footer">Contact</a>

        <div class="topnav-right">
            <p><a href="#top3">Photo</a></p>
        </div>
        <div class="topnav-centre">
            <p><a href="#top1">Home</a></p>
            
        </div>

    </div>

    <div id="slides" >
         <img src="c:/images/t1.jpg" class="slide showing"> 
         <img src="c:/images/t2.jpg" class="slide ">
          <img src="c:/images/t3.jpg" class="slide "> 
        </div>
    <div class="main">
        <p><a name="top1"></a></p>
        <h1>Отдых на море в России</h1>
        <h2>Популярные курорты страны</h2>
        <p>Сочи</p>
        <p>Город Сочи расположился на Северо-Восточном побережье моря. Курортный город находится за 1700 километров от столицы страны. 
           <p> Город принято считать курортной столицей России, расположенной на побережье Черного моря.</p>
            <p>Туристы, посетившие город, могут пойти в Летний театр, в Сочинский цирк, позагорать на центральных пляжах или заняться дайвингом.</p>
            <p>Анапа</p>
            <p>Город Анапа удачно располагается на юге России. Это административный центр муниципального образования и знаменитый курорт.</p>
               <p> До столицы страны, от этого города, начисляется 1530 километров. Здесь средиземноморский климат и практически никогда нет сильных морозов.</p>
                <p>В городе можно посетить два театра, 29 общедоступных библиотек и археологический музей под открытым небом.</p>
                <p>В городе много гостиниц на любой вкус и кошелек. Здесь есть дельфинарий и заповедник.</p>
                <p>Судак</p>
               <p> Город Судак располагается в восточном Крыму. На побережье Черного моря, которое располагается возле города, каждый год много отдыхающих.</p>
                <p>Здесь можно хорошо загореть и попробовать самые лучшие вина. В городе есть исторический музей, винодельческие предприятия, архитектурные памятки 19 века.</p>
                    <p> Здесь располагается знаменитая Кипарисовая алея, которая просто поражает своей красотой.</p>
                        <p> В городе есть несколько храмов, некоторые из них относятся к старинным памяткам архитектуры, можно посетить лютеранскую кирху. </p>
                            <p> Здесь открываются очень хорошие пейзажи и всегда можно обустроиться в комфортном отеле, расположенном недалеко от пляжной зоны.</p>
                                <p> Также, желающие могут посетить довольно привлекательный городской аквапарк.</p>
          <h2>Курорт Вашей Мечты</h2>                      
    <p><a name="top3"></a></p>
    <div class="about">
        <div class="about__item">
            <div class="about__img">
                <img src="c:/images/a1.jpg" alt="">
            </div>
            <div class="about__text">CОЧИ</div>
        </div>
        <div class="about__item">
            <div class="about__img">
                <img src="c:/images/a2.jpg" alt="">
            </div>
            <div class="about__text">АНАПА</div>
        </div>
        <div class="about__item">
            <div class="about__img">
                <img src="c:/images/a3.jpg" alt="">
            </div>
            <div class="about__text">ГЕЛЕНДЖИК</div>
        </div>
    </div>
    <p><a name="top2"></a></p>
    <h2>Сервис обслуживания</h2>
    <p>Список гостиниц насчитывает более 1000 разнообразных вариантов из которых вы можете сделать выбор опираясь на свои предпочтения.</p>
       <p>  Используя фильтрацию, в несколько кликов можно найти идеально подходящий объект размещения, который будет подходить именно вам. </p>
        <p> Мы ценим каждого клиента, своевременно обрабатываем заявки и не заставляем ждать. Услуги бесплатны, что является немалозначимым фактором. </p>
         <p>Бронируйте с нами и получайте скидки.</p>
         <h2>Список лучших отелей </h2>
         <p>Гранд Прибой (бывш. «Ателика Гранд Прибой)</p>
            <p> Отель Prometey Club 4* (Сочи, Лазаревское)</p>
                <p>Отель Ribera Resort & SPA 4* (Крым, г. Евпатория)</p>
                    <p>Отель Ателика Гранд Босфор (г. Туапсе)</p>
                        <p>Отель Ателика Небуг (г. Туапсе)</p>
                            <p>Отель Гамма 4-5* (г. Туапсе)</p>
                                <p> Отель Джемете (г. Анапа)</p>
                                    <p>Отель Ривьера Клуб 4* (г. Анапа)</p>
</div>
<div class="section" id="footer">
    <div class="container">
        <div class="section__header">
            <h3 class="section__suptitle">Бронирование Горячей Путёвки</h3>
            <p><a name="top4"></a></p>
            <h2 class="section__title">Контакты Агентства</h2>
        </div>

        <div class="contacts">
            <div class="contacts__left">
                <h4 class="contact__title">Вы можете связаться с нами,написав сообщение на почту,указанную ниже.</h4>
                <div class="contact__subtitle"> Данные Агента:</div>

                <ul class="contact__info">  
                    <li class="contact__info-item">
                        <img class="contact__info-icon" src="assets/Images/contacts/phone.png" alt="">
                        8(905)-575-55-95
                    </li>
                    <li class="contact__info-item">
                        <img class="contact__info-icon" src="assets/Images/contacts/mail.png" alt="">
                        mmkatkov355@gmail.com
                    </li>
                </ul>

                <div>
                    <form  class="form" action="/" method="post">
                        <div class="form__group">
                            <label class="form__label" for="input-email">Адресс почтового ящика:</label>
                            <input class="form__input" type="text" id="input-email" placeholder="mmkatkov355@gmail.com">
                        </div>

                        <div class="form__group">
                            <label class="form__label" for="input-text">Заполните следующию анкету и агент свяжется с вами</label>
                            <textarea class="form__textarea" name="input-text" id="input-text" placeholder="Введите сообщение"></textarea>
                        </div>

                        <div class="text__right">
                            <button class="send__button" type="submit">Отправить</button>
                        </div>
                    </form>
                </div>

            </div>
        </div>

</div>
<h2>Закладки страницы:</h2>
<p><a href="#top1">Описание Курортов</a></p>
<p><a href="#top3">Фотографии Курортов</a></p>
<p><a href="#top2">Сервис Обслуживания</a></p>
<p><a href="#top4">Контактная информация</a></p>
<div id="demo">
</div>
<button onclick="getElementById('demo').innerHTML = Date()">Узнать Время</button>
<p>

    
</p>
<div class="copyright">
    2022 © The Resort
 </div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>
<script src="c:/File/app.js"></script>
</body>

    <style>
        img{
            display:block;
            margin-top: 500px;
            margin:10px;
            border:1px solid green;
            padding: 0.5em;
            border-radius:1rem;
            box-shadow:3px 3px 8px 0px rgba(0,0,0,0.3);
            max-width: 20vw;
        }
        .button {
             background-color: #4CAF50;
             border: none; 
             color: white; 
             padding: 15px 32px; 
             text-align: center;
             text-decoration: none;
             display: inline-block;
             font-size: 12px; 
             border-radius: 16px;
             transition-duration: 0.4s;
             cursor: pointer;
             box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
        }
        .button:hover {
             background-color: red; color: white;
             }
        .styled-table {
             border-collapse: collapse; 
             box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
             width: 60%;
             border-spacing: 0px;
         }
         .styled-table img{ 
            width: 15vw;
             height: 10vw; 
        }
        td{ 
            padding: 10px 2px 2px 5px ;
         }
         #demo {
             font-family: "Sofia", sans-serif; font-size: 30px; color: blue;
             }
         td[colspan="3"] {
        text-align: center;
         }

         .container{
      width: 100%;
      max-width: 1200px;
      margin: 0 auto;
     }

         .intro{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    height: 100vh;

    background:
    url('../Images/intro.jpg') center no-repeat;
    background-size: cover;
}

.intro__inner{
    width: 100%;
    max-width: 880px;
    margin: 0 auto;

    text-align:center;
}

.intro__title{
    color: #fff;
    font-size: 100px;
    font-weight: 600;
    text-transform: uppercase;
    line-height: 1;
}

.intro__title:after{    
    content: "";
    display: block;
    width: 60px;
    height: 3px;
    margin: 40px auto 40px;

    background-color: rgb(22, 35, 218);
}

.intro__suptitle{
    margin-bottom: 20px;
    /*  font-family: 'Kaushan Script', cursive; */
    font-family: 'Pacifico', cursive;
    font-size: 52px;
    color: rgb(24, 21, 231);
}
.header{
    width: 100%;
    padding-top: 30px;
    margin-top: 17px;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
}

.header.fixed{
    padding: 10px 0;

    background-color: #42b4ec;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
    margin-top: 17px;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;

    transform: translate3d(0, 0, 0);
}

.header.active{ 
    background-color: #40c4ec;
}

.header__inner{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 17px;
}

.header__logo{
    font-size: 15px;
    font-weight: 1000;
    width: 800px; ;
    margin-top: 17px;
    color: #fff;
}

.nav{
    font-size: 14px;
    text-transform: uppercase;
}

.nav__link{
    display: inline_block;
    vertical-align: top;
    margin: 0 15px;
    position: relative;

    color: #fff;
    text-decoration: none;

    transition: color .1s linear;
}

.nav__link:after{
    content: "";
    display: block;
    width: 100%;
    height: 3px;

    background-color: #33e5f9;
    opacity: 0;

    position: absolute;
    top: 100%;
    left: 0;
    z-index: 1;

    transition: opacity .1s linear
}

.nav__link:hover {
    color: #21aaf9;
}

.nav__link:hover:after, 
.nav__link.active:after{
    opacity: 1;
}

.nav__link.active{
    color: #22acf6;
}
.button{
    display: inline-block;
    vertical-align: top;
    padding: 8px 30px;
    
    border: 3px solid #fff;

    font-size: 13px;
    font-weight: 700;
    color: #fff;
    text-transform: uppercase;
    text-decoration: none;

    transition: .1s linear, color .1s linear;
}

.button:hover{
    background-color: #fff;
    color: #333;
}

.send__button{
    display: inline-block;
    vertical-align: top;
    padding: 8px 30px;
    margin-bottom: 20px;

    border: 2px solid #2dfafa;
    border-radius: 1.8rem;
    background: none;
    cursor: pointer;

    font-size: 13px;
    font-weight: 700;
    color: #2985f5;
    text-transform: uppercase;
    text-decoration: none;
    
    transition: .1s linear, color .1s linear;
}

.send__button:hover{
    background-color: #fff;
    color: #2585e4;
}

.slider{
    width: 100%;

    position: absolute;
    bottom: 0;
    left: 0;
    z-index: 1;
}

.slider__inner{
    display: flex;
    justify-content: space-between;
}

.slider__item{
    width:23%;
    padding: 20px 0;
    position: relative;

    border-top: 2px solid #fff;
    opacity: .7;

    font-size: 18px;
    color: #fff;
    text-transform: uppercase;

}

.slider__item.active{
    opacity: 1;
}

.slider__item.active:before{
    content: "";
    display: block;
    width: 70px;
    height: 3px;

    background-color: #29f4fe;

    position: absolute;
    top: -3px;
    left: 0;
    z-index: 1;
}
.section{
    background-color: #fff;
    padding: 80px 0;
}

.section--portfolio{
    background: url(../Images/Portfolio.jpg), center no-repeat;
    background-size: cover;
}

.section__header{
    width: 100%;
    max-width: 950px;
    margin: 0 auto 40px;
    text-align: center;
}

.section__suptitle{
    font-family: 'Anton',sons-serif;
    font-size: 21px;
    color: #333;
}

.section__title{
    font-size: 30px;
    font-weight: 700;
    color: #333;
    text-transform: uppercase;
}

.section__title:after{
    content: "";
    display: block;
    width: 60px;
    height: 3px;
    margin: 30px auto;
    background-color: #248aff;
}

.section__text{
    color: #999;
    font-size: 15px;
}
.contact{
    display: flex;
}

.contact__left{
    width: 48%;
    padding: 2rem;
}

.contact__right{
    width: 52%;
    background: url(../Images/QR.jpg), center no-repeat;

}

.contact__title{
    font-size: 21px;
    text-transform: uppercase;
    color: #333;
    font-weight: 700;
}

.contact__subtitle{
    font-size: 15px;
    color: #333;
}

.contact__info{
    margin: 1rem 0 1rem;
    padding: 0;
    list-style: none;
}

.contact__info-item{
    display: flex;
    align-items: center;
    margin-bottom: 0.5rem;
}

.contact__info-icon{
    margin-right: 0.5rem;
}
.copyright{
    padding: 20px 0;

    border-top: 1px solid rgb(39, 133, 240);

    font-size: 14px;
    color: #333;
    text-align: center;
}
.about{
    display: flex;
    justify-content: space-between;
}

.about__item{
    width: 380px;
    background-color: rgba(143, 229, 236, 0.606);
    position: relative;
    margin-top: 50px;
    
}

.about__item:hover .about__img{
    transform: translate3d(-10px, -10px, );
}

.about__item:hover .about__img img{
    opacity: .1;
}

.about__item:hover .about__text{
    opacity: 1;
}

.about__img{
    background: linear-gradient(to bottom, rgb(166, 240, 229), #c8f2e0);

    transition: transform .2s linear;
}

.about__img img{
    display: block;
    transition: opacity .1s linear;
}

.about__text{
    width: 100%;

    font-size: 18px;
    color: rgb(82, 87, 226);
    text-transform: uppercase;
    font-weight: 700;
    text-align: center;
    opacity: 0;

    position: absolute;
    top: 38%;
    left: 0;
    z-index: 2;
    transform: translate3d(0, 38%, 0);

    transition: opacity .1s linear;
}

 .portfolio{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.portfolio__item{
    width: 32.33333333333333333333%;
    border-bottom: 4px solid #dadada;
}

.portfolio__item img{
    width: auto;
    display: block;
}
.form__label{
    display: inline-block;
    margin-bottom: .6rem;
    font-size: 1rem;
    color: rgb(34, 108, 235);
    font-weight: 700;
}

.form__input, .form__textarea{
    display: block;
    width: 50%;

    padding: 14px 20px;

    border: 1px solid rgb(46, 241, 255);
    border-radius: 1.8rem;

    font-family: 'Pacifico', cursive;
    font-size: 0.8rem;
    line-height: 1.2;
    font-weight: 400;
}

.form__group{
    margin-bottom: 2.7rem; 
}

.form__textarea{
    height: 200px;
    resize: none;
}
    </style>


</html>
