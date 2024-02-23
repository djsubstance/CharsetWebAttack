# CharsetWebAttack
20 methods to compromise a target if they dont set the charset in the http response

1. SQL Injection
By modifying the charset, you might bypass sanitization filters that don't account for alternative encodings, allowing for injection of malicious SQL queries.

2. Cross-Site Scripting (XSS)
Alternative charsets can be used to encode payloads in a way that they are not detected by basic XSS filters but will execute once decoded by the browser.

3. Directory Traversal
Encoding file paths using different charsets might help in bypassing filters preventing directory traversal attacks.

4. Command Injection
Charset manipulation can enable command injection by encoding malicious commands in ways that are overlooked by input validation routines.

5. Email Header Injection
If an application constructs email headers based on user input, changing the charset might allow for the injection of additional headers or manipulation of existing ones.

6. HTTP Request Smuggling
Varying the charset in HTTP requests can be part of complex techniques to smuggle malicious requests through security devices that misinterpret the payload boundaries.

7. HTTP Response Splitting
Charset variations might be exploited to inject HTTP headers or even additional responses within the body of an HTTP response.

8. Template Injection
Template engines might improperly handle different charsets, leading to injection opportunities.

9. File Upload Vulnerability
Manipulating the charset of the file name or content might bypass file validation checks, leading to uploading of malicious files.

10. SSRF (Server-Side Request Forgery)
Using alternative charsets in URLs or parameters might bypass filters preventing SSRF attacks.

11. XML External Entity (XXE) Injection
Encoding payloads in different charsets might bypass filters or parsers looking for XXE patterns.

12. Buffer Overflow
Certain charsets might lead to unexpected byte lengths, potentially triggering buffer overflows in vulnerable applications.

13. LDAP Injection
Charset manipulation can help encode LDAP injection payloads, bypassing filters or validation mechanisms.

14. SSI (Server-Side Includes) Injection
Changing the charset might allow for the injection of SSI directives that would otherwise be filtered.

15. Path Manipulation
Encoding paths using different charsets might bypass validation checks, leading to unauthorized file access.

16. Remote File Inclusion (RFI)
Alternative charsets might be used to obscure or mutate URLs in RFI attacks, evading detection.
17. Local File Inclusion (LFI)
Similar to RFI, changing charset encoding can help in bypassing filters against LFI vulnerabilities.

18. Null Byte Injection
Although less common with modern systems, altering charset might allow for null byte injection attacks where the application misinterprets the end of strings.

19. Cryptojacking Payload Delivery
Encoding cryptojacking scripts in alternative charsets might bypass content filters on vulnerable servers.

20. CORS Bypass
Manipulating charsets in cross-origin requests might exploit misconfigurations in CORS policies, leading to unauthorized actions.


