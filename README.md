# Resume-parser
Explanation of Key Features

Extraction Accuracy (95%):
The code calculates the accuracy of entity extraction by comparing the results against a predefined ground truth (calculate_entity_accuracy). You can expand this by adding more detailed ground truth data.

Processing Speed (1,000 Resumes per Hour):
By using Python’s multiprocessing module (parallel_resume_processing), resumes are processed in parallel, significantly boosting throughput.
The measure_processing_speed function measures the time taken and calculates resumes processed per hour.

Tokenization, Lemmatization, POS Tagging, and Stopwords Elimination:
These tasks are handled inside the process_resume function using SpaCy.

Named Entity Recognition (NER) with 85% Accuracy:
The code leverages SpaCy’s NER capabilities and compares extracted entities with the ground truth. Precision can be further improved by fine-tuning SpaCy models if needed.


Visualization of Named Entities:
The visualize_entities function uses SpaCy’s displacy tool to visualize named entities within resumes.

Performance Considerations:
The speed is optimized using multiprocessing, which should help you reach or exceed 1,000 resumes per hour, depending on system resources.
Accuracy measurement provides immediate feedback on how well the extraction matches the expected results.
