---
tags:
  - cipm
  - privacy
---
## Cybersecurity Goals 
- Confidentiality
- Integrity 
- Availability 

## Relationship between Privacy and Cybersecurity 
- Cybersecurity and privacy programs share the common goal of protecting electronic personal information

## Cybersecurity Controls
- Control objectives are *statements of a desired security state*
- *Security Controls* are specific measures that fulfill these objectives 

### Security Control Categories 
- *Technical Controls* - Enforce CIA in the digital space. Examples include firewalls, ACLs, IPSs, Encryption, etc.
- *Operational Control* - Processes in place to manage technology securely. Examples include user access reviews, log monitoring, vulnerability management, etc. 
- *Managerial Controls* - Procedural mechanisms that focus on risk management. Examples include risk assessments, security planning exercises, service acquisition, etc. 

### Security Control Types 
- *Preventive Controls* - Stop an issue before it occurs 
- *Detective Controls* - Identify events that have already happened
- *Corrective Controls* - Remediate security issues have occurred
- *Deterrent Controls* - Prevent an attacker from attempting to violate security

### Data Protection
- *Data at Rest* - Stored Data that resides on physical media or in the cloud
- *Data in motion* - Data in transit over a network
- *Data in Process* - Data actively being used by a computer system

### Data Encryption
- Uses algorithms to protect information both in transit and at res
- Implementation of encryption include Full-Disk Encryption (FDE) and Transport Layer Security (TLS)

### Data Loss Prevention 
- Enforce information handling policies and procedures to prevent data loss and theft 
- They search systems for sensitive information that might be unsecured and monitor network traffic to detect data ex-filtration attempts 
- They work in 2 different environments 
	- Host-Based DLP 
		- Use software agents to detect sensitive information
	- Network-Based DLP
		- Dedicated devices that sit on the network and monitor outbound network traffic, watching for transmissions

### Data Minimization
- Seek to reduce risk by reducing the amount of sensitive information that organizations maintain on a regular basis
- Best achieved by destroying data when is it no longer needed

- *Deidentification* - Removing the ability to link data back to an individual
- *Data obfuscation* - Transforming data into a format where the original information can't be retrieved. Tools include:
	- Hashing - Transforming a value into a corresponding hash value
	- Tokenization - Replaces sensitive values with a unique ID, maintaining a lookup table to convert back
	- Masking - Partially redacts sensitive informaitno by replacing some or all of the fields 

>[!Note] Hashing is susceptible to rainbow attacks 

### Backups 
- Should be fully addressed in the Disaster Recovery Plan 

- *Full Backups* - A complete copy of the data. Duplicate every file on the system regardless of setting
- *Incremental Backup* - Store only those files that have been modified since the most recent full or incremental backup. Use an archive bit to track each file's backup state
- *Differential Backups* - Store all files that have been modified since the time of the most recent full backup. Only files that have archive bit turned on 

>[!Note] Differential backups are faster to restore but take longer to create than incremental ones

### Cybersecurity Policies 
- *Policies* are broad statements of management intent 
### Cybersecurity Standards
- *Standards* provide mandatory requirements describing how an organization will  carry out its information security policies 
### Cybersecurity Procedures 
- *Procedures* are detailed, step-by-step processes that individuals and organizations must follow in specific circumstances 
- They ensure a consistent process for achieving a security objective
### Cybersecurity Guidelines 
- *Guidelines* provide best practices and recommendations related to a given concept, technology or task
- They are non-mandatory and are offered in the spirit of helpful advice 
### Exceptions and Compensating Controls 
- Organizations should provide mechanisms for exceptions to rules laid out in policy
- Exception processes require the use of *compensating controls* to mitigate the risk
- PCI DSS lays out three criteria for a compensating control to be satisfactory 
	- It must meet the intent and rigor of the original requirement
	- It must provide a similar level of defense as the original requirement
	- It must be 'above and beyond' other PCI DSS requirements
### Key Principles when Develop Policies 
- Obtain input from all relevant stakeholders
- Follow the chain of command 
- Accomodate the organizational culture 
- Meet internal and external requirements 
### Identity and Access Management
- *IAM* programs provide the framework to ensure users are who they claim to be and limit their access to data in a way that allows them to perform their duties 
### Least Privilege 
- A core IAM principle
- It is important for two reasons 
	- It minimizes the potential damage from an insider attack 
	- It limits the ability of an external attacked to quickly gain privileged access when compromising an employee's account 
#### Identification, Authentication and Authorization 
1. *Identification*
	- The individual makes a claim about their identity
	- They may present proof 

2. *Authentication*
	- The individual proves their identity to the satisfaction of the control system

3. *Authorization*
	- The access control system determines if the individual is allowed to access the requested system

### Authentication Techniques
- Something you know
- Something you have
- Something you are 

>[!Note] Multi-factor authentication require the individual to present two of the three authentication techniques 

