#Summary:
To enhance the interaction between local governments and the communities they
represent, we leveraged the power of AI to simplify the complaint management
process for government entities.
#Goal:
Develop a software prototype implementing an algorithm capable of processing social
media or text-based data. This prototype will serve as a proof-of-concept demonstration
to showcase the technology’s potential.
#Problem:
It is often unclear to citizens how to effectively submit issues to their local government
such that action is taken to fix them. The submission process also can vary by issue type
and by jurisdiction.
#Solution:
We developed a proof-of-concept that incorporates the following elements:
• Synthetic email data: To replicate complaints received by the local government,
large-language models were used to generate thousands of emails.
• Text classification: An algorithm was developed to understand the text in the emails,
identifying valuable keywords and word groupings to enable categorization.
We have defined an implementation roadmap for Tyler Technologies to build AI features
upon the proof-of-concept (complaint de-duplication & validation, image classification,
etc.).

#Process:
- *Synthetic Data Generation*: We generated synthetic email dataset using LLMs like ChatGPT, Bard, Llama.
- *Classification*: Emails were classified into benign vs malign using sentiment analysis and deep learning classifier.
- *Issue Categorization*: Categories were inspired from official website of City of Fairfax. Categories were fed into SBert to get vector representations.
- *Clustering*: The vector representations were then used for Clustering via HBDSCAN/K-means.
- *Top-k Topics*: Top-k topics were extracted from the data to get an insight of major problems in the city.

##Implementation Roadmap
<img width="1272" alt="Screenshot 2024-05-10 at 5 59 34 PM" src="https://github.com/aanchal898/CityZen-Automating-govt-citizen-issue-reporting/assets/64893010/a78cc2a9-ea95-488b-95eb-22cd07218c2a">

