# fava

Web interface for the double-entry bookkeeping software
[beancount](http://furius.ca/beancount/) with a focus on features and usability.

You can try out a demo here: [fava.pythonanywhere.com](http://fava.pythonanywhere.com)

[![fava](https://raw.githubusercontent.com/aumayr/fava/master/util/screenshots/screenshot-01.png)](#screenshot)
(More Screenshots here: [github.com/aumayr/fava/tree/master/util/screenshots](https://github.com/aumayr/fava/tree/master/util/screenshots))

Built on [Flask](http://flask.pocoo.org/), it relies on an artificial API
(`api.py`) that calls into `beancount` and displays the results.

## Installation

1. Prerequisites: An installed version of
   [beancount](http://furius.ca/beancount/) and Python >= 3.5
2. Download [`fava`](https://github.com/aumayr/fava/archive/master.zip) to your computer and unzip it
3. Install it by running `python setup.py install`

## Usage

1. Start `fava` by running `fava
   /Volumes/Ledger/example.ledger` (substitute with the path to your own
   beancount-file) to run the included web server.
2. Point your browser at `http://localhost:5000` to view the web interface.

## Notable features

*(many missing here)*

### Keyboard Shortcuts

`fava` comes with Gmail-style keyboard shortcuts:

<kbd>?</kbd>: Show keyboard shortcuts overview  

**Jumping to pages:**  
<kbd>g</kbd> then <kbd>i</kbd>: Go to Income Statement  
<kbd>g</kbd> then <kbd>b</kbd>: Go to Balance Sheet  
<kbd>g</kbd> then <kbd>t</kbd>: Go to Trial Balance  
<kbd>g</kbd> then <kbd>g</kbd>: Go to General Journal    
<kbd>g</kbd> then <kbd>q</kbd>: Go to Custom Query  

<kbd>g</kbd> then <kbd>h</kbd>: Go to Holdings  
<kbd>g</kbd> then <kbd>w</kbd>: Go to Net Worth  
<kbd>g</kbd> then <kbd>d</kbd>: Go to Documents  
<kbd>g</kbd> then <kbd>n</kbd>: Go to Notes  
<kbd>g</kbd> then <kbd>e</kbd>: Go to Events  
<kbd>g</kbd> then <kbd>c</kbd>: Go to Commodities  

<kbd>g</kbd> then <kbd>s</kbd>: Go to Source  
<kbd>g</kbd> then <kbd>o</kbd>: Go to Options  
<kbd>g</kbd> then <kbd>x</kbd>: Go to Statistics  
<kbd>g</kbd> then <kbd>r</kbd>: Go to Errors  

**Filtering:**  
<kbd>f</kbd> then <kbd>t</kbd>: Filter by Time      ( pull down menu)  
<kbd>f</kbd> then <kbd>g</kbd>: Filter by Tag       ( pull down menu)  
<kbd>f</kbd> then <kbd>c</kbd>: Filter by Component ( pull down menu)  
<kbd>f</kbd> then <kbd>p</kbd>: Filter by Payee     ( pull down menu)  

**Options in transaction pages:**  
<kbd>l</kbd>: show/hide legs  
<kbd>s</kbd> then <kbd>l</kbd>: show/hide legs (duplicate shortcut for consistency)  
<kbd>m</kbd>: show/hide metadata  
<kbd>s</kbd> then <kbd>m</kbd>: show/hide metadata (duplicate shortcut for consistency)  
<kbd>s</kbd> then <kbd>o</kbd>: show/hide open  
<kbd>s</kbd> then <kbd>c</kbd>: show/hide close  
<kbd>s</kbd> then <kbd>t</kbd>: show/hide transaction  
<kbd>s</kbd> then <kbd>b</kbd>: show/hide balance  
<kbd>s</kbd> then <kbd>n</kbd>: show/hide note  
<kbd>s</kbd> then <kbd>d</kbd>: show/hide document  
<kbd>s</kbd> then <kbd>p</kbd>: show/hide pad  
<kbd>s</kbd> then <kbd>P</kbd>: show/hide padding  

**Charts:**  
<kbd>Shift</kbd> + <kbd>c</kbd>: show/hide chart  
<kbd>c</kbd>: cycle through all the charts available  

---
**Caution**: Consider this *beta*-software. Contributions are very welcome :-)
