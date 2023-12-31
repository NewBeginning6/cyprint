

# CyPrint

CyPrint is a Python package for customized colorful logging.

## Installation

You can install CyPrint using pip:

```bash
pip install cyprint
```

## Usage

```python
from cyprint import cyprint, cypb

cyprint('info信息', "INFO")
cyprint('警告信息', "WARNING")
cyprint('成功信息', "SUCCESS")
cyprint('错误信息', "ERROR")
cyprint('debug信息', "DEBUG")

# Create a progress bar
total_events = 100  # Replace with your total number of events
for i in range(total_events):
    cypb(i, total_events, cyname="Progress")
    # Your processing code here...
```

### Customizing Log Messages

You can also create custom log messages by specifying the log level:

```python
cyprint('Custom message', 'debug')
```

### Progress Bar

The `cypb` function generates a progress bar:

```python
from cyprint import cypb

total_events = 100  # Replace with your total number of events
for i in range(total_events):
    cypb(i, total_events, cyname="Progress")
    # Your processing code here...
```

## Contributing

We welcome contributions! If you'd like to contribute to CyPrint, please fork the repository and submit a pull request.
