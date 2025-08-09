📝 Project Documentation: AI-Powered Student Essay Grader


---

✅ Overview

The AI-Powered Student Essay Grader is an automated text-processing pipeline built using LangGraph, LangChain, and Gemini LLMs. It is designed to evaluate student essays for grammar, argument strength, coherence, clarity, and potential plagiarism. The system processes a given essay, generates a final grade, provides rich feedback, and exports the results in CSV format. It also utilizes memory to keep track of interactions and enhance prompt context.




🎯 Motivation

Manual essay grading is time-consuming, subjective, and inconsistent across evaluators. With the rise of AI and LLMs, it becomes feasible to build scalable and consistent grading systems to:

1.  Help teachers automate repetitive assessment tasks.

2. Provide students with instant and actionable feedback.

3. Improve objectivity in grading.

4. Maintain records for analysis and reporting.


This project bridges the gap between AI capabilities and educational assessments, offering an end-to-end solution that mimics human grading behavior using structured graph workflows.




🧩 Key Components

1. LangGraph: Manages node-based text processing with memory-aware state updates.


2. LangChain: Provides the LLM interface (Gemini) with custom prompt handling.


3. Graph Nodes:

load_essay_node: Loads user input.

check_plagiarism_node: Checks for plagiarism using LLM.

evaluate_grammar_node: Scores grammar.

evaluate_arguments_node: Assesses argument strength.

grade_assignment_node: Assigns a final grade.

generate_feedback_node: Generates feedback.

csv_export_node: Saves all evaluation results to a CSV file.



4. Memory: LangGraph memory integration ensures context and continuity.


5. Prompt Customization: Each node includes a dedicated prompt with professional tone and clarity.


6. Temperature Control: Each LLM call includes adjustable temperature for creativity control.






🧪 Method

The method follows a graph-based pipeline where nodes operate in a sequential and stateful manner.

Workflow:

1. Essay Submission: The essay text is loaded.


2. Plagiarism Check: Evaluates if content is original using a carefully crafted prompt.


3. Grammar Evaluation: LLM scores grammar usage.


4. Argument Evaluation: LLM scores the logical coherence of arguments.


5. Final Grading: Uses all prior inputs to generate a 100-point scale grade.


6. Feedback Generation: Custom feedback is created based on prior analysis.


7. Export: All scores and feedback are written to a CSV file.


8. Memory: Maintains user-specific essay history and interactions.



Each LLM node is prompted using a detailed and role-specific instruction, e.g., a grammar expert, university professor, or academic writing assistant.




💡 Benefits

1. Automated Evaluation: Reduces grading time significantly.

2. Scalable: Can grade thousands of essays in batch with consistent quality.

3. Insightful Feedback: Empowers students to learn from personalized insights.

4. Memory-Aware: Tracks essay versions, useful for iterative submissions.

5. Export-Ready: Easy CSV exports for academic record keeping and analysis.

6. Customizable Prompts: You can easily adapt prompts to match any grading standard or domain.





✅ Conclusion

This project demonstrates how cutting-edge AI tools like LangGraph and LLMs can revolutionize educational assessment. The AI-Powered Essay Grader is not only an effective tool for teachers but also a powerful learning companion for students. With modular nodes, flexible memory, and professional prompt design, it delivers a seamless and scalable grading experience
