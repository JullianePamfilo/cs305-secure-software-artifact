Client and Its Requirements in Brief
Artemis Financial is in the business of providing secure digital banking. "Artemis Security A minor technical audit to ensure we are following best practice and provide mitigation advice The Artemis team want to ensure we are following best practice in our Spring Boot RESTful API implementation in order to maintain the same level of security over the ongoing development." What I had to do was: - Identify security threats - Use secure coding methods to counter them - Suggest methods to mitigate security risks and protect the clients’ data and comply with regulations
Success in Identifying Vulnerabilities
I managed to find vulnerabilities such as hard-coded credentials, insecure HTTP methods, and not validating input by using static code analysis together with manual code inspection. Part of the motivation for me to push for these was to take advantage of discussions such as these around securing code — that’s a good thing, because healthy code security is going to keep both end users and the company’s reputation safe from potential vulnerabilities and/or attacks.
Challenging/Helpful Assessment Aspects
The hardest thing was how to interpret the output of the dependency-check tools and what you see there to what are known vulnerabilities. But this has definitely taught me how to triage by CVSS and apply targeted fixes.
Increasing Layers of Security
By way of further security hardening, I added input validation, parameter sanitizing and disabled unnecessary HTTP methods. Going forward I'd add more tools - your OWASP ZAP or something like Burp Suite - and implement OWASP Top 10 testing and mitigation.
Ensuring Functionality and Security
I also used unit tests, and Postman to be sure the API still worked as expected after sparsifying the security. I've also looked at Git diffs and re-run the vulnerability scans to make sure there were no new issues.
Tools and Practices Used
I've implemented Maven OWASP Dependency-Check where I also took responsibility for including security into the CI/CD pipeline (Lombard Odier’s company CI/CD was full of vulnerabilities), Spring Security, I have implemented Git version control and some of the more boring defence (no input box on pages, trying to secure all things like no hardcoded secrets, checking user input and so on). These are useful skills that I will use in future projects.
Value for Future Employers
This artifact provides evidence of my skills in finding and correcting software vulnerabilities in a real-world setting using enterprise Java frameworks such as Spring Boot and industry best practice for software security development. It’s a good demonstration of my practical security and development ability.
