# CreativeWritingAssistant

```
# Creative Writing Assistant

The Creative Writing Assistant is a Python program that utilizes OpenAI's GPT-3.5 language model to assist with creative writing tasks. It provides functionalities for generating writing prompts, characters, outlines, dialogues, writing advice, and story endings. The program engages in a conversational format with the user, allowing them to interact with the model and obtain the desired content.

## Setup

To run the Creative Writing Assistant, you'll need Python 3 and the following dependencies:

- OpenAI Python (install with `pip install openai`)

Clone the repository and navigate to the project directory.

```bash
git clone [repository_url]
cd creative-writing-assistant
```

## Usage

1. Import the necessary libraries at the beginning of your code.

```python
import openai
import json
```

2. Define the required functions for each feature of the writing assistant. These functions generate prompts, characters, outlines, dialogues, writing advice, and endings. You can modify these functions to fit your specific requirements.

3. Set up the conversation with the GPT model by defining the `run_conversation()` function. This function interacts with the GPT-3.5 model using the `openai.ChatCompletion.create()` method.

4. Handle function calls within the conversation by implementing the `handle_function_call()` function. This function processes specific function calls made by the model's responses and generates the corresponding content.

5. Run the main conversation loop to engage with the model and retrieve the generated output. The loop iterates until a final response is obtained, handling any function calls made by the model and continuing the conversation as necessary.

6. Obtain and process the output by extracting the generated content from the final response message.

```python
output = message['content']
print(output)
```

7. Execute the Python script and observe the generated output based on the user's requests and model-generated function calls.

```bash
python creative_writing_assistant.py
```

## Contributing

Contributions to the Creative Writing Assistant project are welcome! If you find any issues or have ideas for improvements, please feel free to open an issue or submit a pull request.

Before contributing, please review the [Contribution Guidelines](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE).

## Disclaimer

The Creative Writing Assistant utilizes OpenAI's GPT-3.5 language model, and its use is subject to OpenAI's terms and conditions. Be aware of any usage limits and requirements imposed by OpenAI. Ensure compliance with the terms of use and any applicable laws or regulations when using the Creative Writing Assistant.
