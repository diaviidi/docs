# Lyra : Definition of the ID for Alastria

## ANS - Alastria Name Service

alastria.users.<alias> aka @<alias>
alastria.<brand>

Each brand will need to deploy a Smart contract acting as a resolver for its own domain.
Based on ENS but with a different way of giving names

## Alastria ID App

Double verification : email + SMS (phone) 
We will need a double verification to create a new Identity. The app will ask for the Phone Number and will send a verification code via SMS. The app will also ask for an email and will send a code to the email.

Once the App is verified we can save basic information about the user : First Name and last names (we have 2 in Spain), address, gender and date of birth. 

1. Create a Smart contract representing your ID
2. Create a file (JSON) with all your data following the standar Persona. We create a merkle tree of all the information. This way we can share anly the information we want to share and the hashes for other information. A nonce will be added whenever needed (DNI) for security reasons.
3. Write in the registry the top of the merkle tree. AT this point thins information is not certified by anyone (not trutsable)
4. Ask for an alias and create the alias in the ANS.

## LRegister/Login into an App

Picture of a QR
