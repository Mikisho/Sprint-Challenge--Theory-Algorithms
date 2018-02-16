### Answers
  --------------------------------------------
  ********************************************
1. Single regex that matches either of:
antelope rocks out
antelopes rock out

`Regex: /antelopes?/g`

2. Regex that matches either of:
  goat
  moat
  but not:
  boat

  `Regex: /([gm]oat/g)`

3. Regex that matches dates in YYYY-MM-DD format. (Year can be 1-4 digits, and
  month and day can each be 1-2 digits). This does not need to verify the date
  is correct (e.g 33333-33-33 can match).

  2000-10-12
  1999-1-20
  1999-01-20
  812-2-10

 `Regex: /\d{1,4}-(1[0-2]|0[1-9]|[1-9])-((0[0-9]|[1-2][0-9]|3[01]|[1-9])([\s\r\n]|$))/g`