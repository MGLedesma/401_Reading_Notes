# Burp Suite

Resource: [What Is Burp Suite?](https://www.technipages.com/what-is-burp-suite)

## What Is Burp Suite?
- a suite of tools from PortSwigger to aid in the penetration testing of web applications over both HTTP and HTTPS
- primary tool is a proxy designed to allow the analysis and editing of web traffic
- proxy can intercept web requests and responses and read and edit them in real-time before they reach their respective destinations
- many of the tools are designed to integrate with the main proxy and can have requests imported to them
    - Intruder allows to import a request and then configure arrange of payloads to attempt and can then run through them automatically.
    - Repeater allows to import a web request and then make manual modifications to it and see the response side by side allowing for minor adjustments to attempted exploits and easily see if it’s working.
    - A dashboard feature shows a list of identified issues, although these need to be manually checked for false positives.
    - Sequencer is designed to analyse the randomness of data such as session IDs, CSRF tokens, and password reset tokens.
    - The analysis requires more than 100 samples but can identify weaknesses in how supposedly random values are being generated.
    - Decoder allows you to decode strings from a range of encoding standards as well as allowing you to encode data again.
    -  Comparer allows you to compare two strings to check for minor differences
