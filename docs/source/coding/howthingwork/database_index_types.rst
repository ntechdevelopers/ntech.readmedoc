Database Index Types
===================================


**CLUSTERED INDEX**

- Physically reorders data rows based on the index key
- One per table
- Significantly speeds up range queries and queries on the indexed column(s)
- Can slow down data modifications (inserts, updates, deletes) due to reordering

**NON-CLUSTERED INDEX**

- Creates a separate structure with pointers to data rows, sorted by the index key
- Multiple allowed per table
- Efficient for equality searches
- Can be used for covering indexes, where all the required columns are included in the index

**UNIQUE INDEX**

- Ensures that all values in a column or a combination of columns are unique
- Can be clustered or non-clustered
- Prevents duplicate values, ensuring data integrity
- Often used on alternate keys (other than the primary key) that must be unique

**FILTERED INDEX**

- Indexes only a subset of rows based on a filter predicate
- Improves performance for queries that frequently filter on the specified condition.
- Reduces index size compared to indexing the entire table

**FULL-TEXT INDEX**

- Enables efficient searching within text data (e.g documents, articles) based on keywords and phrases
- Uses specialized indexing and search algorithms (e.g, inverted indexes)
- Supports linguistic features like stemming and thesaurus

**COMPOSITE INDEX**

- An index created on multiple columns
- Can be clustered or non-clustered
- Optimizes queries that filter or sort on multiple columns
- The order of columns in the index definition is crucial for performance

**COVERING INDEX**

- Includes all columns needed for a query in the index itself, avoiding the need to access the base table
- Can be non-clustered
- Significantly speeds up queries that only need data from the indexed columns

**INDEX WITH INCLUDED COLUMNS**

- Similar to a covering index, but only includes non-key columns
- Non-clustered
- Can improve query performance if the additional columns are frequently used

**SPATIAL INDEX**

- Efficiently index and query spatial data (geometric shapes, geographic locations)
- Implementation: R-tree, Quadtree, Grid
- Optimizes spatial queries
- Handles dynamic updates to spatial objects
- Scales to large datasets

**BITMAP INDEX**

- Efficiently indexes columns with a low cardinality (few unique values).
- Stores bitmaps indicating which rows contain a particular value
- Compact and fast for certain types of queries