
# PB Speak Library

`PB Speak` is a Python library for text-to-speech functionality, designed to provide a simple and customizable way to convert text into spoken words. It uses the `pyttsx3` library for offline text-to-speech synthesis.

## Features
- Customizable speaker name.
- Adjustable speaking rate.
- Supports multiple voices (male, female).
- Easy-to-use interface.

## Installation

### Prerequisite
Ensure `pyttsx3` is installed in your Python environment:
```bash
pip install pyttsx3
```

If the library is packaged, you can install it directly:
```bash
pip install pb_speak
```

## Usage

Here's how to use the library in your Python code:

### Import and Create an Instance
```python
from pb_speak import pbSpeak

# Create an instance of the pbSpeak class
speaker = pbSpeak(name="Priyanshu", rate=180)
```

### Speak Text
```python
# Speak a simple text
speaker.speak("Hello! This is PB Speak in action.")
```

### Parameters
- `name`: The name of the speaker displayed in the console (default: `"PB Speaker"`).
- `rate`: The speech rate in words per minute (default: `170`).
- `voice_index`: The index of the voice to use (default: `1` for female voice, `0` for male voice).

## Complete Example
Here’s a complete example of how to use PB Speak:

```python
from pb_speak import pbSpeak

# Create a speaker instance with custom settings
speaker = pbSpeak(name="Priyanshu", rate=190, voice_index=0)

# Speak some text
speaker.speak("Welcome to the PB Speak library. Enjoy converting text to speech!")
```

## Customization
- **Change Name**: Specify a custom name for the speaker by passing it to the `name` parameter.
- **Adjust Rate**: Modify the `rate` parameter to control the speed of the speech.
- **Select Voice**: Use `voice_index` to choose a voice (e.g., `0` for male, `1` for female).

## File Structure
```
pb_speak/
├── pb_speak.py       # Contains the pbSpeak class
├── LICENSE           # License file
├── README.md         # Documentation
├── setup.py          # Installation script
```

## Development
If you'd like to contribute to the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/FalconX80/pb_speak.git
   ```

2. Navigate to the project directory:
   ```bash
   cd pb_speak
   ```

3. Install the library in editable mode:
   ```bash
   pip install -e .
   ```

4. Test the library:
   ```python
   from pb_speak import pbSpeak

   speaker = pbSpeak(name="Developer")
   speaker.speak("Thank you for contributing to PB Speak!")
   ```

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Author
Developed by **Priyanshu Bhatt**.  
For inquiries, email: [priyanshubhatt80@gmail.com](mailto:priyanshubhatt80@gmail.com).

## Feedback and Contributions
- Found a bug? [Open an issue](https://github.com/FalconX80/pb_speak.git/issues).
- Have a feature request? Feel free to submit it.
- Contributions are welcome! Submit a pull request with your changes.

## Acknowledgments
This project uses the amazing [`pyttsx3`](https://pypi.org/project/pyttsx3/) library for text-to-speech functionality.
