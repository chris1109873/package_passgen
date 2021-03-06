# package_passgen

### Project description:
A package to generate strong random passwords. User can define the length, 
number of passwords and the character sets (punctuation, lowercase, uppercase 
and numbers) that needs to be included in the password.


### Usage:

* No of passwords that would be generated by default is 1
* Minimum length of password is 8
* Possible options for charsets include 'punctuation', 'lowercase', 
  'numbers' and 'uppercase'. You can choose to include one or more charsets
  in the generated password


``` python
  import package_passgen as passgen

  include_charsets = ['punctuation', 'lowercase', 'numbers', 'uppercase']
  
  password_list = passgen.generate_password(
    password_length=10,
    include_charsets=include_charsets,
    no_of_passwords=5
    )
  
  for p in password_list:
    print(p)
```
