from pathlib import Path

content = """# Interviewer Questions List

## Profile & Verification
1. Can you share your LinkedIn profile link?
2. How much total experience should I mention for you?
3. Are you a Data Engineer or Software Engineer, or both?

## Experience Details
4. How many years of experience do you have in the software industry?
5. Do you have experience with healthcare data integration?
6. How many years of experience do you have specifically in healthcare data?
7. Are you currently working with a healthcare client?
8. Have you worked with healthcare clients before this role?

## Technical Skills
9. How many years of experience do you have with Databricks?
10. How many years of experience do you have with Python?
11. What is your experience level with SQL?
12. What is your experience with PySpark?
13. How many years of experience do you have with Azure Cloud?
14. Have you worked on ETL processes?
15. How many years of ETL experience do you have?

## Education & Certifications
16. Do you have any certifications?
17. When did you complete your master’s degree?
18. From which university did you complete your master’s?
19. When did you complete your bachelor’s degree?
20. From which stream or specialization did you complete your bachelor’s?

## Interview Availability
21. Are you available for interviews this week or next week?
22. Are you available on Friday?
23. What time are you generally available on Friday?
24. Are you available on Monday?
25. What time slots are you available on Monday (EST)?
"""

path = Path("/mnt/data/Interviewer_Questions_List.md")
path.write_text(content, encoding="utf-8")

path
