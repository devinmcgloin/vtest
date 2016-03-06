# Visial Testing
vtest is a visual testing framework. It also doesn't exist yet.

## Simple Example
Here we're looking at the python function `startswith`. Yes, this is incredibly simplistic. 1 represents truth and 0 falsity. We're testing the function on all possible 3 length strings, in order to see how it behaves. The particular function here is `s.startswith("g") or s.startswith("&")`, we can see here that it returns true from `&!!` to `&~~` and  `g!!` to `g~~`. Great thats exactly what we wanted.

![Simple Demo](https://raw.githubusercontent.com/devinmcgloin/vtest/master/img/simple.png)

This obviously works for math as well. Here's `x^3/3`

![Math Demo](https://raw.githubusercontent.com/devinmcgloin/vtest/master/img/math.png)

## Open Questions

- Visualizing items requires an order, if you're testing functions like `s.startswith("g") or s.endswith("&")` this doesn't work as break points would have to be found in two different orders.
- Right now finding breakpoints is done by generating all possible combinations, and calling the function on every single one. This obviously won't scale in its current form.
- How do you sort and find break points in composite data types?
