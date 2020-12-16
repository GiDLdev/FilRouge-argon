<template>
    <footer>
        <hr>
        <div>
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
footer {
    width:100%;
    background-color: #040302;
    padding: 0 15px 15px;
    height:69px;
}
footer hr{
    margin-top:0;
    margin-bottom:10px;
    position: relative;
    background-color: #e0dccc;
    width:100%;
}
p.p7,
p.p7 a{
    color:#e0dccc;
}
p.p7 a:hover,
p.p7 a:active,
p.p7 a:focus{
    color:#fffae4;
    -webkit-text-decoration-line: underline;
            text-decoration-line: underline;
}
</style>
