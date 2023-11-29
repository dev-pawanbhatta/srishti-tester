# Srishti Tester - Python Module for Srishti API Generator

## Overview

Srishti Tester is a Python module designed to work seamlessly with the Srishti API Generator. This module simplifies the process of testing and interacting with APIs generated by Srishti, allowing users to perform various HTTP requests without writing a single line of code.

## Features

- **Effortless API Testing:** Test APIs generated by Srishti without the need for manual coding.
- **Supports Multiple HTTP Methods:** Perform GET, POST, PUT, and DELETE requests effortlessly.
- **Flexible Configuration:** Easily configure API endpoints, headers, and request payloads.

## Installation

```bash
git clone https://github.com/dev-pawanbhatta/srishti-tester.git
```

```bash
cd srishti-tester
```

```bash
pip install requests
```

```bash
cp script.py
```
### Copy the below code in script.py

```bash
from srishti_tester.tester import Tester

a = Tester(token="",base_url='http://localhost', port=8000)

files = {'image': open('example.jpg','rb')}

response = a.put(table="test_table", id=4, files=files, data={ 'name':'John', 'email':'test@test.com','password':'12345678' })

print(response)
```

```bash
python script.py
```

## Configuration

token: Your Srishti API token for authentication.
base_url: The base URL of your Srishti API.
port: (Optional) Specify the port for the HTTP connection (default is 443).

## Documentation

For more details on the Srishti API Generator and its capabilities, refer to the official documentation.

## Contributing

Contributions are welcome! If you have ideas for improvements or encounter any issues, please open an issue or submit a pull request.




