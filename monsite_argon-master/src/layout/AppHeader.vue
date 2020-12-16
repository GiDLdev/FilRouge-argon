<template>
    <div>
        <b-navbar toggleable="lg" >
            <b-navbar-brand href="#">
                <img src="img/logo1-ac-vect.svg" style="width:auto; height:135px;" alt="Mon site">
            </b-navbar-brand>

            <b-navbar-toggle  target="nav-collapse">☰</b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav >
                    <b-nav-item class="text-center" href="#" disabled>ACCUEIL<br><img src="img/mobile/mobile-menu-arabesque_fffae4.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">BOUTIQUE<br><img src="img/mobile/mobile-menu-pattern_4e473e.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">ATELIERS<br><img src="img/mobile/mobile-menu-arabesque_4e473e.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">SERVICES<br><img src="img/mobile/mobile-menu-pattern_4e473e.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">GALERIES<br><img src="img/mobile/mobile-menu-arabesque_4e473e.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">ACTIVITÉS<br><img src="img/mobile/mobile-menu-pattern_4e473e.png"></b-nav-item>
                    <b-nav-item class="text-center" href="#">CONTACT<br><img src="img/mobile/mobile-menu-arabesque_4e473e.png"></b-nav-item>
                </b-navbar-nav>

                <!-- Right aligned nav items 
                <b-navbar-nav class="ml-auto">
                    <b-nav-form>
                    <b-form-input size="sm" class="mr-sm-2" placeholder="Recherche"></b-form-input>
                    <b-button variant="outline-success" size="sm" class="my-2 my-sm-0" type="submit">Recherche</b-button>
                    </b-nav-form>

                    <b-nav-item-dropdown text="Langue" right>
                    <b-dropdown-item href="#">EN</b-dropdown-item>
                    <b-dropdown-item href="#">ES</b-dropdown-item>
                    <b-dropdown-item href="#">RU</b-dropdown-item>
                    <b-dropdown-item href="#">FA</b-dropdown-item>
                    </b-nav-item-dropdown>

                    <b-nav-item-dropdown right>
                                        // Using 'button-content' slot 
                    <template v-slot:button-content>
                        <em>Utilisateur</em>
                    </template>
                    <b-dropdown-item href="#">Profil</b-dropdown-item>
                    <b-dropdown-item href="#">Déconnexion</b-dropdown-item>
                    </b-nav-item-dropdown>
                </b-navbar-nav> -->
            </b-collapse>
        </b-navbar>
    </div>
</template>
<script>
import { BNavbar, BNavbarBrand, BNavbarToggle, BNavbarNav } from "bootstrap-vue/esm/components/navbar";
import { BCollapse } from "bootstrap-vue/esm/components/collapse";
import { BNavItem, BNavItemDropdown, BNavForm } from "bootstrap-vue/esm/components/nav";  
import { BDropdownItem } from "bootstrap-vue/esm/components/dropdown";
import { BFormInput } from "bootstrap-vue/esm/components/form-input";
import { BButton } from "bootstrap-vue/esm/components/button";

export default {
  components: {
    BNavbar,
    BNavbarBrand,
    BNavbarToggle,        
    BCollapse,
    BNavbarNav,    
    BNavItem,
    BNavItemDropdown,        
    BDropdownItem,
    BNavForm,
    BFormInput,
    BButton 
  }
};
</script>
<style>
.navbar{
    background-color: black;
}


</style>
