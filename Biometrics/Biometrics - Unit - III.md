# Privacy Enhancement Using Biometrics
## Introduction

>Information security as “protecting information and information systems from unauthorized access, use, disclosure, disruption, modification, or destruction”

Four major aspects of information security:
- Integrity - guard against improper modification or destruction of the data and ensure non-repudiation and authenticity of information.
- Data confidentiality - prevent illegitimate access or disclosure of sensitive information.
- Availability - guarantee timely and reliable access to and use of information.
- Authentication - only legitimate and authorized users should be able to access the data and carry out specific tasks.

>It is generally agreed that biometric recognition can effectively address the authentication problem. 

- Since biometric traits cannot be easily lost, stolen, misplaced, or shared, biometric recognition offers a natural and more reliable authentication solution compared to other techniques such as passwords or physical tokens (e.g., ID cards). 
- This is the reason why biometric systems are being increasingly deployed to control access to other information systems. 

---

## Privacy Concerns associated with the Biometric Deployments

>It is important to realize that a biometric system is just one component of the overall information security solution because it address only the authentication aspect

Other technologies such as encryption, digital signature, etc. are needed to meet the confidentiality, integrity, and availability requirements of the total information system.

If the biometric system is compromised or circumvented, the security of the entire information system gets affected. 

---

## Identity and Privacy

 Privacy refers to the right of the a person to be left alone, i.e., the ability to lead one’s own life free from intrusions, to remain anonymous, and to control access to one’s own personal information (Identity).

When the breach of security in an information system leads to personal and subjective harm to the person involved, it can be termed as loss of privacy.

---

## Privacy Concerns

1. Will the undeniable proof of biometrics-based access infringe upon an individual’s right to remain anonymous?
	- It is often possible to covertly recognize a user by capturing his biometric traits without his active involvement (e.g., face can be captured using hidden surveillance cameras). 
	- As a result, persons who desire to remain anonymous in any particular situation may be denied their privacy due to biometric recognition.
	
2. Will the biometric data be abused for an unintended purpose (function creep), e.g., allowing linkage of identity records across systems without the knowledge of the user? 
	- For example, a fingerprint template obtained from a bank’s database may be used to search for that person’s health records in a medical database.
	- How to ensure that an information system is indeed exclusively using biometric recognition for the intended purpose (e.g., can it be provably demonstrated that the trusted system administrators cannot abuse the system)?

3. Will the requirement of biometrics be proportional to the need for security, e.g. Should a fingerprint be required to purchase a hamburger at a fast food restaurant or access a commercial website?

4. Who owns the biometric data, the individual or the service providers?

---

### 1. *Infringement on the Right to Remain Anonymous*
   - **Concern**: Biometric traits (e.g., face, fingerprints) can be captured covertly, making it difficult for individuals to remain anonymous in public or private spaces.
   - **Privacy Enhancements**:
     - **Anonymization Techniques**: Use biometric systems that store only anonymized or encrypted templates, not raw biometric data. For example, facial recognition systems could use hashed or tokenized representations of facial features.
     - **Consent Mechanisms**: Ensure that biometric data is only collected with explicit user consent. Covert collection should be prohibited by law.
     - **Context-Specific Use**: Limit the use of biometrics to specific contexts where anonymity is not expected (e.g., airport security) and avoid its use in public spaces where anonymity is desired.
   
---

### 2. *Function Creep and Unintended Use*
   - **Concern**: Biometric data collected for one purpose (e.g., banking) could be misused for unrelated purposes (e.g., health records linkage).
   - **Privacy Enhancements**:
     - **Data Segregation**: Ensure biometric data is stored in isolated systems and not shared across databases without explicit user consent.
     - **Auditability**: Implement systems that log all access and usage of biometric data, allowing for independent audits to detect misuse.
     - **Provable Security**: Use cryptographic techniques (e.g., zero-knowledge proofs) to ensure that biometric data is only used for its intended purpose and cannot be accessed or misused by administrators.

---

### 3. *Proportionality of Biometric Use*
   - **Concern**: Requiring biometrics for low-security tasks (e.g., purchasing a hamburger) may be disproportionate and invasive.
   - **Privacy Enhancements**:
     - **Risk-Based Authentication**: Use biometrics only when the security risk justifies it (e.g., high-value transactions or access to sensitive areas).
     - **Alternative Methods**: Provide non-biometric alternatives (e.g., PINs, passwords) for low-security tasks.
     - **User Choice**: Allow users to opt out of biometric authentication when it is not strictly necessary.

