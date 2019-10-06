# Basicdrf
Basic django rest framework login register and logout with tokens as well as social authentication with facebook.

### Endpoints

/rest-auth/login/ (POST)
..* username
..* email
..* password
      Returns Token key

/rest-auth/logout/ (POST)

/rest-auth/password/reset/ (POST)
..* email

/rest-auth/password/reset/confirm/ (POST)
..* uid
..* token
..* new_password1
..* new_password2

/rest-auth/password/change/ (POST)
..* new_password1
..* new_password2
..* old_password

/rest-auth/user/ (GET, PUT, PATCH)
..* username
..* first_name
..* last_name
Returns pk, username, email, first_name, last_name

#### Registration

/rest-auth/registration/ (POST)
..* username
..* password1
..* password2
..* email

#### Social Authentication

/rest-auth/facebook/ (POST)
..* access_token
..* code
