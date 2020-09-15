# CRUD Factory

CRUD Factory is basically for creating services. The service can then be used for creating, retrieving, updating, deleting and querying data.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install crud_factory.

```bash
pip install crud_factory
```

## Usage

```python
import db # from models 

from crud_factory import CRUDFactory

class BaseService(CRUDFactory):
    db = db

class UserService(BaseService):
    """ Activities of a User """
    model_class = User
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first or contact the developer to discuss what you would like to change.


## Dependencies
Python>=3.7
SQLAlchemy
phonenumbers
Unidecode
