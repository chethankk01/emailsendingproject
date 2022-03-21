# emailsendingprojectdjango
sending email to specified gmail

**After you create a project include these variables in settings.py**

EMAIL_HOST = "smtp.gmail.com"
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = "email address"
EMAIL_HOST_PASSWORD = "email password"

EMAIL_BACKEND = "django.core.mail.backends.smtp.EmailBackend"

**After including the variable in the views.py**

step 1: from django.core.mail import send_mail
step 2: from django.conf import settings
step 3: After importing through the send_mail function send the mail i.e
        send_mail(subject,content,from,to)
