

# HuntXSS
HuntXSS is a security tool designed to identify and exploit cross-site scripting (XSS) vulnerabilities in web applications. XSS is a type of security vulnerability that allows an attacker to inject malicious code into a web page viewed by other users. This can lead to the theft of sensitive information or the execution of unauthorized actions on the user's behalf.

HuntXSS works by scanning web pages and identifying potential sources of XSS vulnerabilities, such as user input fields or script tags. It then tests these potential vulnerabilities by injecting test payloads to see if they are successful in executing malicious code.

The tool is designed to be easy to use and customizable, with options for specifying the target website, payload types, and output format. HuntXSS also includes a user-friendly interface for viewing and analyzing the results of its scans, allowing users to quickly identify and address any vulnerabilities.

Overall, HuntXSS is a powerful tool for web developers and security professionals looking to identify and mitigate XSS vulnerabilities in their web applications.


## Easy Installation

```
git clone -b master https://github.com/MonkHacker1/HuntXSS.git
cd HuntXSS
pip3 install -r requirements.txt
```

## Usage Instructions
`python3.6 xssmap.py -h`

Support POST and GET request methods, support parameter injection detection in cookie, referer, useragent fields
For example, test the returnUrl parameter in POST data:

`python3.6 xssmap.py -u "https://example.com/login.do" --data="returnUrl=utest" -p returnUrl` 


## Features
1. Support url encoding bypass
2. Support unicode encoding of HTML tag attribute value to bypass
3. Support HTML encoding to bypass the HTML tag attribute value
4. Support for flexible replacement of () '"to bypass
5. Case bypass


## Todo

- [ ] DOM XSS Detect
- [ ] Json XSS Detect







