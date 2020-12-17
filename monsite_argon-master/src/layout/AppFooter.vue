<template>
    <footer>
        <div>
            <hr>
            <p class="p7">&copy; Copyright {{year}} Angélique Calfati - Tous droits réservés | <a href="#0">Mentions Légales</a> | <a href="#0">Crédits</a> | 
                <a href="#0">Plan du site</a> | <a href="#0">CGV</a> | Désign & Développement : <a href="https://www.gidl.fr" target="_blank" rel="follow">GiDL</a>
            </p>
        </div>
    </footer>
</template>
<script>
export default {
  name: 'app-footer',
  data() {
    return {
      year: new Date().getFullYear()
    }
  }
};
</script>
<style>

</style>
