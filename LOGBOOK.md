# Gibber Logbook

## Goal 
Create a language model which can be prompted with a specific topic (e.g machine learning) and will return a tweet length response about the topic

## Timeline
### 2023-02-20 18:57 ET: [Kadeem] Setting up project in Azure
Got a dead simple version of the application running end to end in Azure. It's a simple character level bigram model so performance isn't great but it's a fun start. UI is even simpler with just a button to send an HTTP request to a REST API wrapping the model. 

Considerations for next steps:
- Model: Change to word level n-gram model, may be able to use simple BOW representation to start but could explore other alternatives
- UI: Noticed some display issues when changing resolution on the frontend so will need to take resolution into consideration when sizing the UI elements
- Infrastructure: Lots of work to be done here, need a clear deployment procedure (building, packaging etc..), took some shortcuts installing required software directly onto the VM, may need a hard reset of that machine
