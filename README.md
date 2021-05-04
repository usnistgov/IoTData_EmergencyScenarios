#
#
# IoT Data: Emergency Scenarios Repository 

The NIST IoT Data:  Emergency Scenarios data repository is an online venue open to the public where interested parties can access emulated IoT data related to four specific emergency scenarios.  This data demonstrates situational awareness information that would be provided to a first responder or an incident commander during a mission critical event.

## Scenarios

* **Active Shooter:**  The active shooter scenario portrays a shooting incident within an office complex.  Law Enforcement officers are the primary first responder types targeted for the data provided.

* **Flood:**  The flood scenario demonstrates a large scale heavy rain event with corresponding emergency response throughout the city.  Fire Service, Emergency Medical Service and Law Enforcement personnel all can utilize the data provided within the scenario.

* **Mass Transit Accident:**  The mass transit accident scenario portrays a train derailment and associated fire.  The train cars are in various states of accessibility, and the tunnel where the crash occurs further limits the visibility of the first responders.  Emergency Medical Service and Fire Service personnel would be the primary users of this data.

* **Wildfire:**  The wildfire scenario demonstrates a large-scale burn event beginning in remote areas and spreading to more populated areas.  Fire Service and Emergency Medical Service personnel are the primary first responder types targeted for the data provided.

Within the folder for each scenario, an additional README file will provide additional details regarding the scenario, as well as the data provided.

## Contribute to the Space 

* By contributing to this space all individuals, groups or organizations will be required to abide by the Rules_of_Behavior.txt document.
* By contributing to this repository it is assumed that you have read and will abide by the terms in the Rules_of_Behavior.txt.
* Contributions may be renamed, moved or deleted without prior notification. Always create local backups or working backups of your contribution(s).

Contributions come in three categories:

1. **Tool:** A tool can be an open source solution or process, ranging from software to frameworks. Examples may include IoT generators, data stores upon which IoT data is generated or simulated/emulated first responder (persons) actions or bio-metrics. DISCLAIMER: Do not include identifiable information in submission data or tools as described in the Rules_of_Behavior.txt document.

2. **Scenario or Use Case:** A scenario is an example of an first response event, e.g. fire or earthquake. A use case is a situation where a tool or IoT data is applicable to different first response events, and not specific to any one scenario. In other words, the tool can be used in multiple first response scenarios.

3. **Feedback:** Help the community. Provide feedback on tools, scenarios and use cases.

Tools, scenarios and use cases are contributed via pull requests, while feedback is contributed via issues. Contributed tools and use cases can be hosted directly in this repository, or you can host them elsewhere online and link to them from this repository.

### How to Contribute Tools, scenarios and Use Cases

1. Fork a copy of /usnistgov/IoTData_EmergencyScenarios/ to your own organizational or personal space. 

2. Create a branch in your fork, named specifically for your contribution. 

3. In your branch: 

3.a. Create a new directory within the relevant scenario or create a new directory reflecting a scenario not listed.
3.a.i. example: directory: wildfire/<teamname>, transit/<name>, tornado/<companyname>	

3.b. Include in the directory a README_<scenario_name>.md file in each scenario directory describing the submission
3.b.i. example: README_wildfire.md

3.c. If hosting a tool in this repository, also include in the directory any pertinent source code files or documentation. Sub-directories with relevant source code or descriptive files are allowed. Please do not include any "closed-source" or proprietary code, code that includes "hard coded" values, such as IP addresses, keys, passwords, etc. Identifiable information, such as addresses, names, birth dates, etc. Geo-tagged or coordinate data may be considered identifiable, consider location randomization or a wide location area if this information is included. Do not include any potentially or otherwise malicious code. Such code will result in a permanent ban to this repository.

3.d. If more than one datasets, tools, source code, etc. are being provided to the contribution, aptly name the submissions to reflect it's unique use case within the scenario directory.

example: Submission 1: tornado/<teamname>/city/iotData.txt
example: Submission 2: tornado/<teamname>/rural/iotData.txt

3.e. Update the README_<scenario_name>.md file of the main scenario directory to which you’re contributing. This README provides an index of that directory's contents. It should include an entry reflecting your contribution. More than one README can be submitted if it enhances viewers/users understanding of your submission.	

4. Create a [pull request](https://github.com/usnistgov/IoTData_EmergencyScenarios/pull/new/master) (PR) from your branch to the master branch in USNISTGOV/IoTData_EmergencyScenarios. 

6. Moderators will then review the PR and may provide comments and suggestions to the contributor. 

### How to Contribute Feedback 

Submit an [issue](https://github.com/usnistgov/IoTData_EmergencyScenarios/issues/new) to provide feedback on tools or use cases in the space. Please select appropriate tags related to the feedback. 

### Additional Contribution Resources

**GitHub Help:** If you're having trouble with these instructions, and need more information about GitHub, pull requests, and issues, visit GitHub's Help [page](https://help.github.com/categories/collaborating-with-issues-and-pull-requests/). 

**Contribution Assistance:** If you're having trouble submitting your contribution to this space, or otherwise would like to send us feedback, [contact us](mailto:TBD@TBD.gov). 


## Operating Rules 

NIST will only accept open source submissions, per the Open Source Initiative’s [definition](https://opensource.org/osd) of “open source”. Upon submission, materials will be public, considered to be open source, and may be altered and shared. 

This is a moderated platform. NIST reserves the right to reject, remove, or edit any submission, including anything that: 

* promotes pay-for services or products;  
* includes personally identifiable or business identifiable information according to Department of Commerce Office of Privacy and Open Government [guidelines](http://www.osec.doc.gov/opog/privacy/PII_BII.html); 
* is inaccurate;  
* contains abusive or vulgar content, spam, hate speech, personal attacks, or similar content;
* is clearly "off topic"; 
* makes unsupported accusations; or, 
* contains .exe or .jar file types.* 

*These file types will not be merged into the NIST repository; instead, NIST may link to these if hosted elsewhere. 

## Representations and Warranties & Software Use Agreement 

Any references to commercial entities, products, services, or other nongovernmental organizations or individuals on the site are provided solely for the information of individuals using this page. These references are not intended to reflect the opinion of NIST, the Department of Commerce or the United States, or its officers or employees. Such references are not an official or personal endorsement of any product, person, or service, nor are they intended to imply that the entities, materials, or equipment are necessarily the best available for the purpose. Such references may not be quoted or reproduced for the purpose of stating or implying an endorsement, recommendation, or approval of any product, person, or service. 

This platform is provided as a public service. Information, data, and software posted to this platform is “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the software or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the software. You are solely responsible for determining the appropriateness of using and distributing the software and you assume all risks associated with its use, including but not limited to the risks and costs of program errors, compliance with applicable laws, damage to or loss of data, programs or equipment, and the unavailability or interruption of operation. This software is not intended to be used in any situation where a failure could cause risk of injury or damage to property. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE SOFTWARE (OR THE USE OF OR INABILITY TO USE THIS SOFTWARE), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

## Moderators 
See Rules_of_Behavior.txt document