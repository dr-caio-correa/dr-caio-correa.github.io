---
title: Contact
description: Send me a message
---

<section class="section">
  <h2>Send me a message</h2>
  <p class="muted">Fill out the form and I’ll get back to you.</p>

  <div class="contact-grid">
    <form class="contact-form" method="POST" action="https://formspree.io/f/YOUR_FORM_ID">
      <div class="contact-left">
        <label>
          <span>Your name</span>
          <input name="user_name" type="text" placeholder="Your Name" required>
        </label>

        <label>
          <span>Email address</span>
          <input name="user_email" type="email" placeholder="you@email.com" required>
        </label>

        <label>
          <span>Subject</span>
          <input name="user_subject" type="text" placeholder="Subject" required>
        </label>
      </div>

      <div class="contact-right">
        <label>
          <span>Message</span>
          <textarea name="user_message" rows="10" placeholder="Write your message…" required></textarea>
        </label>

        <!-- Optional: helps reduce spam + gives context -->
        <input type="hidden" name="_subject" value="New message from Caio Correa Analytics">
        <input type="text" name="_gotcha" style="display:none">

        <button class="contact-btn" type="submit">Send message</button>
      </div>
    </form>
  </div>
</section>
