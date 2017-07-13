# Common JS Pitfalls

> Note: A lot of these can be avoided by using JavaScript Strict Mode

* Global Variables
  * Really easy to make accidentally
  * Mess up scope
* Scope
  * When using `var`, variables are not scoped to a block (`{}`).
  * This is not the case with `let` or `const`
* Semicolons
  * Sometimes semicolons are required to end an expression. 
  * Best practice - just put them in everywhere.

```
;;;;;;;;;;;;;;a = 1+1;
;;;;;;;;;;;;;;;;;; console.log(a);
```
* Reserved Words - Don't use them outside of context

```
abstract boolean break byte case catch char class const continue
 debugger default delete do double else enum export extends false final
 finally float for
 function goto if implements import in instanceof int interface long native new null
 package private protected public return short static super switch synchronized this
 throw throws transient true try typeof var volatile void while with
```

* Unicode
  * One must be careful - unicode requires two bites for one character
* `typeof`
  * Since everything is an object™, it can be unreliable (eg. `typeof [] === 'object'`)
* Floating Point
  * 0.1 + 0.2 !== 0.3 🤷‍
  * Scale it up, perform the math, scale it down
* Falsy Values
  * 0, NaN, '', false, null, undefined