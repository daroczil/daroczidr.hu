+++
fragment = "contact"
#disabled = true
date = "2017-09-10"
weight = 1100
#background = "light"
form_name = "defaultContact"

title = "Üzenet küldése"
subtitle  = "Kérjük, hogy adja meg elérhetőségeit, majd írja meg üzenetét, és kattintson a Küldés gombra:"

# PostURL can be used with backends such as mailout from caddy
#post_url = "https://example.com/mailout" #default: formspree.io
email = "daroczil@gmail.com"
button = "Küldés" # defaults to theme default
#netlify = false

# Optional google captcha
#[recaptcha]
#  sitekey = ""

[message]
  #success = "" # defaults to theme default
  #error = "" # defaults to theme default

# Only defined fields are shown in contact form
[fields.name]
  text = "Név"
  #error = "" # defaults to theme default

[fields.email]
  text = "Email cím"
  #error = "Hibás email cím" # defaults to theme default

[fields.phone]
  text = "Telefonszám"
  error = "Csak számokat irjon be, pl. 06205555555" # defaults to theme default

[fields.message]
  text = "Üzenet"
  #error = "" # defaults to theme default

# Optional hidden form fields
# Fields "page" and "site" will be autofilled
[[fields.hidden]]
  name = "page"

[[fields.hidden]]
  name = "someID"
  value = "example.com"
+++
