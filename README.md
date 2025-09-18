# Promo Code Generator

Generate **unique 12-character promo codes** with configurable rules and export them to **CSV** and **Excel**.

## Features
- Enforce minimum counts for letters/digits
- Require specific letters (e.g., must include `A`, `E`, `U`, `X`)
- Optional prefix/suffix
- Exclude ambiguous characters (`0`, `O`, `1`, `I`, `S`, `5`)
- Block codes matching forbidden regex patterns
- Guaranteed uniqueness (in-memory or SQLite backend)
- Cryptographically secure randomness

## Requirements
- Python 3.9+
- Dependencies:  
  ```bash
  pip install pandas openpyxl

## Usage
1. Open the notebook or script.
2. Edit the Configuration section to set your rules.
3. Run the code to generate codes.
4. Outputs will be saved as:
    - promo_codes.csv
    - promo_codes.xlsx

## Example Configuration
```python
MIN_LETTERS = 4
MIN_DIGITS = 4
REQUIRE_ONE_OF = set("AEUX")
PREFIX = "ACME"
SUFFIX = "25"
```

This generates codes like:

```bash
ACME9K7X2T25
ACMEQ48E6A25
```
