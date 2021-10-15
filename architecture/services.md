---
description: which service corresponds to which function of the application?
---

# Services



#### Auth <a href="auth" id="auth"></a>

* `FindAuthenticatedGoogleAccount`: service to return an authenticated user, or nil. e.g. id, email, username, access_token

#### Outputs <a href="outputs" id="outputs"></a>

* `TransformResponsesToCSV`: service to transform Launch.responses to CSV file
* `TransformDBSurveyToHTML`: service to create HTML strings: title & array of each survey page
* `TransformSheetsSurveyToHTML`: service to create HTML strings: title & array of each survey page

#### Responses <a href="responses" id="responses"></a>

* `StoreResponses`: send message(responses_hash) to queue

#### Retrieve Surveys <a href="retrieve-surveys" id="retrieve-surveys"></a>

* `GetSurveyFromDatabase`: return an entity of survey from database
* `GetSurveyFromSpreadsheet`: return an entity of survey from spreadsheet

#### Ｍanage Surveys <a href="anage-surveys" id="anage-surveys"></a>

* `StartSurvey`: get update survey in spreadsheet then store in db and return the updated survey
* `CloseSurvey`: close the survey and launch, return launch entity with close state

#### Modify Surveys <a href="modify-surveys" id="modify-surveys"></a>

* `CreateSurvey`: create a new template survey
* `CopySurvey`: copy the survey to a new one
* `DeleteSurvey`: delete survey in db and spreadsheet, return delete_survey
* `UpdateSurveyOptions`: return updated survey entity with new option, only db is updated
* `EditSurveyTitle`: return updated survey entity with new title, both spreadsheet and db are updated
