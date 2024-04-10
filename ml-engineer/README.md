Dear Candidate,

Thank you for expressing interest in the ML position at Captonomy Consulting. To assess your expertise in machine learning concepts and applications, we have a scenario for you to address. Please note this is a hypothetical scenario, and we're not expecting a detailed technical solution or actual code. Instead, we're interested in your high-level approach and strategic thinking. It's important to note that generic or auto-generated responses won't align with our expectations. We seek genuine insights that showcase your understanding and innovative problem-solving abilities.

### Scenario 
Your task is to devise a model capable of extracting structured information from a collection of digital (raster) document images (e.g., invoice, utility-bill, bill-of-lading, tax forms etc). These documents exhibit semi-structured characteristics, wherein predefined fields such as *name*, *amount*, *address*, *Total amount*, etc usually exist in this type of document (each type of document has different *predefined* fields). The challenge lies in identifying these fields **accurately** across diverse document layouts. If your approach is based on text processing you may assume that the image can be converted to textual form, including spatial information, using an OCR engine, yet the quality of the OCR is not always very good (e.g. hard-to-read handwritten info, badly-digited documents, etc).

Remember that your solution should differ from the way a current LLM treats information (which is to generate data in a semi-random way): in our example we need our model to give us a definite (positive or negative) answer and an exact, few-word, structured reply (e.g. when asking "what is the total for this utillity-bill?" it should either give the exact number or reply "do-no-know" and not produce some random number).

#### Goal
The goal is to create a solution that **requires no training at all** to begin extracting information from structured documents that has never seen before and has not been trained on, more or less as a human would do. Your solution should be able to get better by time on document types (or layouts) that has seen before but without extensive re-training (e.g. no retraining of model from scratch).

#### Challenges
- Variability in field positions across images due to diverse document layouts.
- Definitive answers with 100% confidence (a "do-not-know" answer is preferrable from a 80%-certainty answer since both will require a human to inspect/validate)
- Limited or no labeled data for training, necessitating robust feature engineering.
- Managing uptraining strategies effectively to fine-tune existing Language Models (LLMs) or build models from scratch for improved performance.
- Mitigating the risks of hallucinations or generating spurious information while ensuring grounding of extracted data to maintain accuracy and reliability.

#### Example
Assuming the goal is to extract two fields, specifically the **Invoice Number** and **Invoice Total**, for **both** of these images and the results should be the same. **Do not assume** that you are tasked to build a solution that specifically targets invoices of this type, or invoices in general: **the task is to be able to handle such a problem without having to re-train a model for ANY type of specific document type**.

![InvoiceA](https://github.com/Captonomy/assessment/assets/14951564/e6887b15-c19b-417e-9144-33b1d88085ee)

![InvoiceB](https://github.com/Captonomy/assessment/assets/14951564/2d4db56f-c03a-4327-b49a-9d9d56f548b6)


**The deliverable should be a small (200-500 word) essay** that showcases the challenges inherent in this scenario, focusing on strategies to address uptraining complexities, the decision-making process between utilizing existing LLMs or training from scratch (or any other ML based solution), and methods to prevent model hallucinations while maintaining grounded, reliable extractions. Be specific with solutions that (you think) will solve this problem and avoid generalities. Do not include in your reply:
- generalities like "An LLM can do this ...." or essay-like facts and stories
- a set of models that could *possibly* solve the problem; be very specific: pick one or two models and explain why and how you will use and transform/uptraing/fine-tune it to do what is asked. Be specific of your approach.
- you are allowed to say "we will need to research *this* and *that*", but any research you propose should be very specific, as if you could give that to an ML engineer and start researching tomorrow

We're eager to gain insights into your problem-solving strategies and methodology. Your response will be pivotal in assessing your capabilities to address complex ML challenges effectively.

Loking forward to your insights!
