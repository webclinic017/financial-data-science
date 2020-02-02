# Investment Data Science

## dives module

\'di&0305;(,)vez \
̅
### dbengines.py

- wrappers and convenient methods for database engines: pymongo, sqlalchemy, redis"""

### structured.py

- classes and methods for manipulating structured data, underlying stored in sql
- subclasses for CRSP, Compustat, IBES, and other derived data sets

### unstructured.py

- class and methods for unstructured datasets, underlying stored in mongodb
- loaders for FOMC minutes, Loughran-McDonald word lists, and other

### evaluate.py

- classes and methods for backtesting and evaluating portfolio returns

### taq.py

- class and methods for loading and manipulating Daily TAQ tick data
- methods for direct access (by symbol) of raw .gz daily files, cleaning, liquidity measures

### econs.py

- classes and methods for manipulating economic data sources
- industry sectoring, sic-naics-bea codes, from BEA, naics.com crosswalk, Fama-French groups
- loaders for BEA and FRED

### custom.py

- common function call arguments and useful wrappers
- e.g. dives.customn.kerasClassifier extends keras.wrappers.scikit_learn.KerasClassifier
  - parameterize network structure, 
  - endogenize input and output dimensions from data,
  - auto transform and inverse_transform class labels

### util.py

- small collection of useful functions and classes
- e.g. NamedDict extends dict: multiple, named key fields
- e.g. DataFrame extends pandas.DataFrame: new methods hqueue, lags, to_numeric