document.getElementById('explosionButton').addEventListener('click', function() {
    const explosionSound = document.getElementById('explosionSound');
    const explosionImage = document.getElementById('explosionImage');
    
    // Probabilidad de que ocurra la explosión (50%)
    if (Math.random() < 0.5) {
        explosionSound.play();
        explosionImage.classList.remove('hidden');
    } else {
        explosionImage.classList.add('hidden');
    }
});
