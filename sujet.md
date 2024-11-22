# Practical Session #1: Introduction

1. Find in news sources a general public article reporting the discovery of a software bug. Describe the bug. If possible, say whether the bug is local or global and describe the failure that manifested its presence. Explain the repercussions of the bug for clients/consumers and the company or entity behind the faulty program. Speculate whether, in your opinion, testing the right scenario would have helped to discover the fault.

### 🟢 Description of the Bug: 
The **"BLASTPASS"** vulnerability was a critical security flaw discovered in iOS in September 2023. It exploited a weakness in the image processing component of the operating system. Attackers could send a maliciously crafted image or attachment to a target device. Upon receiving this malicious content, the device would process the image, triggering the exploit. This zero-click vulnerability allowed attackers to install spyware capable of accessing sensitive information, all without any user interaction.

### 🟢 Scope of the Bug:
The **"BLASTPASS"** vulnerability was **global**, affecting all iPhone users running the impacted versions of iOS. The exploit's zero-click nature made it particularly dangerous, as any device processing the malicious image was vulnerable, regardless of geographic location.

### 🟢 Manifestation of the Failure:
The failure manifested as **unauthorized access to the device's data**. Users were unaware of the compromise, as no interaction was required to activate the exploit, and it left no immediate signs of intrusion. Sensitive data such as messages, emails, and personal information could be accessed and exfiltrated by attackers.

### 🟢 Repercussions for Clients/Consumers:
For users, this vulnerability posed severe **privacy and security risks**:
- Unauthorized access to personal and sensitive data.
- Increased risk of **identity theft**, **financial loss**, or exposure of **confidential information**.
- The stealthy nature of the exploit left users unaware that their devices were compromised.

### 🟢 Repercussions for the Company:
For Apple, the discovery of such a critical vulnerability had significant **reputational implications**:
- The company had to act swiftly to **develop and deploy patches**, reassure users, and mitigate fallout.
- Despite its reputation for strong security, such incidents can erode **user trust** and confidence in the platform’s security.

### 🟢 Could Testing the Right Scenario Have Helped Discover the Fault?
**Yes**, rigorous security testing could have identified this vulnerability before it was exploited. Specific methodologies include:
- **Fuzz Testing**: Random or unexpected data input to uncover potential security flaws.
- **Code Audits and Reviews**: Focused reviews of the image processing components could have revealed the flaw.
- **Proactive Zero-Click Vulnerability Testing**: Dedicated efforts to simulate zero-click attack scenarios.

Implementing these strategies might have enabled Apple to proactively discover and address this vulnerability, preventing its exploitation in the wild.

----------------------------------------------------------------------------------------------------------------------------------------------------------
2. Apache Commons projects are known for the quality of their code and development practices. They use dedicated issue tracking systems to discuss and follow the evolution of bugs and new features. The following link https://issues.apache.org/jira/projects/COLLECTIONS/issues/COLLECTIONS-794?filter=doneissues points to the issues considered as solved for the Apache Commons Collections project. Among those issues find one that corresponds to a bug that has been solved. Classify the bug as local or global. Explain the bug and the solution. Did the contributors of the project add new tests to ensure that the bug is detected if it reappears in the future?

4. Netflix is famous, among other things we love, for the popularization of *Chaos Engineering*, a fault-tolerance verification technique. The company has implemented protocols to test their entire system in production by simulating faults such as a server shutdown. During these experiments they evaluate the system's capabilities of delivering content under different conditions. The technique was described in [a paper](https://arxiv.org/ftp/arxiv/papers/1702/1702.05843.pdf) published in 2016. Read the paper and briefly explain what are the concrete experiments they perform, what are the requirements for these experiments, what are the variables they observe and what are the main results they obtained. Is Netflix the only company performing these experiments? Speculate how these experiments could be carried in other organizations in terms of the kind of experiment that could be performed and the system variables to observe during the experiments.

5. [WebAssembly](https://webassembly.org/) has become the fourth official language supported by web browsers. The language was born from a joint effort of the major players in the Web. Its creators presented their design decisions and the formal specification in [a scientific paper](https://people.mpi-sws.org/~rossberg/papers/Haas,%20Rossberg,%20Schuff,%20Titzer,%20Gohman,%20Wagner,%20Zakai,%20Bastien,%20Holman%20-%20Bringing%20the%20Web%20up%20to%20Speed%20with%20WebAssembly.pdf) published in 2018. The goal of the language is to be a low level, safe and portable compilation target for the Web and other embedding environments. The authors say that it is the first industrial strength language designed with formal semantics from the start. This evidences the feasibility of constructive approaches in this area. Read the paper and explain what are the main advantages of having a formal specification for WebAssembly. In your opinion, does this mean that WebAssembly implementations should not be tested? 

6.  Shortly after the appearance of WebAssembly another paper proposed a mechanized specification of the language using Isabelle. The paper can be consulted here: https://www.cl.cam.ac.uk/~caw77/papers/mechanising-and-verifying-the-webassembly-specification.pdf. This mechanized specification complements the first formalization attempt from the paper. According to the author of this second paper, what are the main advantages of the mechanized specification? Did it help improving the original formal specification of the language? What other artifacts were derived from this mechanized specification? How did the author verify the specification? Does this new specification removes the need for testing?

## Answers
