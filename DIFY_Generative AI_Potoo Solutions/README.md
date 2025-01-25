# Summary

This project, in collaboration with Potoo Solutions, aimed to enhance business intelligence by transitioning from static Tableau dashboards to dynamic, conversational interfaces powered by Large Language Models (LLMs). These interfaces enabled users to query structured data in natural language and receive accurate, real-time responses, including visual insights, simplifying data exploration and decision-making processes. 

## Methodology using DIFY

To achieve these goals, two distinct workflows were developed and evaluated. The Agentic Workflow used real-time API connections to access and process Potoo Solutions' experimental data for the Wüsthof brand, dynamically retrieving data and leveraging an LLM to generate insights. The Simple Workflow focused on structured Excel data, enabling visual data generation and analysis through LLM processing and Python-executed visualizations.

## Evaludation metrics

The workflows were evaluated based on Accuracy Score, Faithfulness, and Answer Relevancy, with accuracy further assessed on data extraction, code functionality, and visualization accuracy. Results showed the Agentic Workflow excelled at handling real-time data, while the Simple Workflow proved effective for visual outputs.

## Conclusion

The project faced some challenges, such as LLMs struggling with large datasets due to token limits and occasional inconsistencies in responses. Additionally, the Dify platform, though easy to use, lacked certain Python tools, which slowed down some processes. These challenges were managed through careful planning and adjustments.

Future enhancements could focus on handling larger datasets, integrating advanced visualization capabilities, and incorporating real-time customer query documentation. This project demonstrates the potential of AI-driven solutions to improve data access, provide actionable insights, and support smarter decision-making for Potoo Solutions’ customers.