---

### 4. *Ownership of Biometric Data*
   - **Concern**: It is unclear whether individuals or service providers own biometric data, leading to potential misuse.
   - **Privacy Enhancements**:
     - **Data Portability**: Allow users to transfer or delete their biometric data from service providers' systems.
     - **Transparency**: Require service providers to disclose how biometric data is stored, used, and protected.
     - **Minimization**: Encourage the use of decentralized systems where biometric data is stored on the user’s device (e.g., smartphones) rather than in centralized databases.

---

### Additional Privacy-Enhancing Technologies

   - **Encryption**: Store and transmit biometric data in encrypted form to prevent unauthorized access.
   - **Liveness Detection**: Ensure biometric systems can distinguish between live traits and spoofed ones (e.g., photos or fake fingerprints).
   - **On-Device Processing**: Perform biometric matching on the user’s device rather than sending data to a central server.
   - **Federated Learning**: Train biometric algorithms without sharing raw data across systems.
   - **Blockchain**: Use blockchain for secure, transparent, and tamper-proof storage of biometric data usage logs.

>Fair information practice principles such as transparency, informed consent, use limitation, accountability, and auditing could be followed to limit the privacy concerns arising from biometric recognition. 
>
>Since these issues are beyond the scope of technology, appropriate legislations must be put in place to enforce these principles.

---

## Comparison of Various Biometrics in terms of Privacy

| Biometric Type     | Data Collected                                            | Privacy Concerns                                                                                        | Potential Misuse                                                        | Accuracy                                             |
| ------------------ | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | ---------------------------------------------------- |
| Fingerprint        | Ridge patterns of fingers                                 | Can be left on surfaces, potential for unauthorized access, database vulnerability                      | Tracking, identification without consent, creation of fake fingerprints | High                                                 |
| Facial Recognition | Facial features (distance between eyes, nose shape, etc.) | Mass surveillance potential, bias in algorithms, tracking without consent, data breaches                | Profiling                                                               | High (but can be affected by lighting, angles, etc.) |
| Iris Scan          | Patterns in the iris of the eye                           | Requires close proximity, potential for data breaches, less common than other biometrics                | Tracking, identification without consent                                | Very High                                            |
| DNA                | Genetic information                                       | Highly sensitive data, reveals ancestry and health information, potential for misuse and discrimination | Genetic profiling                                                       | Very High                                            |

---

## Soft Biometrics 

There are many situations where primary biometric traits (i.e., face, fingerprint and iris) are either corrupted or unavailable, and the soft biometric information is the only available clue to solving a crime.

For example, while a surveillance video may not capture the complete face of a suspect, the face image in the video may reveal the suspect’s gender and ethnicity, or the presence of a mark or tattoo may provide additional valuable clues. 

We will discuss some of the soft biometric traits (i.e., periocular, facial marks, and tattoos) below. 

- The periocular biometric is gaining increasing attention since it offers a trade-off between using the entire face image and the iris portion only. 
- Facial marks and tattoos are also gaining widespread attention since they offer complementary information that can be exploited along with primary biometric traits.

---

### Periocular

>The periocular region represents the region around the eyes. It predominantly consists of the<mark style="background: #FFB86CA6;"> skin, eyebrow, and eye. </mark>

The use of the periocular region as a biometric cue represents a good trade-off between using the entire face region or using only the iris for recognition. 

- When the entire face is imaged from a distance, the iris information is typically of low resolution; this means the matching performance due to the iris modality will be poor. 
- On the other hand, when the iris is imaged at small standoff (typically, 1 meter), the entire face may not be available, thereby forcing the recognition system to rely only on the iris.

>Periocular images can also be captured in the NIR spectrum to minimize illumination variation compared to visible spectrum.

![](attachments/Pasted%20image%2020250213222337.png)
Figure: Example of periocular images from two different subjects.

![](attachments/Pasted%20image%2020250213224019.png)
Figure: Example images showing difficulties in periocular image alignment

![](attachments/Pasted%20image%2020250213224056.png)
Figure: Schematic of image alignment and feature extraction processes for periocular images.

>Periocular images contain common components across images (i.e., iris, sclera, and eyelids) that can be represented in a common coordinate system. 

---

### Face Marks

Advances in sensing technology have made it easy to capture high resolution face
images. From these high resolution face images, it is possible to extract details of
skin irregularities, also known as facial marks.

