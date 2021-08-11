# .env Loader For Python
## Quick Start
Windows:
```bash
pip install python-dotenv
```
Linux/MacOS:
```bash
pip3 install python-dotenv
```
---
Create a .env **file** that will store your variables. The variables need to be stored in a specific format.
```
NAME=type:value
```
Example .env file:
```
API_KEY=str:https://my.api.key/api/fgh4u3iqhvn_t89rpwemh_89grmqh4n89b/
IMPORTANT_NUBER=int:6174
IMPORTANT_FLOATS=set:float:3.1415926,float:2.71828
FILE=file:path/to/file.txt
```
**NOTE:** The values inside of the IMPORTANT_FLOATS ```set``` are also typed.

Inside the python script:
```py
from config import Config

api_key = Config.API_KEY
```

