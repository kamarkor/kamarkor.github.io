# Welcome to My Data Universe !
## About Me
<p style="text-align: justify;">Hello! I am Kamar, a data scientist at EDF, one of the world’s largest energy companies. I am currently dedicated to developing impactful solutions in NLP and Generative AI. French-educated, with a dash of Spanish flair, I combine savoir-faire with adaptability to navigate complex challenges. Outside the office, I am a traveler, a photographer, and sometimes an athlete. Dive in, and discover my journey in data science and AI 😊</p>

## Personnal Projects
work in progress...

## Writings
work in progress...

## Contact
You can find me on [LinkedIn](https://www.linkedin.com/in/kamarkoraibi) or send me a message below:
<form action="https://formspree.io/f/xyzykknr" method="POST" onsubmit="submitForm(event) style="display: flex; flex-direction: column; width: 300px;">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    <label for="email">Email Address:</label>
    <input type="email" id="email" name="_replyto" required>
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="3" required></textarea>
    <button type="submit" style="margin-top: 10px;">Message Me</button>
</form>
<p id="confirmationMessage" style="display: none; color: green;">Message sent!</p>

<script>
function submitForm(event) {
    event.preventDefault(); // Empêche le formulaire de se soumettre normalement

    const form = document.getElementById("contactForm");
    const confirmationMessage = document.getElementById("confirmationMessage");

    // Envoie le formulaire via Fetch API
    fetch(form.action, {
        method: "POST",
        body: new FormData(form),
        headers: {
            'Accept': 'application/json'
        }
    }).then(response => {
        if (response.ok) {
            form.style.display = "none"; // Cache le formulaire
            confirmationMessage.style.display = "block"; // Affiche le message de confirmation
        } else {
            alert("Oops! There was a problem submitting your form.");
        }
    }).catch(error => {
        alert("Oops! There was a problem submitting your form.");
    });
}
</script>
