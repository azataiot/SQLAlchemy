# SQLAlchemy



## Overview

![sqla_arch_small](./README.assets/sqla_arch_small.png)

```mermaid
graph TB
A(SQLAlchemy) -->B(ORM)
A -->C(Core)

C -->C1("Scheme / Types")
C -->C2("SQL Expression Language")
C -->C3("Engine")

C3 -->C3a("Connection Pooling")
C3 -->C3b("Dialect")

C3a --> D(DBAPI)
C3b --> D(DBAPI)
```

**ORM vs CORE**

- Core/SQL Expression language is command oriented
- ORM is state oriented

### Installation 

```bash
# cython -- for speed
pip install cython

# default
pip install sqlalchemy

# with asyncio support
pip install "sqlalchemy[asyncio]"

```

