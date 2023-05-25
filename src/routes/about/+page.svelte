<title>Обо мне</title>

	<article class="article">
	<h1> &#9785; <font face="Franklin Gothic">Стрнаица обо мне.</font> &#9785; </h1>

	<blockquote>
		<p> &#10084; Я - Федорова Арина. Учусь в 10 классе. Я живу в Ижевске. На этой странице я хотела бы Вам рассказать о себе и о своих увлечениях, хобби. Добро пожаловать на мой сайт! &#10084;</p>
        </blockquote>
	<blockquote>
		<p>Иже́вск — двадцать первый по численности населения город Российской Федерации, крупный промышленный, торговый, научно-образовательный и культурный центр Поволжья и Предуралья, столица Удмуртской Республики. Образует городской округ город Ижевск.
Знаменит оборонным и машиностроительным производствами. Носит неофициальное звание «оружейной столицы» Российской Федерации, и звание города трудовой славы.</p>
		
		<div class="blockquote-author-image" style="--image: url('https://sun9-east.userapi.com/sun9-33/s/v1/if1/4VL0i0MHS9Nz6N3imQj5aJTP6k6n_mdcHTgND-y05bmOledL97WAUUPCmsWnfIwnaLVILA.jpg?size=1600x1200&quality=96&type=album')"> </div>
   </blockquote>
	
        <p><font face="Century gothic">Теперь я расскажу Вам о своем хобби.</font></p>
	
	<blockquote>
        <p>Мое хобби-это чтение. Я очень люблю читать различные произведения. Больше всего я люблю читать кассику.<p>
		<div class="blockquote-author-image" style="--image: url('https://pravlife.org/sites/default/files/field/image/2021.09.29/istock-167162510.jpg.jpg')">
		</div>
        </blockquote>
          <p><font face="Century gothic">Также я увекаюсь спортом.</font></p>
          <blockquote>
		<p>Я очень люблю бегать и заниматься спортом, развиваться в данном направлении.</p>
		
		<div class="blockquote-author-image" style="--image: url('https://lorikel.ru/wp-content/uploads/2021/02/kak-dyshat-pri-bege.jpg-2.jpg')"> </div>
   </blockquote>
    </article>
    <style>

:root {
	--type-body: Open Sans, Helvetica, Arial, sans-serif;
	--type-quote: Vollkorn;
	--quote-image-width: 140px;
	--border-rad: 7px;
	--accent-color: hsl(322deg 100% 90%);
	--quote-bg: hsl(0 0% 97%);
}


*,
*::before,
*::after {
	box-sizing: border-box;
}

a {
	text-decoration: none;
	color: var(--accent-color);
}

a:hover,
a:focus {
	text-decoration: underline;
}

body {
	margin: 15px 10px;
	font-family: var(--type-body);
	color: hsl(0 0% 15%);
    background-color: #FFE4E1;
}

.article {
	max-width: 900px;
	margin: auto;
}

h1 {
	width: max-content;
	margin: 0 auto 1.8em;
	box-shadow:
		0 2px 0 var(--accent-color),
		0 4px 0 white,
		0 6px 0 var(--accent-color);
	font: 1.4rem var(--type-quote);
	color: hsl(0 0% 25%);
    font: 'Bookman old style';
}
 
blockquote {
	position: relative;
	margin: 40px 0;
	padding: 1.6em 2.4em .7em calc(1.4em + var(--quote-image-width));
	font: italic 1.2rem var(--type-quote);
	background: var(--quote-bg) no-repeat left / var(--quote-image-width);
	border-radius: var(--border-rad);
	border: 2px solid white;
	box-shadow: 2px 2px 4px hsl(0 0% 0% / 20%);
	text-indent: 1.6em;
}

@media (min-width: 768px) {
	blockquote {
		margin: 40px 60px;
	}
}

blockquote::before {
	content: "";
	pointer-events: none;
	position: absolute;
	z-index: 1;
	left: 0;
	top: 0;
	right: 0;
	bottom: 0;
	border-radius: var(--border-rad);
	box-shadow:
		inset -2px -2px 1px hsl(0 0% 100%),
		inset 2px 2px 4px hsl(0 0% 0% / 20%);
}

blockquote::after {
	content: "❝";
	position: absolute;
	z-index: 1;
	left: 50%;
	top: -2px;
	transform: translate(-50%, -50%);
	width: 1.3em;
	height: 1.3em;
	background: white;
	box-shadow: 0 4px 5px -1px hsla(0 0% 0% / 20%);
	border-radius: 999px;
	display: grid;
	place-content: center;
	padding-top: .5em;
	color: var(--accent-color);
	font-size: 36px;
	font-style: normal;
	text-indent: 0;
}

.blockquote-author-image {
	position: absolute;
	left: 0;
	top: 0;
	width: var(--quote-image-width);
	height: 100%;
	opacity: 0.75;
	background: var(--accent-color) var(--image) no-repeat center / cover;
	background-blend-mode: hard-light;
	border-top-left-radius: var(--border-rad);
	border-bottom-left-radius: var(--border-rad);
}

cite {
	display: block;
	margin-top: 30px;
	text-indent: 0;
	text-align: center;
	font: bold .9rem var(--type-body);
	text-transform: uppercase;
	color: hsl(0 0% 20%);
}

@media (min-width: 768px) {
	cite {
		margin-left: calc(1rem - var(--quote-image-width));
	}
}

.cite-last-name {
	background: var(--accent-color);
	color: var(--quote-bg);
}





.controls {
	position: fixed;
	bottom: 10px;
	right: 10px;
	font-size: 0.8em;
	opacity: 0.7;
	transition: .2s;
}

.controls:hover,
.controls:focus {
	opacity: 1;
}

.controls label {
	font-weight: bold;
	text-transform: lowercase;
}

.controls input {
	display: block;
	width: 100%;
	border: 0;
	outline: none;
	padding: 0;
}
    </style>