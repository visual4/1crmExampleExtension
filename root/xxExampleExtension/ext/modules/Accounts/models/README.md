# The file bean.Account.php
the core file /modules/Accounts/models/bean.Account.php contains the main database schema and field configuration for the Accounts module as well as information about some of the relations to other modules.

Everything in this file is written in a sructured configuration language (it looks like YAML, but there are some differences!) 1CRM creates a configuration array from this file.

our file, the ext/modules/Accounts/models/bean.Account.php will change and extend the core file, this is done by merging the core configuration array and the values from our file. This way we can change values or add new values.

In this case the default values for four fields are changed:

- billing_address_country
- billing_address_countrycode
- shipping_address_country
- shipping_address_countrycode

these fields already exist (please take a look at the core bean.Account.php). All other settings for these fields  stay the same, and as the default value, doesn't exist in core, it is just added.