# langchain-falcon-main
Simple Chat UI using Falcon model, LangChain and Chainlit

### Open Source in Action 🚀
- [Falcon](https://falconllm.tii.ae/) as Large Language model
- [LangChain](https://python.langchain.com/en/latest/modules/models/llms/integrations/huggingface_hub.html) as a Framework for LLM
- [Falcon model](https://huggingface.co/tiiuae/falcon-7b-instruct) from Huggingface Website
- [Chainlit](https://docs.chainlit.io/langchain) for deploying.


## STEPS TO REPLICATE 

1. Fork or create this repository in GitHub
   ```
   git clone https://github.com/oldbright22/falcon-main.git
   ```

2. From your GitHub, select new repository created, inside click GREEN button <> Code and 
select CODESPACES tab, and click on create codespace from your (main or master branch).


3. Add huggingfacehub api token to .env as follows:  ALSO might be prompted so keep it around. 
Get Huggingfacehub api token from this [URL](https://huggingface.co/settings/tokens). 
You need to create an account in Huggingface if you haven't already.
   ```
   HUGGINGFACEHUB_API_TOKEN=your_huggingface_token
   ```
Expected result = your own API

4. Install Python Extension:
From LEFT menu where all the BIG icons -- drill down into the Extensions icon
Search/Install Python extension

Expected result:  Python extension installed

5. Create/Install Kernel server:
From LEFT menu where all the BIG icons -- drill down into Explorer icon 
Then click on the 1st Jupyter notebook "langchain_falcon_V1.." this will bring the jupyter notebook active 
Look at the TOP RIGHT section and you will see a drop down for SELECT KERNEL.
Click on it and --- and you will 1st time, see install JUPYTER and this will install additonal extensions

Expected result: ALL required jupyter extensions installed  +  ensure that you can now select this environment in kernel drop down.

## SYSTEM REQUIREMENTS

6. Having above JUPYTER notebook open, go the mid of the page -- and look for TERMINAL section
Run below commands in the terminal 

You must have Python 3.10 or later installed. 

Create a virtualenv and activate it
   ```
   python3 -m venv .venv && source .venv/bin/activate
   ```

Install some required libraries.
   ```  
   pip install -r requirements.txt
   ```

## NOT REQUIRED JUST YET
#7. Run the following command in your terminal to start the chat UI:
   ```
   chainlit run langchain_falcon.py --no-cache -w
   ```