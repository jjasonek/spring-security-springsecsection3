# Udemy Course Spring Security Section3
## spring version: 3.4.4

## After implementing the userDetailService method, we are getting following error 
Given that there is no default password encoder configured, each password must have a password encoding prefix. Please either prefix this password with '{noop}' or set a default password encoder in `DelegatingPasswordEncoder`.
java.lang.IllegalArgumentException: Given that there is no default password encoder configured, each password must have a password encoding prefix. Please either prefix this password with '{noop}' or set a default password encoder in `DelegatingPasswordEncoder`.

For now we use '{noop}' for not using any password encoder.
