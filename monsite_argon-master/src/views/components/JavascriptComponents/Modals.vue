<template>
    <div class="modal fade" id="staticBackdrop" data-backdrop="static" data-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
            <div style="background-color:#fff;" class="modal-content">
                <div style="padding:1rem 1rem 0rem; border-bottom:0px;" class="modal-header">
                    <h6 id="staticBackdropLabel" class="modal-title">Besoin d'information, d'un devis ou bien votre projet à me soumettre ?<br>Discutons-en.</h6>
                    <button style="width:3.75rem; text-align:right; font-family:Myriad Pro Bold; background-color:#fff; border:none;" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">x</span></button>
                </div>
                <div style="padding:0rem 1rem 1rem;" class="modal-body">
                    <form method="post" action="submit.php" class="form-group" >
                        <input placeholder="Votre nom" type="text" id="name" name="name" required pattern="^[A-Za-z '-]+$" maxlength="20" >
                        <input placeholder="Votre e-mail" type="email" id="email" name="email" required pattern="^[A-Za-z]+@{1}[A-Za-z]+\.{1}[A-Za-z]{2,]$">
                        <p class="antispam">Laissez ce champ vide:
                        <br><input name="url"></p>
                        <textarea placeholder="Votre message" type="text" name="message" required="" rows="7" cols="30"></textarea>
                        <div class="btnform">
                            <button class="reset" type="reset" value="effacer">effacer</button>
                            <button class="envoi" type="submit" value="envoyez">envoyer</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Modal from "@/components/Modal.vue";
export default {
  components: {
    Modal
  }
};
/* var $reset = document.querySelectorAll(".reset");
var	$erreur = document.querySelectorAll("required");
var	$input = document.querySelectorAll("input");
var	$text = document.querySelectorAll("textarea");


[].forEach.call(document.querySelectorAll($reset), function(el) {
	el.addEventListener('click', function() {
		$input;
		$text;
		[].forEach.call( document.querySelectorAll($erreur), function(elem) {
				elem.style.display = 'none';
		});
	});
}); */ 


</script>
<style>
  .modal-header h6, input::-webkit-input-placeholder, textarea, input {
    font-family: 'Myriad Pro Regular';
    transition: all 0.3s ease-in-out;
  }
  .modal-header h6 {
    font-size: 22px;
    font-weight: 600;
    color: #730012;
    padding: 20px;
  }
  .form-group{ 
    width:100%;
    padding:30px 20px 20px;
    margin-bottom:0rem;
  }
  input {
    display:block;
    margin:auto 0 30px;
    font-size:16px;
    width: 100%;
    border: none;
    padding: 5px 5px;
    border-bottom: solid 1px #730012;
    transition: all 0.3s cubic-bezier(.64,.09,.08,1);
    background: linear-gradient(to bottom, rgba(255,255,255,0) 96%, #730012 4%);
    background-position: -575px 0;
    background-size: 100% 100%;
    background-repeat: no-repeat;
    background-color: #fff;
  }
  input:focus,
  input:valid,
  textarea,
  textarea:focus{
    box-shadow: none;
    outline: none;
    background-position: 0 0;
  }
  input::-webkit-input-placeholder{
    color: #616F7C;
    font-size: 11px;
    transform: translateY(-20px);
    visibility: visible !important;
  }
  textarea{
    margin:16px 0 36px;
    resize: vertical;
    border:solid 1px #730012;
    padding-left:5px;
    width:100%;
    height:100%;
    background-color: #fff;
  }
  .btnform{
    display:flex;
    flex-flow: row nowrap;
    justify-content: space-between;
  }
  button.reset{
    left:0;
    width: 40%;
    border: solid 1px #731200;
    background-color: transparent;
    color:#731200;
    font-weight: normal;
    cursor: pointer;
    font-size:16px;
    border-radius: 3px;
    padding: 6px;
    height:40px;
    box-shadow: 0 3px 6px 0 rgba(0,0,0,0.2);
    font-family: 'Myriad Pro Regular';
    transition: all 0.3s ease-in-out;
  }
  button.envoi{
    right:0;
    width: 50%;    
    background-color:#730012;
    border: none;
    color: white;  
    font-weight: bold;
    cursor: pointer;
    font-size:16px;
    border-radius: 3px;
    padding: 6px;
    height:40px;
    box-shadow: 0 3px 6px 0 rgba(0,0,0,0.2);
    font-family: 'Myriad Pro Regular';
    transition: all 0.3s ease-in-out;
  }
  button.reset:hover,
  button.envoi:hover { 
    transform: translateY(-3px);
    box-shadow: 0 6px 6px 0 rgba(0,0,0,0.2);
  }
  #erreur {
    display: none;
  } 
  @media (min-width: 320px) and (max-width: 575px){
    .modal-header h6 {
      font-size: 20px;
      padding:10px;
    }
    .form-group{ 
      padding:20px 10px 10px;
    }
  }
.antispam { 
    display:none;
}
</style>
