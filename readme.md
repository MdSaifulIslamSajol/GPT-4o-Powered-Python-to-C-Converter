# Python to C++ Code Generator with LLMs

This project provides an interactive tool to convert Python code into high-performance C++ code using state-of-the-art large language models (LLMs) such as OpenAI GPT-4o and Anthropic Claude. You can also run and compare the outputs of both the original Python and the generated C++ code.

## Features

- **Automatic Code Conversion:**  
  Converts Python code to optimized C++ using LLMs.
- **Model Choice:**  
  Choose between OpenAI GPT or Anthropic Claude for code generation.
- **Streaming Output:**  
  See the generated C++ code in real time as it is produced by the model.
- **Code Execution:**  
  Run both Python and C++ code and view their outputs for benchmarking.
- **Web UI:**  
  User-friendly interface built with Gradio for easy interaction.

## How It Works

1. **Paste or write Python code** in the provided textbox.
2. **Select the LLM model** (GPT or Claude) for code generation.
3. **Click "Convert code"** to generate C++ code.
4. **Run Python or C++ code** and compare their outputs and performance.

## Requirements

- Python 3.8+
- [OpenAI Python SDK](https://github.com/openai/openai-python)
- [Anthropic Python SDK](https://github.com/anthropics/anthropic-sdk-python)
- [Gradio](https://gradio.app/)
- [dotenv](https://pypi.org/project/python-dotenv/)
- `clang++` (for compiling C++ code, optimized for Apple M1 by default)
- API keys for OpenAI and Anthropic (set as environment variables)

## Setup

1. **Clone this repository** and navigate to the project folder.
2. **Install dependencies:**
    ```bash
    pip install openai anthropic gradio python-dotenv
    ```
3. **Set your API keys** in a `.env` file:
    ```
    OPENAI_API_KEY=your-openai-key
    ANTHROPIC_API_KEY=your-anthropic-key
    ```
4. **Run the notebook** or script.

## Usage

- Launch the notebook and follow the instructions in the Gradio UI.
- You can switch between models for code generation.
- The C++ code is compiled and executed on your machine (ensure you have a compatible compiler).

## Notes

- The default C++ compilation command is optimized for Apple M1.  
  If you are on a different platform, modify the `execute_cpp` function accordingly.
- For ultra-low cost, you can switch to smaller models by uncommenting the relevant lines in the code.

## Example

![screenshot](screenshot.png)

## License

MIT License

---

**Created for educational purposes: learn how LLMs can automate code translation and optimization!**