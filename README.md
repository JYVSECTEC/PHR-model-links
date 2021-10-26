> Initial release

# Awesome PHR

A curated list of references used in [Prepare-Hunt-Respond (PHR) model](https://github.com/JYVSECTEC/PHR-model).

### Contents 

* [Authorities and communities](#authorities-and-communities)
* [Guides](#guides)
* [Papers](#papers)
* [Blogs](#blogs)
* [Tools](#tools)
* [Resources](#resources)
* [Contribute](#contribute)


### Authorities and communities

**Preparation**

* Police of Finland
  * [FI](https://poliisi.fi/)
  * [EN](https://poliisi.fi/en/frontpage)

* Finnish Transport and Communications Agency - National Cyber Security Centre
  * [FI](https://www.kyberturvallisuuskeskus.fi/)
    * [Kybersää](https://www.kyberturvallisuuskeskus.fi/fi/ajankohtaista/kybersaa)
  * [EN](https://www.kyberturvallisuuskeskus.fi/en/)
    * [Cyber Weather](https://www.kyberturvallisuuskeskus.fi/en/ncsc-news/cyber-weather)

* Finnish pro bono hacker collective KyberVPK - "Depending on the needs of the organization requesting assistance, KyberVPK can help prevent security issues, test the security of customer environments, work together to resolve security breaches, or help with the secure deployment of systems, for example."
  * [FI](https://kybervpk.fi/)
  * [EN](https://kybervpk.fi/en/)

* Cyber threat news and reports
  * [CyWare Monthly Threat Briefing](https://cyware.com/monthly-threat-briefing) - Monthly threat briefing on new cyber threats, breaches, incidents, vulnerabilities, and scams.
  * [CrowdStrike Global Threat Report](https://www.crowdstrike.com/resources/reports/global-threat-report/) - A yearly report highlighting real-world scenarios and new trends. Downloading the report requires registration.
  * [Talos Intelligence Blog](https://blog.talosintelligence.com/) - Quarterly reports, newsletters and blog posts on new cyber threats. 
  * [ThreatPost](https://threatpost.com/) - Cybersecurity related news website.
  * [Security Intelligence](https://securityintelligence.com/) - Another cybersecurity related news website.

### Learning material

* [Jyväskylän yliopiston ja maanpuolustuskorkeakoulun kyberturvallisuuden taskutieto (FI)](https://www.jyu.fi/it/fi/opiskelu/maisteriohjelmat/kyberturvallisuus/kyberturvallisuuden-taskutieto-1)

### Guides

**Preparation**
* [Incident management guide for healthcare organizations](https://jyvsectec.fi/wp-content/uploads/2020/12/kyberhairioiden-hallinta-kasikirja-terveydenhuollon-toimijoille.pdf) - Freely available incident management guide targeted for the Finnish healthcare organizations and operators by JYVSECTEC

### Papers

**Preparation**

* [An AI-based, Multi-stage detection system of banking botnets](https://arxiv.org/pdf/1907.08276.pdf) - JPMorgan Chase engineers propose a "Cyber Data Lake", where data feeds from new domain registrations, benign and malicious domains, known domain fuzzing permutations, internal logs and threat intelligence are combined into a central platform using Big Data tools such as Hadoop and Spark. Deep learning models are trained using features from the platform and provide lexical models and anomaly detection to detect spearphishing and data exfiltration.
* [AI Cybersecurity Challenges](https://www.enisa.europa.eu/publications/artificial-intelligence-cybersecurity-challenges) - ENISA's report about the phases and assets of AI during it's lifecycle but also the emerging threats created or aimed at AI - created models.

**Triage / Respond**

* [Framework for investigating cyber attacks](https://www.nist.gov/publications/d4i-digital-forensics-framework-reviewing-and-investigating-cyber-attacks)

### Blogs

**Preparation**

* [Collecting and curating IoC whitelists for threat intelligence and machine learning](https://medium.com/@jason_trost/collecting-and-curating-ioc-whitelists-for-threat-intelligence-and-machine-learning-research-c5f435431d3e) - Malicious programs may use popular domains and DNS servers for connection checking and address lookups, which can lead to open-source threat intelligence classifying them malicious by accident. The blog contains a number of ways to expand your whitelists to prevent blocking beningn domains.

* [Data Analysis for Cyber Security 101](https://towardsdatascience.com/data-analysis-for-cybersecurity-101-detecting-data-exfiltration-ae887594f675) - A blog series with two posts at the time of writing. In the first post, network traffic visualization methods to detect data exfiltration in a CTF challenge are explored. The second post highlights different methods for lateral movement detection, such as dark space and honey things.

* [Machine Learning Methods for Malware Detection](https://media.kaspersky.com/en/enterprise-security/Kaspersky-Lab-Whitepaper-Machine-Learning.pdf) - Whitepaper by Kaspersky Lab which explains requirements, process of creating and applications of a machine learning malware detection system.

* [Detecting Obfuscated PowerShell using Machine Learning](https://www.fireeye.com/blog/threat-research/2018/11/obfuscated-command-line-detection-using-machine-learning.html) - A blog by FireEye, where a random forest and a neural network model are trained to detect obfuscated PowerShell scripts generated by Invoke-Obfuscation tool.

**Enrichment**

* [Encrypted Traffic Analysis: Use Cases & Security Challenges](https://www.enisa.europa.eu/news/enisa-news/encrypted-traffic-analysis-use-cases-security-challenges) - A report by ENISA, which highlights how features, such as round trip time, number of packets and protocol handshakes, can be extracted from encrypted traffic. A deep learning model trained with these features can for example classify encrypted traffic into streaming, voIP, chat or email. 

**Playbooks**

### Papers
* [Data-driven Threat Hunting using Sysmon](https://www.researchgate.net/publication/325370335_Data-Driven_Threat_Hunting_Using_Sysmon) - A paper proposing a threat assessment system that is updated with new threat information and is able to detect threats what would otherwise go undetected past intrusion detection systems, such as encrypted traffic.

### Blogs
* [How to create and maintain Jupyter threat hunting notebooks](https://expel.io/blog/how-to-create-maintain-jupyter-threat-hunting-notebooks/) - Setup a Jupyter Notebook server with threat hunting notebook templates using Docker.

* [Threat Hunting with Jupyter Notebooks](https://posts.specterops.io/threat-hunting-with-jupyter-notebooks-part-1-your-first-notebook-9a99a781fde7) - A blog series that contains a basic tutorial for Jupyter Notebooks, data analysis with pandas and Apache Spark and SparkSQL usage for querying Elasticsearch databases and combining security events.

**Triage / Respond**

* [Deploy the containerized GRR to unmask the intruders](https://jyvsectec.fi/2020/04/deploy-the-containerized-grr-to-unmask-the-intruders/) - The first post of series focusing on containerized GRR Rapid Response revealing in-depth details how to use tool in real-world scenarios

### Tools

**Preparation**

* [Mordor Dataset](https://mordordatasets.com/introduction.html) - Pre-recorded JSON security event files generated by different attacks which can be used for threat hunting training or as datasets for training machine learning models.
* [IDS 2018 Dataset](https://www.unb.ca/cic/datasets/ids-2018.html) - A dataset from a large virtual environment where multiple attack scenarios are conducted. The dataset contains network logs, UNIX and Windows system logs. Useful for training anomaly detection models or personnel on threat hunting with an publicly available dataset.
* [VirusShare](https://virusshare.com/) - A large dataset of malware, useful for training or evaluating existing machine learning models that are deployed to detect malicious files. Due to the nature of the dataset, access is granted on invitation, which can be requested by email.
* [theZoo](https://github.com/ytisf/theZoo) - An open malware repository, can be used for the same use cases as VirusShare dataset.
* [Windows EVTX Samples](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES) - Windows event logs from different types of attacks, mapped to MITRE ATT&CK tactics. Useful for practicing log analysis and threat hunting.
* [Kybermittari](https://www.kyberturvallisuuskeskus.fi/fi/palvelumme/tilannekuva-ja-verkostojohtaminen/kybermittari) - Incident management and handling tool for Finnish organizations by NSCS-FI
* [Infection Monkey](https://github.com/guardicore/monkey)- An open-source automated penetration testing tool. The tool utilizes a server to command and visualize the exploitation of vulnerable devices in the network. The tool generates a overview security report, a zero trust report and a list of MITRE ATT&CK techniques used. 

**Data Collection**

* [Secure and privacy-preserving machine learning with Crypten](https://ai.facebook.com/blog/crypten-a-new-research-tool-for-secure-machine-learning-with-pytorch/) - Machine learning models are usually trained with unecrypted data, which is problematic when dealing with highly sensitive data, such as medical records. CrypTen enables encrypted tensors for PyTorch framework. Models are also encrypted, and when inference is run, the model output is decrypted.

**Enrichment**  

* [Feature Extractor](https://gitlab.com/CinCan/feature_extractor) - Feature Extractor is a tool that reduces analysts' workload when studying IoCs. Built during CinCan project.
* [Flare](https://github.com/austin-taylor/flare) - A network analytical framework, which provides quick and easy-to-use tools to detect anomalies in network traffic. These include: beacon detection by identifying periodic activity, Domain generation algorithm (DGA) classifier, URL entropy and Levenshtein features.
* [ThreatIngestor](https://github.com/InQuest/ThreatIngestor) - Combine multiple threat intelligence sources into YARA rules and send them forward to MISP. Provides easy automation with simple configuration files.

**Playbooks**

* [HELK](https://github.com/Cyb3rWard0g/HELK) - An open source threat hunting platform built on top of the ELK stack.
* [Threat Hunter Playbook](https://threathunterplaybook.com/introduction.html) - A collection of threat hunter concepts and techniques. Examples of Jupyter Notebooks where attacks from a pre-recorded security log are visualized.

**Triage / Respond**

* [GRR Rapid Response](https://github.com/google/grr) - Google's open source, agent-based Incident Response framework for remote live detection and response written in Python programming language

### Resources

**White papers**
* [RGCE - Realistic Global Cyber Environment](https://jyvsectec.fi/wp-content/uploads/2018/10/JYVSECTEC-cyber-range.pdf) - Fully functional isolated Internet, run, hosted, and developed by JYVSECTEC

**Webinars** 
* [Machine Learning Use Cases for Cybersecurity](https://youtu.be/jmVPLwjm_zs) - A talk by Chris Davis, provides a good overview of machine learning and how it can be applied to cyber security.
* [Leveraging TheHive & Cortex for automated incident response](https://www.youtube.com/watch?v=K6K1fNpbf9w) - A SANS webcast introducing TheHive incident response framework with a usage demonstration.
* [Faster, Better, AND Cheaper: Improving security operations using open source tools](https://www.youtube.com/watch?v=jhOpV9eEeb0) - A SANS webcast listing a number of open source tools for a complete security operations center solution. The SOC solution includes gathering network traffic, host logs and threat information to Elastic stack, alerts are generated using Sigma rules and the incident management and response is automated with TheHive and Cortex.

**Books**

DFIR

* [Incident Response & Computer Forensics](https://www.amazon.com/Incident-Response-Computer-Forensics-Third/dp/0071798684) - Incident responder's and forensic analyst's reference book
* [Data Analytics for Digital Forensics and Cybersecurity](https://www.researchgate.net/publication/320373832_Data_Analytics_for_Digital_Forensics_and_Cybersecurity) - Paper describing the diversity problem in digital forensics - the amount of gatherable data is growing due to more devices and more data being available, and the data is gathered from different operating systems and file formats, where a lack of standard is a problem. The paper presents solutions in deduplication and intelligent automated evidence processing, which would eliminate repetitive work tasks, centralize forensics processing and utilize machine learning to classify relevant evidence.
* [Advancing Automation in Digital Forensic Investigations Using Machine Learning Forensics](https://www.intechopen.com/books/digital-forensic-science/advancing-automation-in-digital-forensic-investigations-using-machine-learning-forensics) - A book chapter with a literature review of machine learning in digital forensics and overview of potential new machine learning applications in the field
* [DF 2.0: an Automated, Privacy Preserving, and Efficient Digital Forensic Framework that Leverages Machine Learning for Evidence Prediction And Privacy Evaluation](https://commons.erau.edu/jdfsl/vol14/iss2/3/) - A proposal for a digital forensic framework that would use machine learning to calculate a "relevance score" for evidence, which would be used to filter the most useful evidence to investigators 

Malware Analysis

* [The Art of Memory Forensics: Detecting Malware and Threats in Windows, Linux, and Mac Memory](https://www.amazon.com/Art-Memory-Forensics-Detecting-Malware/dp/1118825098)
* [Practical Malware Analysis: The Hands-On Guide to Dissecting Malicious Software](https://www.amazon.com/Practical-Malware-Analysis-Hands-Dissecting/dp/1593272901) - Comprehensive book that every malware analysts should read

**Podcasts**
* [Kuulusteluhuone](https://open.spotify.com/show/6TUoUF3WDIdZlQwKCRz8cv) - The official podcast of National Bureau of Investigation of Finland
* [Herrasmieshakkerit](https://www.f-secure.com/fi/business/podcasts/herrasmieshakkerit) - Information security podcast by Mikko Hyppönen and Tomi Tuominen
* [Supodi](https://supo.fi/supodi) - Podcast by SUPO - Finnish Security and Intelligence Service
* [Darknet Diaries](https://darknetdiaries.com) - "This is a podcast about hackers, breaches, shadow government activity, hacktivism, cybercrime, and all the things that dwell on the hidden parts of the network. This is Darknet Diaries."

**Youtube**

* [JYVSECTEC](https://www.youtube.com/channel/UCRD1NIpM6_jDg06_c5mxBrw)
* [SANS Institute](https://www.youtube.com/channel/UC2uPNhGken-ogEpJDi4ly6w)

**Websites**  
* [The National Cyber Security Centre (FIN)](https://www.kyberturvallisuuskeskus.fi/) - Cyber security news and guides targeted on organizations and citizens in Finland
* [The National Cyber Security Centre (UK)](https://www.ncsc.gov.uk/)
* [Police of Finland](https://www.poliisi.fi/rikokset/kyberrikollisuus)
* [SANS](https://www.sans.org/)
* [NIST - National Institute of Standards and Technology](https://www.nist.gov/)

**Standards**
* ISO 27005 - Tietoturvariskien arviointi
* ISO 27043 - Incident investigation principles and processes
* ISO 30121 - Information technology - Governance of digital forensic risk framework
* ISO 31010 - Riskienarviointitekniikat

**Certificates**
* [FINCSC](https://www.fincsc.fi/) - Finnish Cyber Security Certificate by JYVSECTEC

**Miscellaneous**
* [Cyber security terminology (EN to FIN)](https://turvallisuuskomitea.fi/kyberturvallisuuden-sanasto/) - Cyber security terminology translated to Finnish
* [Where to study cyber security?](https://www.jyu.fi/it/fi/tutkimus/julkaisut/it-julkaisut/kyberalan_koulutus_suomessa_verkkoversio.pdf) - A list of Finnish Universities that offers cyber security education and run scientific research (2019)

### Contribute

Are you interested in to contribute? Please read [Prepare, Hunt, and Respond – conceptual model](https://jyvsectec.fi/2019/11/prepare-hunt-and-respond-conceptual-model/) blog post and join in.
