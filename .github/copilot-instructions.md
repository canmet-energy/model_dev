# GitHub Copilot Instructions for HPXML API Project

# Personal Preferences
- Talk to me  in french
- Comment the code like I know nothing and organize code in a clear way.


## Resources
- read /workspaces/model_dev/resources/energyplus/InputOutputReference.pdf so you understand the idf context.


## Coding Standards
 - Develop tests for all code you write.
 - Use consistent naming conventions for variables, functions, and classes. 

### Ruby Code
- Use Ruby 3.0+ features where appropriate
- Follow Ruby style guidelines (e.g., RuboCop)
- Implement proper error handling and logging
- Use type hints for method parameters and return values
- Document methods with YARD comments
- Use the `openstudio` and `openstudio-standards` gem for developing NECB building models in Ruby


### Python Code
- Use Python 3.12+ features where appropriate
- Follow PEP 8 style guidelines
- Implement proper error handling and logging
- Use type hints for function parameters and return values
- Document functions with docstrings
- use the python package openstudio===3.9.0 when developing openstudio models in python
- if developing Energyplus models in python, ask me if I want to use the `eppy` package or the `openstudio` package do generate and manipulate EnergyPlus models in python