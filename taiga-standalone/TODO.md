# Activity tracking for TaIGa
This is a to-do list of the pending ativities for the standalone version of TaIGa. Activities are separeted into categories.

## Refactor
- [x] Add comparators to the `Taxon` class
- [ ] Fix type hints - probably keep the `typing` based annotations to enable backwards compatibility with Python >= 3.5

## Testing
- [x] Finish testing text parsing for organism names
- [x] Test text parsing for Taxon IDs
- [ ] Test parsing Genbank files
	- [ ] Single organism, single record
	- [ ] Single organism, multiple records
	- [ ] Multiple organisms

## Dev
- [ ] Drop `pandas` and use the built-in `csv` module to handle outputs instead
- [ ] Find a way of fetching all possible taxa classification from Taxonomy instead of providing a manual list - this may be an issue with ordering columns in the output
- [ ] Look into implementing `abc` for the `Taxon` class (a big maybe tho)
- [ ] Write getter and setter methods for the `Taxon` class. Maybe look into implementing [this syntax](https://docs.python.org/3/library/functions.html?highlight=property#property)