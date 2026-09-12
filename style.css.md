```css
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap');

:root {
    --dark: #17130f;
    --brown: #6f4228;
    --light-brown: #a66a3f;
    --cream: #f5efe7;
    --white: #ffffff;
    --text: #403a35;
    --border: #ded4c8;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "DM Sans", sans-serif;
    color: var(--text);
    background: var(--white);
    line-height: 1.7;
}

h1,
h2,
h3 {
    font-family: "Playfair Display", serif;
}

a {
    text-decoration: none;
    color: inherit;
}


/* NAVBAR */

.navbar {
    height: 82px;
    padding: 0 7%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: rgba(255,255,255,0.96);
    position: sticky;
    top: 0;
    z-index: 1000;
    border-bottom: 1px solid #eee;
}

.logo {
    display: flex;
    align-items: center;
    gap: 12px;
}

.logo > span {
    width: 43px;
    height: 43px;
    background: var(--dark);
    color: #fff;
    display: grid;
    place-items: center;
    font-family: "Playfair Display", serif;
    font-size: 18px;
}

.logo strong {
    display: block;
    font-family: "Playfair Display", serif;
    font-size: 19px;
    color: var(--dark);
}

.logo small {
    display: block;
    font-size: 10px;
    letter-spacing: 2px;
    text-transform: uppercase;
}

nav {
    display: flex;
    gap: 35px;
}

nav a {
    font-size: 14px;
    font-weight: 600;
}

nav a:hover {
    color: var(--brown);
}

.menu-btn {
    display: none;
    border: none;
    background: none;
    font-size: 25px;
}


/* HERO */

.hero {
    min-height: 90vh;
    display: flex;
    align-items: center;
    padding: 100px 8%;
    background:
        linear-gradient(90deg, rgba(15,10,7,.86), rgba(15,10,7,.35)),
        url("images/hero.jpg") center/cover;
    color: white;
}

.hero-content {
    max-width: 760px;
}

.tagline,
.section-label {
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 3px;
    color: var(--light-brown);
    margin-bottom: 15px;
}

.hero .tagline {
    color: #e0ad83;
}

.hero h1 {
    font-size: clamp(48px, 7vw, 85px);
    line-height: 1.08;
    margin-bottom: 25px;
}

.hero h1 span,
h2 span {
    color: var(--light-brown);
}

.hero-text {
    max-width: 600px;
    font-size: 18px;
    color: #eee;
    margin-bottom: 35px;
}

.hero-buttons {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
}

.btn {
    display: inline-block;
    padding: 14px 26px;
    border: 1px solid transparent;
    font-weight: 700;
    font-size: 14px;
    cursor: pointer;
    transition: .3s;
}

.primary {
    background: var(--brown);
    color: white;
}

.primary:hover {
    background: var(--light-brown);
    transform: translateY(-2px);
}

.secondary {
    border-color: white;
    color: white;
}

.secondary:hover {
    background: white;
    color: var(--dark);
}


/* GENERAL SECTIONS */

.section {
    padding: 110px 8%;
}

.section-heading {
    max-width: 700px;
    margin: 0 auto 55px;
    text-align: center;
}

.section-heading h2,
.section-content h2,
.why-us h2,
.cta h2 {
    font-size: clamp(38px, 5vw, 58px);
    line-height: 1.15;
    margin-bottom: 20px;
}

.section-heading > p:last-child {
    color: #777;
}


/* ABOUT */

.about {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
    align-items: center;
}

.section-image {
    min-height: 580px;
    background:
        url("images/about.jpg") center/cover;
}

.section-content > p:not(.section-label) {
    margin-bottom: 18px;
    color: #666;
}

.features {
    display: flex;
    gap: 40px;
    margin-top: 35px;
    flex-wrap: wrap;
}

.features strong {
    display: block;
    font-family: "Playfair Display", serif;
    font-size: 32px;
    color: var(--brown);
}

.features span {
    font-size: 12px;
    color: #777;
}


/* SERVICES */

.services {
    background: var(--cream);
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.service-card {
    background: white;
    padding: 35px;
    border: 1px solid #e7ded5;
    transition: .3s;
}

.service-card:hover {
    transform: translateY(-7px);
    box-shadow: 0 15px 35px rgba(50,30,15,.1);
}

.service-icon {
    font-size: 35px;
    margin-bottom: 20px;
}

.service-card h3 {
    font-size: 25px;
    margin-bottom: 10px;
    color: var(--dark);
}

.service-card p {
    color: #777;
    font-size: 14px;
}


/* WHY US */

.why-us {
    padding: 100px 8%;
    background: var(--dark);
    color: white;
    display: grid;
    grid-template-columns: .8fr 1.2fr;
    gap: 90px;
    align-items: center;
}

.why-us > div:first-child > p:last-child {
    color: #aaa;
    max-width: 450px;
}

.why-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 45px;
}

.why-grid span {
    color: #b9825b;
    font-size: 12px;
}

.why-grid h3 {
    font-size: 22px;
    margin: 8px 0;
}

.why-grid p {
    color: #aaa;
    font-size: 14px;
}


/* GALLERY */

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
}

.gallery-item {
    height: 330px;
    position: relative;
    overflow: hidden;
    background: #ddd;
}

.gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: .5s;
}

.gallery-item:hover img {
    transform: scale(1.08);
}

.gallery-overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    padding: 25px;
    color: white;
    background: linear-gradient(transparent, rgba(0,0,0,.8));
}

.gallery-overlay h3 {
    font-size: 23px;
}

.gallery-overlay p {
    font-size: 12px;
}


/* CTA */

.cta {
    padding: 80px 8%;
    background: var(--cream);
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 30px;
}

.cta h2 {
    margin-bottom: 10px;
}

.cta p:not(.section-label) {
    color: #777;
}


/* CONTACT */

.contact {
    background: white;
}

.contact-grid {
    max-width: 1100px;
    margin: auto;
    display: grid;
    grid-template-columns: .8fr 1.2fr;
    gap: 70px;
}

.contact-info {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.contact-box {
    display: flex;
    gap: 15px;
    align-items: flex-start;
}

.contact-box > span {
    font-size: 23px;
}

.contact-box small {
    font-size: 10px;
    letter-spacing: 2px;
    font-weight: bold;
    color: #999;
}

.contact-box a {
    display: block;
    font-weight: 600;
    color: var(--brown);
}

.contact-box p {
    margin: 0;
}


.contact-form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.contact-form input,
.contact-form select,
.contact-form textarea {
    width: 100%;
    padding: 15px;
    border: 1px solid var(--border);
    outline: none;
    font-family: inherit;
    font-size: 14px;
}

.contact-form input:focus,
.contact-form select:focus,
.contact-form textarea:focus {
    border-color: var(--brown);
}

.contact-form button {
    border: none;
}


/* FOOTER */

footer {
    padding: 40px 8%;
    background: #0f0d0b;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
}

.footer-logo strong {
    display: block;
    font-family: "Playfair Display", serif;
    font-size: 20px;
}

.footer-logo span {
    font-size: 11px;
    letter-spacing: 2px;
    color: #999;
}

footer p {
    color: #888;
    font-size: 12px;
}


/* WHATSAPP */

.whatsapp {
    position: fixed;
    right: 22px;
    bottom: 22px;
    width: 58px;
    height: 58px;
    border-radius: 50%;
    background: #25D366;
    color: white;
    display: grid;
    place-items: center;
    font-size: 27px;
    z-index: 999;
    box-shadow: 0 5px 20px rgba(0,0,0,.25);
}


/* MOBILE */

@media (max-width: 900px) {

    nav {
        position: absolute;
        top: 82px;
        left: 0;
        right: 0;
        background: white;
        display: none;
        flex-direction: column;
        padding: 25px 8%;
        gap: 20px;
        box-shadow: 0 10px 25px rgba(0,0,0,.08);
    }

    nav.active {
        display: flex;
    }

    .menu-btn {
        display: block;
    }

    .about,
    .why-us,
    .contact-grid {
        grid-template-columns: 1fr;
    }

    .why-us {
        gap: 50px;
    }

    .service-grid,
    .gallery-grid {
        grid-template-columns: 1fr 1fr;
    }

    .cta {
        flex-direction: column;
        align-items: flex-start;
    }
}


@media (max-width: 600px) {

    .navbar {
        padding: 0 5%;
    }

    .hero {
        padding: 80px 6%;
        min-height: 85vh;
    }

    .hero h1 {
        font-size: 48px;
    }

    .hero-text {
        font-size: 16px;
    }

    .section {
        padding: 75px 6%;
    }

    .service-grid,
    .gallery-grid,
    .why-grid {
        grid-template-columns: 1fr;
    }

    .section-image {
        min-height: 400px;
    }

    .features {
        gap: 25px;
    }

    footer {
        flex-direction: column;
        align-items: flex-start;
    }

    .gallery-item {
        height: 280px;
    }
}
```