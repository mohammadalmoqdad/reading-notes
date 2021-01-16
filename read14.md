## When is Basic Authorization used vs. Bearer Authorization?
- the basic is for sign in for the first time and it use the bcrypt to encrypt the password, but the bearer isis used to avoid asking for pass and username each time and it done by storing a token with secret key

## What does the JSON Web Token package do? 
transfare encrypted data.

## What considerations should we make when creating and storing a SECRET?
- memorizable, and not a plain text


* encryption translates data into another form, or code, so that only people with access to a secret key (formally called a decryption key) or password can read it. Encrypted data is commonly referred to as ciphertext, while unencrypted data is called plaintext.

* Token is a JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim

* Bearer Tokens are the predominant type of access token used with OAuth 2.0. A Bearer Token is an opaque string, not intended to have any meaning to clients using it

* JSON Web Token is a way to send information that can be verified and trusted by means of a digital signature.



# Role Based Access Control
- **it is an approach to restricting system access to authorized users.**.
- it is also is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.

- The way of thinking at RBAC :
  - for each user what is the role for that user
  - what is the resources that user can access.


- benefits :
  - privacy is rellated to the role not the user
  - each new employee has the ability to activate his own role
  - SELinux support it

- management of individual user rights becomes a matter of simply assigning appropriate roles to the user's account; this simplifies common operations, such as adding a user, or changing a user's department.



- Three primary rules are defined for RBAC:

1. **Role assignmen**t:
- A subject can exercise a permission only if the subject has selected or been assigned a role.
2. **Role authorization**:
- A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
3.**Permission authorization**:
- A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.







