# Udemy Course Spring Security Section3
## spring version: 3.4.4

## After implementing the userDetailService method, we are getting following error 
Given that there is no default password encoder configured, each password must have a password encoding prefix. Please either prefix this password with '{noop}' or set a default password encoder in `DelegatingPasswordEncoder`.
java.lang.IllegalArgumentException: Given that there is no default password encoder configured, each password must have a password encoding prefix. Please either prefix this password with '{noop}' or set a default password encoder in `DelegatingPasswordEncoder`.

For now we use '{noop}' for not using any password encoder.


## PasswordEncoder
### We use the BCryptPasswordEncoder which is the default one for the factory.
54321 -> $2a$12$gqh4eq8vC5UirpfzWwGWf.BgJ9Ffd0ADUSDqf34qaHCoDeBNEUzZS

now we have not encoded password for the user
and encoded one (using BCrypt) for the admin.


## Dealing with Compromised Passwords
after applying the haveIBeenPwnedRestApiPasswordChecker, we get the error message:
The provided password is compromised, please change your password.

To solve this, we change our passwords.
Prdel@54321 -> $2a$12$6HmvMNc6LH.9kb3raE5d4emPS/MfENuIMZhw2jVc4bVdXd13021JC
