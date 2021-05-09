---
title: Form Update APK
description : Update APK
---

<form action="https://docs.google.com/forms/u/0/d/e/1FAIpQLScq0tj4XdC_3JnybHlE9OxI25XouFkzj8l4yYw2tPbmcUfP6w/formResponse" method="post" target="hidden_iframe" onsubmit="return validateForm();">
    
   <div class="form-group dknform">
        <label for="inputEmail4">Nama Aplikasi</label>
            <input type="text" class="form-control" id="nama" placeholder="Sesuaikan dengan Playstore" required name="entry.1015864905">
    </div>
    <div class="form-group dknform">
        <label for="inputEmail4">Versi Aplikasi</label>
            <input type="text" class="form-control" id="versi" placeholder="Versi yang akan diupdate" required name="entry.634211217">
    </div>
    <div class="form-group dknform">
        <label for="inputEmail4">Link Aplikasi</label>
            <input type="text" class="form-control" id="link-app" placeholder="Upload Aplikasi ke Google Drive / Apapun" required name="entry.1405466329">
    </div>
    <div class="form-group dknform">
        <label for="inputEmail4">Link Playstore</label>
            <input type="text" class="form-control" id="link-ps" placeholder="Sesuaikan dengan link aplikasi yang sudah tayang" required name="entry.1584739944">
    </div>
    <div class="form-group dknform">
        <label for="inputEmail4">Email</label>
            <input type="email" class="form-control" id="email" placeholder="you@dokundigital.com" required name="entry.75301436">
    </div>
    <div class="form-group dknform">
        <label for="inputEmail4">No Whatsapp</label>
            <input type="text" class="form-control" id="no-wa" placeholder="0876xxxx" required name="entry.695235416">
    </div>

  <button type="submit" class="btn btn-primary dknform">Kirim</button>
</form>
<iframe name="hidden_iframe" id="hidden_iframe" style="display: none;"      
    onload="if(submitted) {window.location.href='/forms/sukses'}"></iframe> 
<script type="text/javascript">var submitted=true;</script>
    
<script type="text/javascript">
    function validateName() {
            var name = document.getElementById('nama-aplikasi').value;
            if(name.length == 0) {
              alert("Name can't be blank") ;
              return false;

            }
            if (!name.match(/^[a-zA-Z]{3,}(?: [a-zA-Z]+){0,2}$/)) {
              alert("Please enter your correct name") ;//Validation Message
              return false;
            }
            return true;
          }

          function validateVersi() {
            var name = document.getElementById('versi').value;
            if(name.length == 0) {
              alert("Name can't be blank") ;
              return false;

            }
            if (!name.match(/^[a-zA-Z]{3,}(?: [a-zA-Z]+){0,2}$/)) {
              alert("Please enter your correct versi") ;//Validation Message
              return false;
            }
            return true;
          }

          function validateLinkApp() {
            var name = document.getElementById('link-app').value;
            if(name.length == 0) {
              alert("Name can't be blank") ;
              return false;

            }
            if (!name.match(/^[a-zA-Z]{3,}(?: [a-zA-Z]+){0,2}$/)) {
              alert("Please enter your correct name") ;//Validation Message
              return false;
            }
            return true;
          }

          function validateLinkPS() {
            var name = document.getElementById('link-ps').value;
            if(name.length == 0) {
              alert("Name can't be blank") ;
              return false;

            }
            if (!name.match(/^[a-zA-Z]{3,}(?: [a-zA-Z]+){0,2}$/)) {
              alert("Please enter your correct name") ;//Validation Message
              return false;
            }
            return true;
          }

          function validatePhone() {
            var phone = document.getElementById('no-whatsapp').value;
            if(phone.length == 0) {
              alert("Phone number can't be blank") ;//Validation Message
              return false;
            }

            if(!phone.match(/^[0]?[789]\d{9}$/)) {
             alert("Please enter a correct phone number") ;//Validation Message
             return false;
           }

           return true;

         }

         function validateEmail () {

          var email = document.getElementById('email').value;
          if(email.length == 0) {
            alert("Email tidak boleh kosong") ;//Validation Message
            return false;

          }

          if(!email.match(/^[A-Za-z\._\-[0-9]*[@][A-Za-z]*[\.][a-z]{2,4}$/)) {
            alert("Mohon masukkan email dengan benar") ;//Validation Message
            return false;

          }

          return true;

        }


        function validateForm() {
          if (!validateName() || !validateVersi() || !validateLinkApp() || !validateLinkPS() ||  !validatePhone() || !validateEmail()) {

            alert("Form tidak terkirim");//Validation Message
            return false;
          }
          else {
            submitted=true;
            return true;
          }
        }
        </script>