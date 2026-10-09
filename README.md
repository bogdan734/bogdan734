<img src="assets/banner.svg" width="100%" alt="Bohdan Havryliuk, founder, CEO and chief engineer at Kalorad. Our own language model, trained from scratch, now training on MareNostrum 5 with EuroHPC compute.">

<p>
<a href="https://kalorad.app"><img alt="kalorad.app" src="https://img.shields.io/badge/-kalorad.app-14112A?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNjAgMTYwIj48cGF0aCBkPSJNIDEwIDgwIEEgNzAgNzAgMCAwIDEgMTUwIDgwIiBmaWxsPSJub25lIiBzdHJva2U9IiNBNzhCRkEiIHN0cm9rZS13aWR0aD0iMTIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIvPjxwYXRoIGQ9Ik0gMTUwIDgwIEEgNzAgNzAgMCAwIDEgMTAgODAiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzIyRDNFRSIgc3Ryb2tlLXdpZHRoPSIxMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIi8%2BPHJlY3QgeD0iNTUiIHk9IjQ0IiB3aWR0aD0iMTgiIGhlaWdodD0iNzIiIHJ4PSI5IiBmaWxsPSIjRjVFRkU2Ii8%2BPHBhdGggZD0iTSA2NiA4MCBMIDExMCA0NCBNIDY2IDgwIEwgMTEwIDExNiIgc3Ryb2tlPSIjRjVFRkU2IiBzdHJva2Utd2lkdGg9IjE4IiBzdHJva2UtbGluZWNhcD0icm91bmQiLz48L3N2Zz4%3D&logoColor=E0B75A"></a>
<a href="https://www.linkedin.com/in/bohdan-havryliuk-370762386"><img alt="LinkedIn" src="https://img.shields.io/badge/-LinkedIn-14112A?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0UwQjc1QSIgZD0iTTQuOTggMy41YTIuNSAyLjUgMCAxIDEgMCA1IDIuNSAyLjUgMCAwIDEgMC01ek0zIDloNHYxMkgzek05IDloMy44djEuN2guMDVjLjUzLTEgMS44NC0yLjA1IDMuNzgtMi4wNUMyMC42IDguNjUgMjEgMTEuMiAyMSAxNC41VjIxaC00di01LjhjMC0xLjQtLjAzLTMuMi0xLjk1LTMuMi0xLjk1IDAtMi4yNSAxLjUtMi4yNSAzLjFWMjFIOXoiLz48L3N2Zz4%3D&logoColor=E0B75A"></a>
<a href="mailto:bohdan@kalorad.app"><img alt="bohdan@kalorad.app" src="https://img.shields.io/badge/-bohdan%40kalorad.app-14112A?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0UwQjc1QSIgZD0iTTMgNWgxOGExIDEgMCAwIDEgMSAxdjEyYTEgMSAwIDAgMS0xIDFIM2ExIDEgMCAwIDEtMS0xVjZhMSAxIDAgMCAxIDEtMXptMSAyLjNWMTdoMTZWNy4zbC04IDUuNC04LTUuNHpNNS42IDdsNi40IDQuM0wxOC40IDdINS42eiIvPjwvc3ZnPg%3D%3D&logoColor=E0B75A"></a>
</p>

I'm the founder, CEO and chief engineer of **[Kalorad](https://kalorad.app)**. We train our own language model from zero and build the assistant that runs on it inside a customer's own network. No calls to anyone else's AI, weights the customer can own outright, and a tokenizer made for Ukrainian.

It's for the people who can't send their documents to a foreign vendor: banks, hospitals, ministries, law firms.

<img src="assets/stats-dark.svg" width="100%" alt="10,000 H100 GPU-hours on MareNostrum 5 from EuroHPC. 1.3B active parameters, mixture of experts, training now. 6 to 41 percent fewer tokens per Ukrainian sentence than GPT-4o, Llama-3.1, Gemma-3, Mistral and Qwen3. First run: 683M parameters for $86.">

## How it's made

<img src="assets/pipeline-dark.svg" width="100%" alt="Corpus, tokenizer, pretraining on MareNostrum 5, fine-tuning, release, your network.">

**The model.** Our first full pretraining run finished in September: 683M parameters, 13.1B tokens, one GPU, $86 of compute. The production model is a mixture of experts with multi-token prediction and 1.3B active parameters. It has a fast mode and one that thinks longer. It's training now on MareNostrum 5 at the Barcelona Supercomputing Center, on 10,000 H100 hours from the EuroHPC AI Factory call. I wrote the training stack (Slurm jobs, DDP and FSDP, the Muon optimizer, torch.compile) and found the bug that had been making training 39% slower.

**The product.** Chat and an agent that works with Google Workspace, Microsoft 365, KeyCRM, Bitrix24 and email. MCP in both directions. Add-ins for Word, Excel, PowerPoint and Outlook, an add-on for Google Workspace, desktop apps for Windows and macOS, and an OpenAI-compatible API, so anything already built for that API plugs in unchanged.

