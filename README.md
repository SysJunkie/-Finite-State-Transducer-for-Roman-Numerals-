# Finite State Transducer For Roman Numerals

Roman numerals were developed in the 8th century BC, went through several stages of development, and remained in common use into the 14th and 15th centuries. They are still used today in certain contexts such as in book prefaces, introductions and chapters, acts in plays, movements in music, movie sequels, names of monarchs and popes, timepieces, buildings (construction year), Olympic games, Super Bowl, and Wrestlemania events. The standard Roman numerals from 1 to 20 (including subtractive notation for 4 and 9) are as follows: I, II, III, IV, V, VI, VII, VIII, IX, X, XI, XII, XIII, XIV, XV, XVI, XVII, XVIII, XIX, XX.

Used the website at https://www.draw.io/ to draw an FST that simultaneously achieves two things: (1) checks whether the input is a well-formed roman numeral between 1 and 20, and (2) outputs the corresponding Hindu-Arabic numeral.

Implemented the FST in SWI Prolog, so that a query like q0([x,v,i,i],N) yields N = [1,7] and q0(N,[8]) yields N = [v,i,i,i] but any query involving an ill-formed Roman numeral like q0([v,i,v],N) yields ‘false’.
