# Closure Issue in setTimeout Loop

This repository demonstrates a common closure-related issue in JavaScript when using `setTimeout` within a loop. The problem arises because the closure created by `setTimeout` doesn't capture the value of `i` at the time of its creation, but rather captures a reference to the variable `i`. By the time the `setTimeout` callbacks finally execute, the loop has already completed, and `i` has its final value (10). 

The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides the corrected code. This is a frequent source of confusion for developers new to JavaScript closures.