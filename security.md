# Strengthen your AI data privacy and security with watsonx on IBM Cloud

By [Rachana Vishwanathula](https://developer.ibm.com/profiles/rachvis1), Preethi Mohan, Deepak Rai  
24 May 2024  

---
If you're a developer, or if you're operating a business, you know that data privacy and protection
for [generative AI](https://www.ibm.com/topics/generative-ai?utm_source=ibm_developer&utm_content=in_content_link&utm_id=articles_awb-data-privacy-security-watsonx-workloads-ibm-cloud&cm_sp=ibmdev-_-developer-articles-_-ibmcom) solutions are non\-negotiable. [IBM watsonx on IBM Cloud](https://www.ibm.com/watsonx?utm_source=ibm_developer&utm_content=in_content_link&utm_id=articles_awb-data-privacy-security-watsonx-workloads-ibm-cloud&cm_sp=ibmdev-_-developer-articles-_-ibmcom), an AI and data platform for
business, has multi\-level security for every aspect of your IT: datacenter,
infrastructure, network, cloud, storage, data at rest and transit, and AI
models. It also meets multiple compliance requirements and provides numerous
ways to secure different types of data on the cloud.


Every AI developer and architect working on generative AI solutions has to implement security
measures. The bottom line? You need a trusted partner to help you thwart
malicious actors. Read on to learn more about the strict security measures
available on IBM Cloud and watsonx. You'll learn:


* How IBM secures the services in  its data centers and the measures we follow to protect customer data
* The types of data you can use  with the services without violating compliance rules, even when the
 services are available in data centers in different countries
* How to effectively manage and  optimize your workloads with other services to enhance data and network  security


## Governmental security requirements


Governments are rapidly increasing security requirements around data privacy and protection. For
example, in August 2023, India's Parliament passed the [Digital Personal Data Protection (DPDP) Act, 2023](https://en.wikipedia.org/wiki/Digital_Personal_Data_Protection_Act,_2023?utm_source=ibm_developer&utm_content=in_content_link&utm_id=articles_awb-data-privacy-security-watsonx-workloads-ibm-cloud), the first cross\-sectoral law on personal data protection in that country's history.


Following are some of the key points from the legislation that organizations must pay particular
attention to:


* The law allows cross\-border
 transfer of data, with restrictions on certain countries, per a list
 provided by the central government. This "negative list" of
 countries has yet to be communicated.
* Data processing includes
 collection, storage, use, sharing, erasure and destruction of
 "personal data" in digital form, or in non\-digital form that is
 subsequently digitized.
* If there is a higher degree of
 restriction on transfer of personal data outside India in any other law,
 then those restrictions must be followed. Accordingly, sectoral laws (like
 the Reserve Bank of India’s localization mandate for payment system data)
 will continue to be applicable.


There are significant penalties for non\-compliance:


* Up to INR 10,000 (approximately
 USD 120\): Breach in observance of data principal
* Up to INR 200 Crore
 (approximately USD 24 million): Breach in not giving notice of personal
 data breach
* Up to INR 200 Crore: Breach in
 observance of additional obligation in relation to children
* Up to INR 250 Crore
 (approximately USD 30 million): Non\-compliance of the provisions by data
 fiduciaries


The key takeaway is this: any company operating in India needs to be aware that the new law spells
out requirements on cross\-border data transfers and establishes significant penalties for organizations that breach those requirements. Other jurisdictions,
including the United States, are establishing their own requirements and penalties. If you're processing data in the world's largest economies, you need
to follow these regulations.


## Security and watsonx on IBM Cloud


So, you know your organization has to take security extremely seriously. Not only is your
company's reputation at stake if you have a security breach, but you face the possibility of significant fines of you don't take steps to protect your
customers. But who can you trust with your data? Who has the established procedures, sites, and infrastructure to protect you and your customers?


The answer to that question is IBM. With its long history of data expertise and protection, IBM
now applies its multi\-level security protocols to AI data and processes.

Following are just some of the security measures that IBM Cloud data centers provide for watsonx services. As you'll see, IBM's generative AI solution on IBM Cloud puts security at the heart of every feature and function.


## Secure data sites


The watsonx infrastructure resides on the IBM Cloud platform, which has undergone independent audits for compliance with [SSAE16](https://ssae-16.com/?utm_source=ibm_developer&utm_content=in_content_link&utm_id=articles_awb-data-privacy-security-watsonx-workloads-ibm-cloud) Type II SOC 1, 2, and 3 standards, as
outlined by the American Institute of Certified Public Accountants. Physical security of IBM property employs a multi\-layered approach encompassing site,building, data center, and data center partitions. Employee access to systems hosting watsonx on IBM Cloud is restricted based on job requirements. Building security is tiered according to security categorization, employing measures such as:


* Gates
* Badge locks
* Cipher locks
* Key locks
* Biometrics
* Video monitoring
* Access logs


Notably, data centers lack first\-floor windows, and emergency doors are equipped with alarms.


## Geography


Watsonx on IBM Cloud is available in secure facilities in Dallas and Frankfurt, and the service requires a cloud object storage instance where the data is stored. Watsonx services uses a highly available infrastructure that uses multi\-zone regions.
Each service is deployed in three data centers in a region. Any data that is needed for use within the service is replicated between each data center to provide high availability.


## Zero retention


Watsonx services are stateless in nature on IBM Cloud, which means that even though the data is
processed, it is not stored by the services. The data is used only until the transaction is completed. Once the transaction is over, the data is not retained by watsonx services.


## Cryptography


IBM employs the latest technically feasible cryptography technologies, such as TLS/SSL, IPSEC, third\-party CAs, encrypted file systems, encrypted storage systems, and key management systems to encrypt data at rest. Watsonx services accept and send client data over the internet only by using HTTPS through TLS connections.


## Defense in depth


Watsonx uses the *defense in depth* concept throughout its security stack to ensure visibility and control. Within the network security stack,
there are multiple layers of security controls:


* Inspection
* Detection
* Isolation
* Directive
* Responsive
* Preventive


At each layer of the network stack, from physical to application, logs are captured, consolidated, and analyzed. Load\-balancing, DNS spoofing, and DDoS solutions are used to ensure defence from attacks against availability.


## Detection and response


Watsonx services employ artificial intelligence for cybersecurity and leverage threat intelligence feeds to safeguard client data. The watsonx security team uses the [IBM QRadar Security Information and Event Management (SIEM)](https://www.ibm.com/products/qradar-siem?utm_source=ibm_developer&utm_content=in_content_link&utm_id=articles_awb-data-privacy-security-watsonx-workloads-ibm-cloud&cm_sp=ibmdev-_-developer-articles-_-product) system for proactive monitoring, detection, tracking, and response to threats that attempt to compromise watsonx and maliciously access data.


IBM ensures real\-time monitoring of activities, both internally and externally, through the use of firewalls, servers, and application APIs. This comprehensive monitoring solution enables the security team to swiftly address potential security breaches or incidents.


## Compliance


Watsonx instantiation on IBM Cloud involves two services: Watson Studio and Watson Machine Learning. In the landscape of AI use cases, customers utilize various data types. Within the cloud paradigm, data often spans international borders when services are available in different countries. Considering the compliance laws, here are a few categories of data that can be used with watsonx services on IBM Cloud without violating any compliance rules.


## Personal data types


The following personal data types are or can be processed as content:


* **Basic personal  information** about the identity of an
 individual, such as name, address, phone number, email
* **Technically identifiable personal information**, such as device IDs, asset identifiers, usage\-based identifiers, static IP addresses, online access and authentication credentials, online  connections, and network connectivity data, when linkable to an individual
* **Employment and education related identifiable information**, such as job history, job role, performance  review information, employment contract, professional education, resume,  language proficiency, education level, or professional association
* **Personality related  identifiable information**, such as personality insights or sentiment analysis, habits and  activities, opinions, personal preferences and interests, club membership
* **Economic and  financial information**, such as
 credit card, bank account, financial holdings, salary information, tax  statements, stock compensation
* **Location information**, such as geolocation data, appointments,  schedules, calendar entries
* **Behavioral biometrics** processed to identify patterns, not  individuals
* **Government identification numbers**, such as  passport number, social security number, government identity card,  individual identifier, vehicle identifier


Special categories of personal data:


The following special categories of personal data are or can be processed as content:


* **Personal data  revealing racial or ethnic origin**, such as ethnic group, ethnicity, race
* **Personal data  revealing political opinions**, such as political party membership, political activity, personal
 political voting
* **Personal data  revealing religious or philosophical beliefs**, such as ideological activity or belief, individual religion type, philosophical activity or belief, religion, religious activity, or affiliation
* **Personal data revealing trade union membership**
* **Genetic data**, such as DNA sequence, genetic inheritance, genomic data
* **Biometric data**, such as biometric identifier, facial geometry or image, fingerprint, voice signature, retina scan
* **Data concerning a person's sex life or sexual orientation**, such as individual sex life, sexual orientation, or affectations
* **Healthcare information**, such as alcohol screening, blood type, disability status, drug screening, health status, medical
 condition, illness, medical condition, diagnosis or records, mental health  status
* **Non\-personal health data**, such as aggregated data across a population (for example, data on large scale epidemics)
* **Non\-personal criminal  data**, such as general area crime  rates


## Security levels


The following security levels are in place for watsonx.ai on IBM Cloud, IBM's enterprise studio for training, validating, tuning, and deploying AI models:


### Security and privacy for foundation models


Foundation models that you interact with through watsonx are hosted on IBM Cloud. Your data is not sent to any third\-party or open source platforms.


The foundation model prompts that you create and engineer in the Prompt Lab or send by using the API
are accessible only by you and are submitted only to models you choose. Your prompt text is not accessible or used by IBM or any other person or organization.


You control whether prompts, model choices, and prompt engineering parameter settings are saved.
When saved, your data is stored in a dedicated IBM Cloud Object Storage bucket that is associated with your project.


Data that is stored in your project storage bucket is encrypted at rest and in motion. You can delete
your stored data at any time.


if !vml![IBM watsonx data security](secure.fld/image002.png)endif *Figure 2: IBM watsonx data security*


* **Foundation model
 developer**: You can use watsonx.data to
 gather all the required data to build a foundation model, in both  structured and unstructured formats and stored in various databases and  object stores. When building a foundation model, use watsonx.governance to  monitor the data to enable data lineage and capture regulatory compliance  parameters.
* **Prompt engineer**: You can use watsonx.ai to identify the  appropriate foundation model and build the model prompts required for a  solution. When a model is deployed in production, use watsonx.governance  to monitor the model performance. Based on the insights from the monitored  data, a foundation model developer can improve the model performance.
* **Customer**: When you use the application for your business needs, it inferences the foundation model integrated with the solution.  Its output data is monitored by watsonx.governance for bias and drift.


Data stored in these databases and object stores can be protected using IBM Key Protect and IBM Hyper Protect Crypto services with shared and dedicated Hardware Security Modules.


## Network security


if !vml![watsonx network security](secure.fld/image003.png)endif *Figure 3: IBM watsonx network security*


Watsonx services and other services on IBM Cloud are hosted in the same data centers, preventing any performance issues such as latency. Watsonx services use IBM Cloud Object Storage to store the data and metadata. If secure connections are enabled, this communication can be changed to the customer’s preferred network. Private network endpoints can be configured by enabling secure connections, which will let watsonx services communicate over a private network on IBM Cloud data centers.


If the data is behind a firewall and within enterprise networks, watsonx services can access it in two ways:


* **Physical private  network**: A direct link connector can be
 used to physically connect the data sources with the data center that  hosts watsonx services.
* **Public network**: An IPsec VPN can be used to create virtual point\-to\-point connections using tunneling protocols, encryption, and  dedicated connections, providing a secure method for sharing data across  public networks.


## Resiliency


IBM watsonx has built\-in disaster\-resistant features, meaning your data is protected when the unforeseen occurs:

* The metadata of your projects and
 catalogs is stored in a three\-node dedicated Cloudant Enterprise cluster  that spans multiple geographic locations.
* The files that are associated  with projects and catalogs are protected by the level of resiliency that  is specified by the IBM Cloud Object Storage plan.


## Summary


Security must be at the top of any organization's IT priorities. Beyond the reputational and financial damage that can occur due to a security breach, organizations are increasingly subject to legislation that makes security protections mandatory.


Every solution provider that manages data and includes AI models must make a commitment to security and recognize its own responsibility to customers. There is a critical need for partners that can both help them adopt AI technologies *and* protect customer data.


IBM knows how to do security. IBM watsonx has multi\-level security built in, and watsonx on IBM Cloud gives your company the ability to meet security requirements, protect customers, and ensure compliance at every stage of your business. That expertise and commitment to security will give you — and more importantly, your customers — peace of mind.
