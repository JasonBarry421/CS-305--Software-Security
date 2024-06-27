# CS-305--Software-Security

•	Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?

Artemis Financial is a consulting company that develops individualized financial plans for its customers. To accomplish this task, Artemis Financial must keep a record that includes the customer’s employment status, current address, and social security number. The protection of this information is a primary concern for Artemis Financial as it ensures the company follows the governmental standards set by the Gramm-Leach-Bliley Act (GLB). Adhering to these guidelines should protect customers’ information from external threats. Furthermore, Artemis Financial likely deals with transactions that originate from both national and international sources. These transactions would involve communication between two systems. To ensure these communications are secure, Artemis Financial must adhere to the governmental standards set by the Federal Trade Commission Act (FTCA). Adherence to these standards should hinder (or stop) external threats from hijacking these communications. All in all, ensuring Artemis Financial provides a safe and secure platform is a primary concern for the company. This is because any leak would negatively impact a customer’s confidence in the company. Therefore, the company seeks to use the latest and most effective software security to protect their organization from external threats. A modernization requirement that must be considered involves the ever-evolving nature of web application technologies. More specifically, the application used by Artemis Financial must ensure their libraries stay up to date. This modernization technique should allow Artemis Financial to address bugs and security threats in a timely manner.


•	What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?

When I generated a dependency check, I quickly realized that the majority of the identified vulnerabilities were false positives. To counteract these false positives, I added suppressions. I believe I accomplished this task in an adequate manner that simplifies the dependency report to vulnerabilities that are (actually) present in my code.

•	Which part of the vulnerability assessment was challenging or helpful to you?

The most challenging aspect of the vulnerability assessment was understanding that the project did not want me to fix all vulnerabilities. Most of the identified vulnerabilities (after eliminating false positives) are born from the use of outdated packages. Although updating these packages would’ve fixed most of these vulnerabilities, that was beyond the scope of this assignment. Therefore, the most challenging part of the vulnerability assessment was finding the balance between what the assignment required and the actions I would perform otherwise.


•	How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

The primary method used to increase the level of security was through the implementation of a cryptographic hash function. More specifically, the use of a SHA-256 algorithm protects the program from attacks originating from disguised malicious data. Using a SHA-256 algorithm also helps avoid collisions by verifying the content of transmitted data without exposing the data. While the inclusion of an encryption algorithm increases the program’s security, more security features must be utilized. More specifically, as mentioned before, all packages should be updated. Updating these packages would eliminate most (if not all) identified vulnerabilities which should increase the program’s security.

•	How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

To ensure the code and software application were functional and secure, an OWASP Dependency Report was produced before and after refactoring the code. Ensuring these reports were identical allowed me to confirm that no vulnerabilities were introduced due to the refactored code.

•	What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

Before taking this course, I was unaware of the existence of the OWASP Dependency Report nor the ability to suppress false positives. Furthermore, while I understood that encryption algorithms existed, I was unaware of how to implement them or which algorithm to use. Now, after completing projects such as this, I know of their existence as well as how to effectively use methods of improving a program’s security. Going forward, it would be beneficial to apply these tools in future assignments or tasks.




•	Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

Because of the aforementioned issues caused by the use of outdated packages, I likely won’t show this assignment to future employers. These issues have left me unsatisfied with the final project. However, I believe the value of this project comes not from its completion, but on the road to completing it. As mentioned before, I was unaware of the OWASP Dependency Report, the ability to suppress false positives, and the intricacies of encryption algorithms before taking this course. However, by working on a project such as this one, I have experience that should ensure future projects are more secure and, by extension, more presentable to future employers.
