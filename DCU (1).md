# DCU API Document

1. officerLogin
    endpoint: ...officerLogin.php
    {
      "response" : {
        "code" : 200,
        "message": "Success",
        "data": {
    			"user_details": [
    				{
                   "device_token": 1,
                    "officer_email": ""
                    "officer_password": ""
    		    },
    			],                            
    		}
      },
    }
    

2. Statitics
    endpoint: ...updateStatistics.php
    params: [ `institution_id, user_id, device_token' ]
    {
      "response" : {
        "code" : 200,
        "message": "Success",
    		"data": {
    "statistics": [
      {
        "total_applictions": "100",
        "pending_applications": "40",
        "approved_survey": "60",
        "refused_survey": "50",
      }        
    ],
    "applications": [
      {
        "id": "1",
        "application_number": "DCU20231234",
        "applicant_name": "Hassan Bhagash",
        "application_type": "normal building application",
        "application_location": "Mlandege",
        "offer_no": "DCU.09",
        "status": "New",
    
       }
    ],
    "surveys": [
      {
        "id": "1",
        "application_number": "DCU20231234",
        "applicant_name": "Hassan Bhagash",
        "application_type": "normal building application",
        "application_location": "Mlandege",
        "offer_no": "DCU.09",
        "status": "New","     
       },
    ],
      },
      },
      },

3. Reset Password
      endpoint: ...resetPassword.php
 {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Contant Applicant": {
        "id": "1",
        "officer_id": " ",
        "institution_id": "",
        "old_password": "",
        "new_password": "",
        "confirm_password": "",                 
      }
    }
  }
 }
 
 
 4  .Applications
  endpoint: ...getApplicantions.php
  params: [ `institution_id, user_id,device_token]
 {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Applications": {
        "id": "1",
        "institution": "",
        "application_number": "",
        "applicant_name": "",
        "applicant_phone": "",
        "application_type": "",
        "application_location": "",
        "application_address": "",
        "status": "",   
        "offer_no": "",
        "application_descption": "We have reviewed the documents and application form visit the site for  survey",
        "attachment": "*.pdf",
        "initiated_date": "",       
        "contant_applicant": "",
        "reason_for_contant": "",        
      }
    }
  }
 }
 
 
 5. Applications By ID
    endpoint: ...getApplicationsById.php
    params: [ `device_token, user_id,institution_id,applications]
 {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Applications by ID": {
        "id": "1",
        "institution_id": "",
        "officer_id": " ",
        "application_id": "",                 
      }
    }
  }
 }
 
 
 6. Contant Applicant
    endpoint: ...contantapplicant.php
    params: [ `institution_id, user_id,application]
   {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Contant Applicant": {
        "officer_id": " ", 
        "application_id": "",
        "institution_id":"",
        "reason_for_contant": "",        
      },
    },
  },
  },
  
   7. initiatedDate
    endpoint: ...saveinitiatedDate.php
    params: [ `institution_id, user_id,application]
   {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Contant Applicant": {
        "id": " ", 
        "application_id": "",
        "application_number":"",
        "date": "",        
      },
    },
  },
  },
  
  
   8. Surveys
    endpoint: ...saveSurvey.php
    params: [ `institution_id, user_id,device_token]
   {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {      
      "Save Survey": {
        "officer_id": " ", 
        "application_id": "",
        "institution_id":"",
        "plot_area": "",        
        "built_up": "",        
        "number_parkings": "",        
        "plot_coverage": "",        
        "plot_ratio": "",        
        "number_stories": "",        
        "frontage": "",        
        "rear": "",        
        "side1": "",        
        "side2": "",        
        "existing_structure": "",        
        "existing_intrastructure": "",        
        "other_features": "",        
        "descprition": "",        
      },
    },
  },
  },
  
  
   9. All Survey
    endpoint: ...getSurveys.php
    params: [ `institution_id, user_id,survey]
   {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Contant Applicant": {
        "id": " ", 
        "officer_id": " ", 
        "application_id": "",
        "institution_id":"",                
        "status":"",                
      },
    },
  },
  },
  
  
   10. Survey By ID
    endpoint: ...getApplicationsById.php
    params: [ `device_token, user_id,institution_id]
 {
  "response": {
    "code": 200,
    "message": "Success",
    "data": {
      "Applications by ID": {
        "id": "1",
        "institution_id": "",
        "officer_id": " ",
        "application_id": "",                 
      }
    }
  }
 }
  
  


    
