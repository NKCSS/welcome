---
title: "db_idx_long_double_upperbound"
excerpt: "Get the secondary index of a record from a secondary long double index table given the secondary index key."
---
Get the upperbound secondary index from a secondary long double index table given the secondary index key Upperbound secondary index is the first secondary index which key is < the given secondary index key

#### Parameters
* `code` - The owner of the secondary index table 

* `scope` - The scope where the secondary index resides 

* `table` - The table where the secondary index resides 

* `secondary` - The pointer to the secondary index key which acts as upperbound pivot point, later on it will be replaced with the upperbound secondary index key 

* `primary` - It will be replaced with the primary key of the record which the upperbound secondary index contains 

#### Precondition
A correponding primary long double index table with the given code, scope table must exist 

#### Post Condition
The secondary param will contains the upperbound secondary index key 

#### Post Condition
The primary param will contains the record that corresponds to the upperbound secondary index 

#### Returns
iterator to the upperbound secondary index