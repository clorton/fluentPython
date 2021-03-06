#O

-

A fluent object guy.

"O" (and its sibling "A") provide fluent APIs for building Python objects and arrays.

##Information

-

The syntax is pretty self-explanatory in the code. Look at "O_impl" and "A_impl" for syntax. The only interesting part is how "O" passes function names through to the object. Therefore, you can use _function names_ as property setters. See [examples](#examples) for more details.

###Build

The "build" of "O" is at _TBD_

###Examples

A basic "O" example follows:

```javascript
O
    .refresh(true)
    .voteSort('Count')
    .arguments()
        .round(0)
.$value()
```
yields
```javascript
{ refresh: true, voteSort: 'Count', arguments { round: 0 } }
```

A basic "A" example follows:
```javascript
A
    .$(true)
    .$('Count')
    .$(5)
.$value()
```
yields
```javascript
[ true, 'Count', 5 ]
```
##License

```
The MIT License (MIT)

Copyright (c) 2016 Christopher Lorton

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```