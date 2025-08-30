---
layout              : page
title               : "Contact Me"
meta_title          : "Contact and use our contact form"
subheadline         : "Contact Form"
teaser              : "Want me to apply for a job? Have questions about my work? Found a broken link?"
permalink           : "/contact/"
sidebar             : "left"
---
I look forward to hearing from you, and I'll get back to you as soon as possible!

<div class="container">
  <!-- <h1>Contact Me</h1> -->

  <form target="_blank" action=" https://formsubmit.co/438151fbb32fcd60899ec85ec618e525" method="POST">
    <div class="form-group">
        <div class="form-col">
          <input type="text" name="name" class="form-control" placeholder="Name*" required>
        </div>
    </div>
    <div class="form-group">
      <div class="form-row">
        <div class="form-col">
          <input type="email" name="email" class="form-control" placeholder="Email Address">
        </div>
        <div class="form-col">
          <input type="text" name="phone" class="form-control" placeholder="Phone Number">
        </div>
      </div>
    </div>
    <div class="form-group">
      <textarea placeholder="Your Message*" class="form-control" name="message" rows="10" required></textarea>
    </div>
    <input type="hidden" name="_subject" value="New submission on tatianaanthony.github.io!">
    <input type="text" name="_honey" style="display:none">
    <input type="hidden" name="_next" value="{{ site.url }}/thank-you">
    <button type="submit" class="btn btn-lg btn-dark btn-block">Submit Form</button>
  </form>
</div>