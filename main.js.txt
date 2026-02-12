const passwordPage = document.getElementById('password-page');
const mainSite = document.getElementById('main-site');
const passwordInput = document.getElementById('password-input');
const hint = document.getElementById('hint');

passwordInput.addEventListener('keypress', function(e) {
    if (e.key === 'Enter') {

        if (passwordInput.value.toLowerCase() === 'sandra') {
            passwordPage.classList.add('hidden');
            mainSite.classList.add('show');
        } else {
            hint.classList.add('show');
            setTimeout(() => hint.classList.remove('show'), 3000);
        }

    }
});
