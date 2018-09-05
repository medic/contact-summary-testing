# Running Tests With Contact Summary Tests

Contact Summary test will load your contact-settings.js or contact-summary-templated.js. Then it will loop through the folders in your contact summary json exmaple folders. Then execute your contact.json, lineage.json, and reports.json  against the contact-summary. This returns an output json which is then compared against the expected.json in your test folders. 

### Via command line
 
 `medic-contact-summary-test path_to_contact-summary.js path_to_tests_contact_summary_json`

### An example using the standard config tests
  
   `medic-contact-summary-test medic-webapp/tree/master/config/standard medic-webapp/tree/master/config/standard/tests/contact-summary`




## Folder Structure

The json files need to be in this directory structure to be looped over and tested against the contact-summary that gets loaded. 

```
── contact-summary
│   ├── immunization
│   │   ├── contact.json
│   │   ├── expected-output.json
│   │   ├── lineage.json
│   │   └── reports.json
```

