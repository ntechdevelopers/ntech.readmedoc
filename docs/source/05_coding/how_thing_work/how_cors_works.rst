How CORS Works
==================

**Example:**

You have a website (country A) that tries to use a script from another website (country B).

- Without CORS (passport control), this could be risky—what if the script is harmful?
- With CORS, country B's website tells your browser if it's safe to use the script, like a security check at the airport.

CORS, which stands for Cross-Origin Resource Sharing, is a bit like international travel rules for your web browser.

Let me break it down:

- Imagine each website is a country. When you travel from one country to another, you often need permission or a special pass (like a visa) to enter.
- This is to ensure safety and regulate who comes in and out. In the web world, CORS is like those travel rules.

CORS is a security feature in web browsers. It controls whether resources (like scripts, images, etc.) can be shared between different websites (or "origins").

**Why CORS?**

- To protect web users from malicious content.
- It prevents a website from freely accessing resources from another website without proper permission.

