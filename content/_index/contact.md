+++
fragment = "contact"
#disabled = true
date = "2017-09-10"
weight = 300
background = "dark"
form_name = "defaultContact"

title = "Contact"
subtitle  = "Contactez-nous si vous avez des questions !"

# PostURL can be used with backends such as mailout from caddy
post_url = "https://formspree.io/test@tets.com" #default: formspree.io
email = ""
button = "Send Button" # defaults to theme default
netlify = true

# Optional google captcha
#[recaptcha]
#  sitekey = ""

[message]
  success = "Email envoye" # defaults to theme default
  error = "Email n'a pas ete envoye" # defaults to theme default

# Only defined fields are shown in contact form
[fields.name]
  text = "Your Name *"
  #error = "" # defaults to theme default

[fields.email]
  text = "Your Email *"
  #error = "" # defaults to theme default

[fields.phone]
  text = "Your Phone *"
  #error = "" # defaults to theme default

[fields.message]
  text = "Your Message *"
  #error = "" # defaults to theme default

# Optional hidden form fields
# Fields "page" and "site" will be autofilled
[[fields.hidden]]
  name = "page"

[[fields.hidden]]
  name = "someID"
  value = "template.cedille.club"
+++
