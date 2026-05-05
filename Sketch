const video = document.getElementById('stromVideo');
const instructions = document.getElementById('instructions');
let hasStarted = false;

// Funktion til at starte videoen første gang
function startExperience() {
    if (!hasStarted) {
        video.play();
        instructions.style.display = 'none';
        hasStarted = true;
    }
}

// TOUCH INTERAKTION (Til iPhone)
window.addEventListener('touchstart', (e) => {
    if (!hasStarted) {
        startExperience();
    } else {
        video.pause(); // Pauser når fingeren holdes nede
    }
});

window.addEventListener('touchend', () => {
    if (hasStarted) {
        video.play(); // Starter igen når fingeren løftes
    }
});

// MUS INTERAKTION (Til computer test)
window.addEventListener('mousedown', () => {
    if (!hasStarted) {
        startExperience();
    } else {
        video.pause();
    }
});

window.addEventListener('mouseup', () => {
    if (hasStarted) {
        video.play();
    }
});
