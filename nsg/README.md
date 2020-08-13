# azure-templates nsg

This vnet subnet and nsg template is an exmaple of how to you can combine different nsg rules across multiple subnets.

Recently working on a project a vnet needed multiple subnets and each had different inbound and outbound security rules. To avoid duplication of those shared rules this template can take a base set of rules and union them in a variable.  The variable for the unioned nsg object is dynamically referenced.