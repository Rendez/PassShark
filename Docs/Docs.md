Class: PassShark {#PassShark}
=============================



### Implements:

Options, Events, Log, Class.Occlude




PassShark Method: constructor {#PassShark:constructor}
-------------------------------------------------------


### Syntax:

	var myPassShark = new PassShark(element, options);

### Arguments:

1. element - (**)
2. options - (**)

### Options:

* interval - (**)
* duration - (**)
* replacement - (**)
* prefix - (**)
* debug - (**)

### Returns:





PassShark Method: _setup {#PassShark:_setup}
---------------------------------------------


### Syntax:




PassShark Method: _cloakInput {#PassShark:_cloakInput}
-------------------------------------------------------


### Syntax:



### Arguments:

1. params - (**)


PassShark Method: start {#PassShark:start}
-------------------------------------------


### Syntax:



### Arguments:

1. event - (**)


PassShark Method: stop {#PassShark:stop}
-----------------------------------------


### Syntax:



### Arguments:

1. event - (**)


PassShark Method: _onDeletion {#PassShark:_onDeletion}
-------------------------------------------------------


### Syntax:



### Arguments:

1. caret - (**)
2. diff - (**)


PassShark Method: _setPassword {#PassShark:_setPassword}
---------------------------------------------------------


### Syntax:



### Arguments:

1. str - (**)


PassShark Method: _convertLastChar {#PassShark:_convertLastChar}
-----------------------------------------------------------------


### Syntax:




PassShark Method: _check {#PassShark:_check}
---------------------------------------------


### Syntax:



### Arguments:

1. oldValue - (**)
2. initialCall - (**)
3. posCaret - (**)


PassShark Method: _correctCaret {#PassShark:_correctCaret}
-----------------------------------------------------------


### Syntax:



### Arguments:

1. caret - (**)

### Returns:





PassShark Method: _getCaretRange {#PassShark:_getCaretRange}
-------------------------------------------------------------


### Syntax:



### Returns:




