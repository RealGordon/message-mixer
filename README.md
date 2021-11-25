## JAVASCRIPT SYNTAX, PART III

# Message Mixer
Message Mixer Inc. offers a message-encryption service that transforms input text, using various [ciphers](https://en.wikipedia.org/wiki/Cipher), and displays the encrypted message to the console.

There are three encryption methods provided by this service:

A “Caesar Cipher” in which the characters of the input message are shifted alphabetically by a given amount.
A “Symbol Cipher” in which select characters from the input message are replaced with visually similar symbols.
A “Reverse Cipher” in which each word of the input message is reversed in place


Example:
The Caesar cipher can be accessed with the following command:
```bash
$ node message-mixer.js caesar 4
Enter the message you would like to encrypt...
> hello world
 
Here is your encrypted message:
> lipps asvph
```
To decode the message 'lipps asvph', we can run the program in reverse, like so:
```bash
$ node message-mixer.js caesar -4
Enter the message you would like to encrypt...
> lipps asvph
 
Here is your encrypted message:
> hello world
```

**To import these ciphers into other javascript(node runtime) programs**:
```javascript
const {caesarCipher, symbolCipher, reverseCipher}=require("./encryptors");
```

Super Encoder LLC encoding services uses Message Mixer Inc. open source **encryptors.js** library.
Users of  Super Encoder LLC's **super-encoder.js** can  encode messages and decode them using the commands below:

**to encode**:
```bash
$ node super-encoder.js encode
Enter the message you would like to encrypt...
> hello world
urrkn jrxuc
```

**to decode**:
```bash
$ node super-encoder.js decode
Enter the message you would like to encrypt...
> urrkn jrxuc
hello world
```
