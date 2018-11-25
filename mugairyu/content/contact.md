---
title: "Contactez-nous"
weight: 60
draft: false
tags: [ "contact", "facebook", "message", "email", "mail" ]
keywords: [  "contact", "facebook", "message", "email", "mail" ]
categories:
  - "contact"
---

![Umegawa in Sagami province](/images/Umegawa_in_Sagami_province-mini.jpg)

<form id="contactform" method="post" action="https://formspree.io/antonio@architux.com">
	<div class="field half first">
		<input type="text" name="name" id="name" placeholder="Nom"/>
	</div>
	<div class="field half">
		<input type="email" id="email" name="email" placeholder="Mail">
	</div>
	<div class="field">
		<textarea name="message" id="message" rows="4" placeholder="Message"></textarea>
	</div>
	<ul class="actions">
		<li><input type="submit" value="Envoyer" class="special" /></li>
		<li><input type="reset" value="Réinitialiser" /></li>
	</ul>
	<input type="hidden" name="_next" value="?sent#formspree" />
	<input type="hidden" name="_subject" value="Subject for your mail like new message" />
	<input type="text" name="_gotcha" style="display:none" />
</form>
<span id="contactformsent">Merci pour votre message</span>

<script>
$(document).ready(function($) { 
    $(function(){
        if (window.location.search == "?sent") {
        	$('#contactform').hide();
        	$('#contactformsent').show();
        } else {
        	$('#contactformsent').hide();
        }
    });
});
</script>

