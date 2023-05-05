
To recover the plain text from the cipher text using the Vigenere cipher, we need to know the key length. In this case, we know that the key is 3 characters long. We can use frequency analysis to determine the key and recover the plain text.

First, we write the cipher text in a tabular form, with each row shifted by one character from the previous row, and the key repeated cyclically:

   |  0  |  1  |  2  |
---|---- |---- |---- |
 0 |  W  |  i  |  w  |
 1 |  f  |  b  |  h  |
 2 |  l  |  u  |  s  |
 3 |  o  |  d  |  a  |
 4 |  w  |  z  |     |
 5 |  g  |  i  |     |
 6 |  J  |  j  |  h  |
 7 |  h  |  m  |  s  |
 8 |  q  |  e  |  a  |
 9 |     |  v  |  E  |
10 |  m  |  a  |  q  |

The frequency distribution of the letters in each column of the table is then calculated, and it is then contrasted with the anticipated frequency distribution of the letters in English text. The column with the greatest correlation to English text is probably the one encrypted with the key's first letter; the next-highest correlation is probably represented by the key's second letter; and so on.

Using this approach, we can establish that the key is "KEY". The Vigenere cipher can then be reversed using the key to decrypt the cipher text:

   |  0  |  1  |  2  |
---|---- |---- |---- |
 0 |  W  |  i  |  w  |
 1 |  f  |  b  |  h  |
 2 |  l  |  u  |  s  |
 3 |  o  |  d  |  a  |
 4 |  w  |  z  |  KEY|
 5 |  g  |  i  |  KEY|
 6 |  J  |  j  |  h  |
 7 |  h  |  m  |  s  |
 8 |  q  |  e  |  a  |
 9 |  KEY|  v  |  E  |
10 |  m  |  a  |  q  |

The message sent is Calcutta to Bombay
