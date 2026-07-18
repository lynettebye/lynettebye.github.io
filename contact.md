---
layout: page
title: "Contact"
permalink: /contact
---

![](/assets/images/dream_izho599am8klong-123962.jpg)

# How Can I Help?

If you want to contact me about a story, you can find me on Signal at 447736677070 or email lynettebye@gmail.com.

You're welcome to fill out the form with your questions or schedule an intake call [here](/schedule-call) to discuss coaching fit.

<div id="contact-form-wrap" markdown="0">
<form id="contact-form" class="site-form" action="https://formspree.io/f/xaqrojjr" method="POST">
  <input type="hidden" name="Form" value="Contact page">
  <p>
    <label for="c-name">Name</label><br>
    <input type="text" id="c-name" name="Name">
  </p>
  <p>
    <label for="c-email">Email Address <span class="req">(required)</span></label><br>
    <input type="email" id="c-email" name="email" required>
  </p>
  <p>
    <label for="c-subject">Subject</label><br>
    <input type="text" id="c-subject" name="Subject">
  </p>
  <p>
    <label for="c-message">Message</label><br>
    <textarea id="c-message" name="Message" rows="5"></textarea>
  </p>
  <p><button type="submit" class="teal-button">Submit</button></p>
  <p id="contact-error" style="display:none;color:#b00020;">Sorry, something went wrong sending the form. Please try again, or email Lynette directly.</p>
</form>
<div id="contact-thanks" class="thanks-box" style="display:none;">
  <p>Thank you for your message! I’ll get back to you soon.</p>
</div>
<script>
document.getElementById('contact-form').addEventListener('submit', async function (e) {
  e.preventDefault();
  var form = e.target;
  document.getElementById('contact-error').style.display = 'none';
  try {
    var resp = await fetch(form.action, {
      method: 'POST',
      body: new FormData(form),
      headers: { 'Accept': 'application/json' }
    });
    if (resp.ok) {
      form.style.display = 'none';
      document.getElementById('contact-thanks').style.display = 'block';
    } else {
      document.getElementById('contact-error').style.display = 'block';
    }
  } catch (err) {
    document.getElementById('contact-error').style.display = 'block';
  }
});
</script>
</div>

[Frequently Asked Questions »](/coaching#faq)

![](/assets/images/BranchesAbove-578cb2.jpg)
