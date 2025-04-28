Must

start with underscore (_) or letter (a-z A-Z) and followed by any number of underscores ( _ ), letters ( a-z A-Z ), or digits ( 0-9 )

var my_var index1 index_1 _var __var __lt__ are all legal names

cannot be reserved words:

Conventions
<b>_my_var</b> - This is a convention to indicate "internal use" or "private" objects. Objects named this way will not get imported by a statement such as: from module import *
<b>__my_var</b> - Used to "mangle" class attributes – useful in inheritance chains
<b>__my_var__</b> - Used for system-defined names that have a special meaning to the interpreter

1) Packages - short, all-lowercase names. Preferably no underscores - utilities
2) Modules - short, all-lowercase names. Can have underscores. - db_utils dbutils
3) Classes - CapWords (upper camel case) convention. - BankAccount
4) Functions lowercase, words separated by underscores (snake_case) - open_account
5) Variables lowercase, words separated by underscores (snake_case)  - account_id
6) Constants all-uppercase, words separated by underscores - MIN_APR

LINK to PEP8 - https://peps.python.org/pep-0008/