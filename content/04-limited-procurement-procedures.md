# **Limited procurement procedures**

# **Direct Award**
CA is able to maintain the registration of information regarding single source procedures carried out of the eProcurement system and the execution of the process inside the system as well. Having entered the information regarding the procedure, CA enters information on the winner and the agreement. 
The procurement process is carried out in the following sequence:

![image](images/1.png)

## **Publication of a decision on intent to conclude an agreement**
CA publishes the concluded agreement and enters information regarding the EO immediately. This information is published as a report on the concluded agreement. It is not possible to submit a complaint at this point.
## **Entering information on EO on the basis of the concluded agreement**
CA enters information on EO on the basis of the concluded agreement. Editing is possible only until the report activation made by CA. Additionally CA notes compliance with qualification criteria for a certain EO on the agreement. Once the EO is determined, no further actions are performed by the CA.
## **Concluding an agreement**
Once the EO information is entered, CA can publish the concluded agreement. Conclusion of agreement, report on the introduced changes into the agreement, and execution of agreement are executed in the following way:
   * Changes of the agreement’s status to active or terminated, should be certified with EDS as a matter of course.
   * Entering information on the agreement is optional. Upon affixation of EDS, CA can finish the procedure (complete).
## **Procedure completion**
Once the agreement was uploaded and EDS added, the procedure automatically changes to ‘complete’ status.

## **Transport model**
CN described as Record Package consists of four (at least) or more Release Packages: 
* ‘cnParent’ (hi-level common data of Contract Notice and a budget of procurement)
* ‘cnDetails’ with all other CN data (depends on the starting point (stage): PN, PIN or CfC (PS/PQ/EV)
* ‘eiDetails’ (hi-level common data of used EI)
* At least one ‘fs’ (detailed information about used FS)

```
{
  "uri": "",
  "version": "",
  "extensions": [],
  "publisher": {},
  "license": "",
  “publicationPolicy”: "",
  "publishedDate": "",
  "packages": [
    "uri of EI release package",
    "uri(s) of FS(s) release package(s)",
    "uri of CN hi-level release package",
    "uri of CN details release package"
  ],
  "records": [
    {
      "description": "This Compiled release includes CN's hi-level",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/cnParent"}
      }
    },
    {
      "description": "This compiled release includes CN's details",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/cnDetails"}
      }
    },
    {
      "description": "This compiled release includes FS details",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/fs"}
      }
    },
    {
      "description": "This Compiled release includes EI's hi-level",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/ei"}
      }
    }
  ]
}

```


## **Query models**

### **contractNoticeParent (cnParent) Query Model**
![table](tables/cn_parent_query_model.csv)

## **Command model**

