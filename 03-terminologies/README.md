# Terminologies

## Value related
1. **Data** - values stored in the database.
2. **Information** - the meaning of data that is useful to you. What you retrieve.
3. **Null** - MISSING values.

## Structure related
1. **Table** (relation) - composed of tuples (records) and attributes (fields). Represents either an `object` or `event`.
   - **Data Table** - used to supply information
   - **Validation table** (lookup table) - enforces data integrity
   - **Relationship table** (lookup table) - established a relationship between two tables.
2. **Field** (attribute) - characteristic of a table subject.
   - badly designed fields: `multipart field`, `multi-valued field`, `calculated field`
3. **Record** (tuple) - unique instance of a table subject. Identified by a `unique key`
4. **View** - Virtual tables. Draws data from `base tables`. Generally not stored, but rather retrieved.
5. **Keys**
   - **Primary Key** - Identifies a `specific record` with a database. Enforces `Table-level` integrity.
   - **Foreign Key** - Primary key of another table that has a relationship with a second table.
6. **Index** - a structure that improves RDBMS data processing.

## Relationship related
1. **Relationships** - when one table can be associate to another table.
   - **One-to-One** - set a foreign key to the 2nd table.
   - **One-to-Many** - set a foreign key to the 2nd table
   - **Many-to-Many** - use a `relationship table`
2. **Degree of participation** - minimum number of records that a given table must have with a single record of an associated table.

## Integrity related
1. **Field specification** - all elements of a field.
   - **General** - fundamental information (field name, description, parent table).
   - **Physical** - how a field is represented (data type, length, character support).
   - **Logical** - describes the value stored (required value, range of values, null support)
2. **Data integrity** - validity, consistency, and accuracy of the data.
   - **Table level** - no duplicate records, and identifier field is unique and not null.
   - **Field level** - sound field structure; valid, consistent, and accurate; field of the same type is consistent throughout the DB.
   - **Relationship-level** - sound relationship and synchronized.
   - **Business rules** - restrictions or limitation imposed by an organization on how it uses data. Affects how a field would be represented, how db is designed, type/degree of participation, synchronization.