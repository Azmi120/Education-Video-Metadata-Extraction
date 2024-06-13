# Educational-Video-Metadata-Extraction

In this project, we utilizied LangChain to prompt Large Language Models to extract metadata of educational videos collected from youtube and we discuss our insights on how capable LLMs are in extracting such metadata accurately. One of our main motivation to extract educational metadata from the video was to understand how those metadat interact with students' learning and overall engagement to the video content.

We specifically looked at the extraction of three features (1) Complete problem statement or questions demonstrated in the video along with context (2) If the presenter in the video is pausing for viewers reflection often and (3) if there are off topic entertaining elements in the video.

We randomly selected educational youtube videos along with its audio transcript. The curated dataset of the video and audio transcript can be found in LearnLab Summer School Proj Dataset.xlsx

The code to prompt LLM using LangChain can be found in the Jupyter Notebook "LearnLan.ipynb"

To measure how reliable LLM generated metadata from the video were, two researchers manually tagged the "question” “context” and “solutions” properties returned by LLMs as either correct or incorrect. Based on Cohen’s Kappa coefficient, the inter-coder reliability for this coding showed κ = 0.60.

We found that LLMs stuggled from accurately extracting the context of a question posed by the presenter in the video only using its audio transcript. We discuss the errors in LLM generations in our presentation "LearnLab EDM Track Presentation.pdf"
