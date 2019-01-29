## greet
* greet
    - utter_greet

## thank
* thank
    - utter_thank

## bye
* goodbye
    - utter_bye



## check_service
* checkservice
    - action_example



## unknown
* unknown
    - utter_unknown
	
## jenkins build
* st_jenkin
	- utter_ask_appname
* inform{"app_name": "Test_Job"}
	- slot{"app_name": "Test_Job"}
	- action_jenkins
	
## Generated Story -7546783482923213326 (to trigger jenkins build)
* greet
    - utter_greet
* st_jenkin{"jenkins": " jenkins"}
    - slot{"jenkins": " jenkins"}
    - utter_ask_appname
* inform
    - utter_ask_appname
* inform{"app_name": "test_job"}
    - slot{"app_name": "test_job"}
    - action_jenkins


## Generated Story 2317895387566703737 (to trigger jenkins build)
* greet
    - utter_greet
* st_jenkin{"jenkins": " jenkins"}
    - slot{"jenkins": " jenkins"}
    - utter_ask_appname
* inform{"app_name": "test_job"}
    - slot{"app_name": "test_job"}
    - action_jenkins
* goodbye
    - utter_bye
    - export
		

## Generated Story -7410773716680088475 (to triger a jenkins job with parameters)
* greet
    - utter_greet
* st_jenkinp{"jenkins": " jenkins", "with_param": "with parameters"}
    - slot{"jenkins": " jenkins"}
    - slot{"with_param": "with parameters"}
    - utter_ask_appname
* inform{"app_name": "sampleapp"}
    - slot{"app_name": "sampleapp"}
    - utter_ask_param
* inform_para{"param": "environment", "pvalue": "uat"}
    - slot{"param": "environment"}
    - slot{"pvalue": "uat"}
    - action_jenkins_param
* goodbye
    - utter_bye
	

		



