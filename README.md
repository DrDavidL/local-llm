## Run a Local LLM from a Jupyter Notebook in VSCode!
Using : [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)


### Setup Instructions


1. **Install VSCode**: [Download VSCode](https://code.visualstudio.com/).
2. **Install Git**: [Download Git](https://git-scm.com/downloads).
3. **Clone the Repository**:
   - Open VSCode.
   - Open the Command Palette (`Ctrl + Shift + P` or `Cmd + Shift + P`).
   - Type `Git: Clone` and enter:
     ```plaintext
     https://github.com/DrDavidL/local-llm.git
     ```
   - Select a folder to clone to.
   - Open the cloned repository in VSCode.
4. **Set Up the Python Virtual Environment**:
   - Open the integrated terminal in VSCode (`Ctrl + Shift + ~` or `Cmd + Shift + ~`).
   - Navigate to the project directory:
     ```sh
     cd local-llm
     ```
   - Create a virtual environment:
     ```sh
     python -m venv venv
     ```
   - Activate the virtual environment:
     - **Windows**: `.\venv\Scripts\activate`
     - **MacOS/Linux**: `source venv/bin/activate`
   - Install required packages:
     ```sh
     pip install -r requirements.txt
     ```

5. **Open the IPython (Jupyter) notebook**:
    Open the notebook file (`local.ipynb`).

6. **Select the Python Interpreter**:
    Ensure VSCode is using the Python interpreter from your virtual environment. When you try to run a cell you'll be prompted to choose. 
    - Select the interpreter from the `venv` directory (e.g., `./venv/bin/python` for MacOS/Linux or `.\venv\Scripts\python.exe` for Windows).


  > _If questions:_ [cloning a GitHub repository](https://www.google.com/search?q=cloning+a+GitHub+repository) 🛠 [setting up a Python virtual environment](https://www.google.com/search?q=setting+up+a+Python+virtual+environment)  
  > _More info:_ [VSCode Python tutorial](https://www.google.com/search?q=VSCode+Python+tutorial) 💻 [virtual environments best practices](https://www.google.com/search?q=virtual+environments+best+practices)

7. **Download one or two LLMs from HuggingFace**

Options that will run on machines that are even a few years old. After you download, replace the paths used in the notebook cells with the paths to your own downloaded GGUF formatted files.

- https://huggingface.co/bartowski/Phi-3-mini-4k-instruct-GGUF

- https://huggingface.co/bartowski/Meta-Llama-3-8B-Instruct-GGUF

8. **Run the Notebook cells**

- Open your output file, 'output.md', by right clicking and choosing preview. Move to vertical pain to the right of your notebook. This way you can see the output as it emerges!
- Run the cells of your notebook.

Congrats! You're interacting with an AI model running locally on your device!



