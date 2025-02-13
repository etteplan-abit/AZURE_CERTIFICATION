# Exam AI-102 practice assessment


## Question 1
You are building an app that will analyze resumes and remove names and addresses.
You need to configure the Azure AI Language Personally Identifiable Information (PII) detection feature for the app.
Which categories should you specify in the request?

- [ ] Person, Address, and IP
- [x] Person and Address only
- [ ] Person, PersonType, and Address

Person and Address will detect names and addresses.

PersonType will also remove job roles. IP will also remove IP addresses.

[Entity categories recognized by Personally Identifiable Information (detection) in Azure Cognitive Service for Language - Azure Cognitive Services | Microsoft Learn](https://learn.microsoft.com/azure/cognitive-services/language-service/personally-identifiable-information/concepts/entity-categories)

[Publish and use a Language Understanding app - Training | Microsoft Learn](https://learn.microsoft.com/training/modules/publish-use-language-understand-app/)


## Question 2
You are building an app that will analyze the sentiment of user feedback by using Azure AI Language.
You have a test document named Test.docx that contains one positive sentence and multiple neutral sentences.
You need to validate the app by analyzing Test.docx.
Which label will the app return for Test.docx?

- [ ] mixed
- [ ] negative
- [ ] neutral
- [x] positive

If there is at least one positive sentence in the document, and the rest of the document is neutral, then the document label is positive.

[How to perform sentiment analysis and opinion mining - Azure Cognitive Services | Microsoft Learn](https://learn.microsoft.com/azure/cognitive-services/language-service/sentiment-opinion-mining/how-to/call-api)

[Extract insights from text with the Language service - Training | Microsoft Learn](https://learn.microsoft.com/training/modules/extract-insights-text-with-text-analytics-service/)


## Question 3
You are building an app that will flag documents that contain the names of staff members by using the Azure AI Language Personally Identifiable Information (PII) detection feature.

You need to configure the PII detection feature.

Which category should you use?
- [x] Person
- [ ] DateTime
- [ ] Age
- [ ] PhoneNumber

The Person category detects names of people in the PII detection feature. The PhoneNumber category detects phone numbers, the age category detects people’s ages, and the DateTime detects dates and time values.

[Entity categories recognized by Personally Identifiable Information (detection) in Azure Cognitive Service for Language - Azure Cognitive Services | Microsoft Learn](https://learn.microsoft.com/azure/cognitive-services/language-service/personally-identifiable-information/concepts/entity-categories)

[Publish and use a Language Understanding app - Training | Microsoft Learn](https://learn.microsoft.com/training/modules/publish-use-language-understand-app/)


## Question 4
