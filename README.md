<
<!DOCTYPE html>
<html lang="ro">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Proiect Gaming - Angelescu Nicolae Antonio</title>
</head>
<body>
<!-- Header și navigare -->
<header>
<nav>
<ul>
<li><a href="#home">Acasă</a></li>
<li><a href="#gallery">Galerie</a></li>
<li><a href="#about">Despre</a></li>
<li><a href="#contact">Contact</a></li>
<li><a href="https://www.youtube.com" target="_blank">Videoclipuri</a></li>
<li><a href="https://www.example.com" target="_blank">Resurse</a></li>
</ul>
</nav>
</header>
<!-- Pagina de Acasă -->
<section id="home">
<h1>Bine ai venit la proiectul meu de gaming!</h1>
<p>Acesta este un site dedicat tematicii gaming, creat de <strong>Angelescu Nicolae Antonio</br>Grupa 50319, Anul III, Facultatea de Informatică Economică -
UPG Ploiești</strong>.</p>
</section>
<!-- Pagina Galerie -->
<section id="gallery">
<h1>Galerie</h1>
<div class="carousel">
<!-- Imagini carusel -->
<img src="https://cdn.cloudflare.steamstatic.com/steam/apps/70/capsule_616x353.jpg?t=1671593433" alt="League of Legends" class="carouselslide" style="width:100%; display:block;">
<img src="https://i.pinimg.com/originals/ab/60/97/ab609786d5b774a130e8a57f23a44fbe.jpg" alt="Valorant" class="carousel-slide" style="width:100%; display:none;">
<img src="https://cdn2.unrealengine.com/valorant-v1-1920x1080-0c5b315dbd04.jpg" alt="Joc gaming" class="carousel-slide" style="width:100%; display:none;">
</div>
<button onclick="moveSlide(-1)">&#10094; Înapoi</button>
<button onclick="moveSlide(1)">Înainte &#10095;</button>
</section>
<!-- Pagina Despre -->
<section id="about">
<h1>Despre Proiect</h1>
<p>Acest proiect a fost realizat pentru a prezenta tehnologiile web în contextul jocurilor video. Am utilizat HTML, CSS și JavaScript pentru a construi acest site.</p>
</section>
<!-- Pagina Contact -->
<section id="contact">
<h1>Contact</h1>
<p>Poți să mă contactezi la adresa de e-mail: <strong>tony.angelescu@gmail.com</strong></p>
<h2>Formular de contact</h2>
<form action="mailto:tony.angelescu@gmail.com" method="post" enctype="text/plain">
<label for="name">Numele tău:</label><br>
<input type="text" id="name" name="name" required><br><br>
<label for="email">E-mail:</label><br>
<input type="email" id="email" name="email" required><br><br>
<label for="message">Mesaj:</label><br>
<textarea id="message" name="message" rows="4" required></textarea><br><br>
<input type="submit" value="Trimite">
<input type="reset" value="Resetează">
</form>
<h2>Harta Universității de Petrol și Gaze Ploiești</h2>
<iframe src="https://www.google.com/maps/embed/v1/place?
key=AIzaSyAbpHDLfnu8JoWGCmdfzI0obIUw3EE35I0&q=Universitatea+de+Petrol+și+Gaze+Ploiești" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen=
hidden="false" tabindex="0"></iframe>
</section>
<!-- Footer -->
<footer>
<p>&copy; 2025 Angelescu Nicolae Antonio - Proiect Gaming</p>
</footer>
<!-- Script JavaScript pentru carusel -->
<script>
let slideIndex = 0;
function showSlides() {
let slides = document.querySelectorAll('.carousel-slide');
for (let i = 0; i < slides.length; i++) {
slides[i].style.display = 'none';
}
slideIndex++;
if (slideIndex > slides.length) {slideIndex = 1}
slides[slideIndex-1].style.display = 'block';
}
function moveSlide(n) {
slideIndex += n;
if (slideIndex < 1) { slideIndex = document.querySelectorAll('.carousel-slide').length }
showSlides();
}
setInterval(showSlides, 3000); // Încărcare automată la fiecare 3 secunde
showSlides(); // Pornire carusel
</script>
</body>
</html>
