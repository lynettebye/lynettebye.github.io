---
layout: page
title: "Schedule Call"
permalink: /schedule-call
---

# Schedule a free call to optimize your productivity.

The intake call gives you a taste of what coaching is like with me. You can ask all the questions you have about coaching, and I’ll give you tips right away for the areas you most want to change.

**After you submit the form, there will be a Calendly link to schedule the intake call.**

<div id="intake-form-wrap" markdown="0">
<form id="intake-form" action="https://formspree.io/f/xaqrojjr" method="POST">
  <p>
    <label for="first-name">First Name <span class="req">(required)</span></label><br>
    <input type="text" id="first-name" name="First Name" required>
  </p>
  <p>
    <label for="last-name">Last Name <span class="req">(required)</span></label><br>
    <input type="text" id="last-name" name="Last Name" required>
  </p>
  <p>
    <label for="email">Email Address <span class="req">(required)</span></label><br>
    <input type="email" id="email" name="email" required>
  </p>
  <p>
    <label for="working-on">What are you working on now? <span class="req">(required)</span></label><br>
    <textarea id="working-on" name="What are you working on now?" rows="4" required></textarea>
  </p>
  <p>
    <label for="referral">How did you hear about Lynette's coaching? <span class="req">(required)</span></label><br>
    <textarea id="referral" name="How did you hear about Lynette's coaching?" rows="2" required></textarea>
  </p>
  <p><button type="submit" class="teal-button">Submit</button></p>
  <p id="form-error" style="display:none;color:#b00020;">Sorry, something went wrong sending the form. Please try again, or email Lynette directly.</p>
</form>
<div id="form-thanks" class="thanks-box" style="display:none;">
  <p>Thank you for filling in the form. You can schedule your free 30-minute intake call here: <a href="https://calendly.com/lynettebye/30min">https://calendly.com/lynettebye/30min</a>. You’ll also receive a Google doc prior to our call with questions to prepare before our call.</p>
  <p>I look forward to speaking with you!</p>
</div>
<script>
document.getElementById('intake-form').addEventListener('submit', async function (e) {
  e.preventDefault();
  var form = e.target;
  document.getElementById('form-error').style.display = 'none';
  try {
    var resp = await fetch(form.action, {
      method: 'POST',
      body: new FormData(form),
      headers: { 'Accept': 'application/json' }
    });
    if (resp.ok) {
      form.style.display = 'none';
      document.getElementById('form-thanks').style.display = 'block';
    } else {
      document.getElementById('form-error').style.display = 'block';
    }
  } catch (err) {
    document.getElementById('form-error').style.display = 'block';
  }
});
</script>
</div>


![](/assets/images/OldTreebyWaterfallSep2023-c5229f.jpg)

\*The intake call is for first-time callers. If you’ve done coaching with Lynette before, please email to schedule a call.