This has opened new possibilities in face representation and matching schemes. These skin details are mostly ignored and considered as noise in a typical face recognition system.

 However, facial marks can be used to 
 1. supplement existing facial matchers to improve the identification accuracy, 
 2. facilitate fast face image retrieval, 
 3. enable matching or retrieval with partial or off-frontal face images, and 
 4. provide more descriptive evidence about the similarity or dissimilarity between face images, which can be used as evidence in legal proceedings.

![](attachments/Pasted%20image%2020250213223816.png)

>To represent the face marks in a common coordinate system, primary facial features such as **eyes, eye brows, nose, mouth, and face boundary** are detected by using an Active Appearance Model (AAM) or <mark style="background: #FFB8EBA6;">Active Shape Model</mark> (ASM).

![](attachments/Pasted%20image%2020250213224433.png)
**Figure**:  Schematic of the mark detection process.

---

### Tattoos 

When the primary biometric traits are unavailable or corrupted, tattoos can be used to identify victims or suspects.

>Therefore, recognition of tattoos can provide a better understanding of an individuals background and membership in various organizations, especially criminal gangs.

---
# Introduction to Multimodal Biometric

- A multimodal biometric system refers to a system that uses multiple personal traits, such as iris, fingerprints, face, retina, hand geometry, voice, or signatures, for identification and verification purposes.
    
- It combines two or more biometric modalities to provide rich and reliable information, making it more secure and effective than unimodal biometric systems.

---

## Basic Architecture of Multimodal Biometrics

**Sensors**: 

- These devices capture the raw biometric data from different modalities. For example, a fingerprint scanner captures fingerprint images, a camera captures facial images, and a microphone captures voice recordings.

**Feature Extraction:**

- This module processes the raw biometric data to extract distinctive features that can be used for identification or verification. For instance, minutiae points are extracted from fingerprint images, facial landmarks are extracted from facial images, and vocal characteristics are extracted from voice recordings.

**Fusion Module:**

This component integrates the features extracted from different modalities. Fusion can occur at various levels:

1. Sensor Level: Combining raw data from multiple sensors before feature extraction.    
2. Feature Level: Concatenating or combining feature vectors from different modalities.
3. Matching Score Level: Combining the matching scores obtained from comparing      individual modality features with stored templates.
4. Decision Level: Integrating the final decisions made by individual modality classifiers.

**Database**: 
	This stores the enrolled biometric templates, which are the representative features of individuals' biometric traits.

**Matching Module:**
	This compares the extracted features from the input biometric data with the stored templates in the database to generate matching scores or decisions.

**Decision Module:**
	This module makes the final decision based on the matching scores or decisions from the fusion module. It determines whether the individual is recognized or verified based on predefined thresholds.

**Workflow**:

1. During enrollment, individuals' biometric data from different modalities are captured by the sensors.    
2. The feature extraction module extracts relevant features from each modality.
3. The fusion module combines these features at the chosen level.
4. The fused features are stored as a template in the database.
5. During identification or verification, the same process is repeated for the input biometric data.
6. The matching module compares the input features with the stored templates.
7. The decision module makes the final decision based on the matching scores.

### Key Considerations:

**Choice of Modalities:** 
	Selecting appropriate biometric modalities that are complementary and provide diverse information.

**Fusion Strategy:** 
	Determining the optimal fusion level and technique to effectively integrate the information from different modalities.

**Performance Metrics:** 
	Evaluating the accuracy, efficiency, and security of the multimodal biometric system.

**Diagram:**

	[Sensors]-->[Feature Extraction]-->[Fusion Module]-->[Matching Module]-->[Decision Module]
								⬇️

							[Database]

  ---

## Face- and Ear-Based Multimodal Biometrics

1. The ear and the face are less correlated, and the combination of their discriminative information generally improves the recognition performance; 

2. The ear is not affected by facial expressions and aging, and when the face is unreliable or even unavailable, the multimodal system can rely on the ear, and vice versa;

3. It is much more difficult to spoof both the face and the ear simultaneously than to spoof only one; 

4. Both the data collections are contactless, and thus, the multimodal recognition can still operate from a distance and in a nonintrusive manner; 

