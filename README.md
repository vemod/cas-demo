POC to login via REST API and create SSO with Token Login
=========================================================

- Based on vanilla cas-overlay-master as of 14.10.2022
- Includes following customizations
  - JSON service registry
  - REST api
  - Token login support
  - JWT as service ticket
  - SSL
- Contains postman demo collection to login via rest and create sso via token login


WAR Overlay Type: `cas-overlay`

# Versions

- CAS Server `7.0.0-SNAPSHOT`
- JDK `17`
                     
# How to use

For demo purposes we use `foo.bar` hostname to provide ssl and cookies. Browsers don't store cookies under localhost. 
So just add `127.0.0.1 foo.bar` to `/etc/hosts`

- `./gradlew createKeystore` (just once to have the keystore)
- `./gradlew run -xtest`
- Run steps in postman. Check test results