**The team.** Three engineers: me, plus two who joined in October 2026. The code is closed. Results go to [LinkedIn](https://www.linkedin.com/in/bohdan-havryliuk-370762386) as they come, including the runs that go wrong.

## Open work

Most client work is under NDA. These are the public pieces.

<p>
<a href="https://github.com/bogdan734/eva-ai-recruiter"><img src="assets/cards/eva-ai-recruiter-dark.svg" width="49%" alt="eva-ai-recruiter"></a>
<a href="https://github.com/bogdan734/cv-video-analytics"><img src="assets/cards/cv-video-analytics-dark.svg" width="49%" alt="cv-video-analytics"></a>
</p>
<p>
<a href="https://github.com/bogdan734/twin"><img src="assets/cards/twin-dark.svg" width="49%" alt="twin"></a>
<a href="https://github.com/bogdan734/conference-booking-api"><img src="assets/cards/conference-booking-api-dark.svg" width="49%" alt="conference-booking-api"></a>
</p>
<p>
<a href="https://github.com/bogdan734/dzencode-comments"><img src="assets/cards/dzencode-comments-dark.svg" width="49%" alt="dzencode-comments"></a>
<a href="https://github.com/bogdan734/Nexus"><img src="assets/cards/nexus-dark.svg" width="49%" alt="Nexus"></a>
</p>
<p>
<a href="https://github.com/bogdan734/checkers-api"><img src="assets/cards/checkers-api-dark.svg" width="49%" alt="checkers-api"></a>
<a href="https://github.com/bogdan734/brain-parsers"><img src="assets/cards/brain-parsers-dark.svg" width="49%" alt="brain-parsers"></a>
</p>

## Toolbox

<p>
<img alt="C#" src="https://img.shields.io/badge/-C%23-14112A?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0UwQjc1QSIgZD0iTTEyIDEuNSAyMS4xIDYuNzV2MTAuNUwxMiAyMi41bC05LjEtNS4yNVY2Ljc1ek0xMiA2LjJhNS44IDUuOCAwIDEgMCA1LjAyIDguN2wtMi4yLTEuMjdBMy4yNyAzLjI3IDAgMSAxIDE0LjgyIDEwLjRsMi4yLTEuMjdBNS44IDUuOCAwIDAgMCAxMiA2LjJ6bTUuMyAzLjloLS44di44aC0uOHYtLjhoLS44di44aC0uNnYuOGguNnYuOGgtLjZ2LjhoLjZ2LjhoLjh2LS44aC44di44aC44di0uOGguNnYtLjhoLS42di0uOGguNnYtLjhoLS42em0tMS42IDEuNmguOHYuOGgtLjh6Ii8%2BPC9zdmc%2B&logoColor=E0B75A"> <img alt=".NET" src="https://img.shields.io/badge/-.NET-14112A?style=for-the-badge&logo=dotnet&logoColor=E0B75A"> <img alt="Python" src="https://img.shields.io/badge/-Python-14112A?style=for-the-badge&logo=python&logoColor=E0B75A"> <img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch-14112A?style=for-the-badge&logo=pytorch&logoColor=E0B75A"> <img alt="CUDA" src="https://img.shields.io/badge/-CUDA-14112A?style=for-the-badge&logo=nvidia&logoColor=E0B75A"> <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-14112A?style=for-the-badge&logo=typescript&logoColor=E0B75A"> <img alt="React" src="https://img.shields.io/badge/-React-14112A?style=for-the-badge&logo=react&logoColor=E0B75A"> <img alt="Tauri" src="https://img.shields.io/badge/-Tauri-14112A?style=for-the-badge&logo=tauri&logoColor=E0B75A"> <img alt="FastAPI" src="https://img.shields.io/badge/-FastAPI-14112A?style=for-the-badge&logo=fastapi&logoColor=E0B75A"> <img alt="Django" src="https://img.shields.io/badge/-Django-14112A?style=for-the-badge&logo=django&logoColor=E0B75A"> <img alt="PostgreSQL" src="https://img.shields.io/badge/-PostgreSQL-14112A?style=for-the-badge&logo=postgresql&logoColor=E0B75A"> <img alt="SQLite" src="https://img.shields.io/badge/-SQLite-14112A?style=for-the-badge&logo=sqlite&logoColor=E0B75A"> <img alt="Redis" src="https://img.shields.io/badge/-Redis-14112A?style=for-the-badge&logo=redis&logoColor=E0B75A"> <img alt="Docker" src="https://img.shields.io/badge/-Docker-14112A?style=for-the-badge&logo=docker&logoColor=E0B75A"> <img alt="Google Cloud" src="https://img.shields.io/badge/-Google%20Cloud-14112A?style=for-the-badge&logo=googlecloud&logoColor=E0B75A"> <img alt="Linux" src="https://img.shields.io/badge/-Linux-14112A?style=for-the-badge&logo=linux&logoColor=E0B75A"> <img alt="Stripe" src="https://img.shields.io/badge/-Stripe-14112A?style=for-the-badge&logo=stripe&logoColor=E0B75A">
</p>

## Before Kalorad

Five years of full-stack work for private clients in C#/.NET, Python and TypeScript, two of them leading a team. In 2025 and 2026 I worked on the other side of model training: AI Trainer at Meta, then AI Training Contractor at Scale AI, reviewing and rating model output, mostly code. BSc (Hons) Artificial Intelligence, De Montfort University, First Class.

<p align="center"><a href="mailto:bohdan@kalorad.app">bohdan@kalorad.app</a> · <a href="https://kalorad.app">kalorad.app</a> · <a href="https://www.linkedin.com/in/bohdan-havryliuk-370762386">LinkedIn</a></p>
