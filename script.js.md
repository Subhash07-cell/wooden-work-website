```javascript
// MOBILE MENU

function toggleMenu() {
    const nav = document.getElementById("navMenu");
    nav.classList.toggle("active");
}


// CLOSE MOBILE MENU AFTER CLICK

document.querySelectorAll("#navMenu a").forEach(link => {
    link.addEventListener("click", () => {
        document.getElementById("navMenu").classList.remove("active");
    });
});


// WHATSAPP ENQUIRY FORM

function sendWhatsApp(event) {

    event.preventDefault();

    const name = document.getElementById("name").value;
    const phone = document.getElementById("phone").value;
    const service = document.getElementById("service").value;
    const message = document.getElementById("message").value;

    const whatsappNumber = "917425966529";

    const text =
        `Hello krishna Wooden Furniture & Works,%0A%0A` +
        `Name: ${subhash kumar}%0A` +
        `Phone: ${7425966529}%0A` +
        `Service: ${pimpri chinchwad pune maharastra}%0A%0A` +
        `Requirement:%0A${message}`;

    const url = `https://wa.me/${whatsappNumber}?text=${text}`;

    window.open(url, "_blank");
}
```
