# k-diagrams


## Install https://graphviz.org/download/ and add to PATH

```graphviz-11.0.0 ```

## using pip (pip3)

```pip install diagrams```

## Quick Start

```
# diagram.py
from diagrams import Diagram
from diagrams.aws.compute import EC2
from diagrams.aws.database import RDS
from diagrams.aws.network import ELB

with Diagram("Web Service", show=False):
    ELB("lb") >> EC2("web") >> RDS("userdb")
```

## This code generates below diagram.

```python example.py```


![web_service.png](web_service.png)