---
title: Contact
permalink: /contact/
---

Leave a message below, or simply send an e-mail directly to [{{site.email}}](mailto:{{site.email}}), that we'll get back to you as soon as possible.

<form
  action="https://formspree.io/f/mbjpvrvd"
  method="POST"
  class="wj-contact"
>
    <input type="text" name="email" placeholder="Email Address*" required>
    <textarea type="text" name="content" rows="10" placeholder="Message" required></textarea><br />
    <input type="submit" value="Submit">
</form>

<style>
form.wj-contact input[type="text"], form.wj-contact textarea[type="text"] {
    width: 90%;
    vertical-align: middle;
    margin-top: 0.25em;
    margin-bottom: 0.5em;
    padding: 0.75em;
    font-family: monospace, sans-serif;
    font-weight: lighter;
    border-style: solid;
    border-color: #444;
    outline-color: #2e83e6;
    border-width: 1px;
    border-radius: 3px;
    transition: box-shadow .2s ease;
}
form.wj-contact input[type="submit"] {
    outline: none;
    color: white;
    background-color: #2e83e6;
    border-radius: 3px;
    padding: 0.5em;
    margin: 0.25em 0 0 0;
    border: 1px solid transparent;
    height: auto;
}
</style>
