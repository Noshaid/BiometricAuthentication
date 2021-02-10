# BiometricAuthentication
Face ID or Passcode required to enter 

# Implementation
We will start with the creation of a new method called authenticationWithTouchID. Here we put the logic to authenticate the user using biometrics (fingerprints/face recognition) or with passcode as a fallback.
To do this we use two methods:
canEvaluatePolicy method — returns false if device owner authentication is not available.
evaluatePolicy method — requests authentication from the user through biometrics or passcode.
Basically, our app will show the facial recognition popup first (or fingerprints popup, if our device does not support Face ID) and then the fallback button after the first unsuccessful attempt to use the passcode.
