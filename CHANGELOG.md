# Changelog - xer-reader

## 0.4.1 - 2024-12-20

Corrections to README.

---

## 0.4.0 - 2024-11-21

* Reference [Issue #2](https://github.com/jjCode01/xer-reader/issues/2)
    * The `to_dict` method no longer throws an error if an unreckognized table is found; it now just ignores the table.
    * Added `FINTMPL` to table_data.
    * Updated `to_csv` method:
        * Can now pass a list of table names to export to CSV. For example pass in agrument `table_names=["TASK", "PROJWBS"]` to only export the task and wbs tables to CSV.  
        * Can now change the delimeter. For example, pass in argument `delimeter=","` to use a coma rather than the default tab.

---  

## 0.3.2 - 2024-10-05  

Clean up code.

---  

## 0.3.1 - 2024-07-02

Patched potential errors when transformming from a string to a float. Some languages use a comma rather than a period in floating point numbers. [Issue #1](https://github.com/jjCode01/xer-reader/issues/1)  

---

## 0.2.0 - 2024-02-02

Added `to_excel` function. Export the tables in the .xer file to individual spreadsheets in a .xlsx file.

---

## 0.1.5 - 2023-11-22

* Added docstrings for attributes.
* Fixed typo in README.

---

## 0.1.4 - 2023-10-12

Access to `Table` class.

---

## 0.1.3 - 2023-10-06

General code clean up.

---

## 0.1.2 - 2023-10-05

### Added

* Added `currency` attribute pulled from ERMHDR values.  
* Added `get_table_names` method.  
* Added `has_table` method.  
* Added `parse_tables` method. Replaces the `tables` attribute.

### Removed  

* Removed `tables` attribute. The tables are now returned in the `parse_tables` method.

---

## 0.1.1 - 2023-09-30

Fixed typo in README example.

---

## 0.1.0 - 2023-09-30

Initial version.

---