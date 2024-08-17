Web API Security
===================================


**01. API Keys**

- Identify and authenticate Clients	

**02. Input Validation**

- Never rely on Ul for validation, validate each field on the API	

**03. https over TLS V1.2**

- Valid and strong certificates must be used

**04. OAuth 2.0**

- Secure authentication with authorization flows
- Control delegated access with claim-based Authorization	

**05. Content Security Policy**

- Though mainly used in web apps, you can return API response header with strict CSP policy	

**06. Web Application Firewall**

- Complete suite solution to protect site from XSS, CSRF, DoS, DDoS and other threats

**07. Basic Authentication**

- base64-encoded basic client authentication (must be over https)	

**08. SOP and CORS**

- Only relax same-origin policies with correct and specific CORS policies	

**09. IP White-Listing**

- Only allow clients with specific IPs to access your API


**10. Hash Keys, Secrets**

- Store API keys or secrets hashed using strong hashing functions	

**11. Sanitization**

- Avoid cross-site scripting (XSS) by escaping dangerous scripts in the input	

**12. Rate Limiting**

- Based on IP, domain
- Reduces brute force and DoS and DDoS Attacks
