<template>
    <form class="contact">
        <label for="name">Nom Prénom :</label>
        <input id="name" type="text" placeholder="Dumas Matthias"/>
        <label for="email">Email :</label>
        <input id="email" type="email" placeholder="exemple@gmail.com"/>
        <label for="msg">Votre message :</label>
        <input id="msg" type="text"/>
        <input type="submit" placeholder="Envoyer">
    </form>
</template>


<style scoped>
    .contact{
        display: flex;
        flex-direction: column;
        text-align: left;
        gap: 1rem;
    }  
</style>