5. They can share the same feature extraction and matching algorithms, whereby the derived feature sets are compatible for biometric fusion

 6. Benefiting from their physiological location and structure, the multimodal recognition enjoys a wider range of recognition angle in the yaw direction;

 7. The ear and can be captured along with the face by using the same type of sensor or a single sensor at two times; 

 8. Face detection helps speed up ear detection by offering an ear region of interest. Inspired by these attractive features, the face- and ear-based multimodal biometrics has attracted much attention in computer vision community

**Example:**

![13104_2016_2287_Fig4_HTML.jpg](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcbdJIvi_Iw-HEC7ipqNeaOqPtlQ8XYJH6KVNF0fzSSEyeJAdAtdMfp4LiC27ukGdzx64FhCP-fjbD1kd_B_LaOe94Iv7dqbOgob8dK2-PJBf3uN2doAW8JpjUMrUJ2j5-zYz-Iy3G_iGDH-qGu3sU?key=JCalO9zFEjhGcIRQ-yMScWoC)

![images.jpg](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeEkC07SdWClPjzA4QCkdA3IHN3o-LcSoyxBjqRArHlJy2g8fssgboZj4O79z10eYNfM1Uiz5uJod00qq_EhExK0joDRXt3apZK8r4ZAF5EREpvrwkQRo-DiK_RDzHdiGMQOBrfT3DlqO8gT5yGgw?key=JCalO9zFEjhGcIRQ-yMScWoC)![images.png](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf82nuQRCpfowIhBMc8jk67jUIBwjGY1wvX2He4_y2tQ9FikESAuqOTsDknOFRIw-XbFSvPr8fYw_NxZs2CYcBmDspBx89hNAfUCrZ5KlDt3q3YrJ9fWNgLF4YyUmpiO6-Thtf5UAMED3Amflv45A?key=JCalO9zFEjhGcIRQ-yMScWoC)

---

## Characteristics of multimodal biometrics
- **Enhanced Accuracy**: Multimodal biometrics leverages the strengths of multiple biometric modalities, reducing the risk of false acceptances or rejections and increasing overall accuracy.
- **Robustness:** Combining different biometric traits compensates for individual variations, environmental factors, and changes over time, leading to more reliable identification.
- **Security**: The fusion of multiple biometric traits makes it significantly harder for impostors to mimic or spoof the system, enhancing overall security.
- **Flexibility**: Multimodal systems can adapt to various scenarios and user preferences, allowing for a tailored and user-friendly experience.
- **Integration**: These systems can be integrated with existing security systems or databases, making them suitable for a wide range of applications, from access control to digital payments.
- **Continuous Authentication**: Multimodal systems can provide continuous authentication by constantly monitoring and validating multiple biometric traits, enhancing security in real-time.
- **Adaptability**: Multimodal systems can adapt to changing conditions or injuries that might affect one biometric modality, ensuring reliable identification.
## Advantages 
- **Enhanced Accuracy:** Combining multiple biometric modalities improves the accuracy of identification and reduces the likelihood of false positives and false negatives.
- **Increased Security**: Multimodal biometrics provide a higher level of security by making it difficult For attackers to simultaneously spoof multiple biometric traits.
- **Robustness**: The system remains reliable even in situations where one biometric modality might fail due to injuries, changes over time, or environmental conditions.
- **Reduced Vulnerability to Spoofing**: It becomes more challenging for attackers to successfully mimic or spoof multiple biometric traits, enhancing overall system security.
- **User-Friendly:** Users have the flexibility to choose the biometric modality that suits their preferences, making the system more user-friendly. 
- **Privacy**: Multimodal systems can be designed to use non-sensitive biometric traits, preserving user privacy while still maintaining security.

## Disadvantage
- **Complexity and Cost:** Implementing multimodal biometrics can be more complex and costly due to the need for multiple sensors, hardware, and data processing techniques.
- **Integration Challenges:** Integrating multiple biometric modalities into existing systems might require additional effort and resources.
- **Performance Trade-offs:** The enhanced accuracy comes at the cost of increased computational complexity, potentially leading to slower response times.
- **Ethical Concerns:** Collecting and storing multiple biometric traits raises ethical concerns related to user consent, privacy, and potential misuse of sensitive data.
- **User Acceptance:** Some users might find the use of multiple biometric modalities cumbersome or overwhelming, impacting user acceptance.
- **Data Storage and Management**: Storing and managing data from multiple biometric traits requires effective data security measures to prevent breaches.
- **Error Propagation:** If one of the biometric modalities has errors or inaccuracies, they can potentially affect the overall accuracy of the system.

---