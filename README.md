# deterministic-finite-automaton
1. Какова вычислительная сложность поиска подстроки длиной m в строке длиной n с использованием конечного детерминированного автомата?
  О(n)
2. Постройте конечный детерминированный автомат для поиска подстроки «колокол» в строке «колокольчик и колокол». Проиллюстрируйте по шагам работу алгоритма.
   1) Определение алфавита строки t:
      к л о
   2) Создание таблицы перпеходов:
      к л о
      1 0 0
      1 2 0
      1 0 3
      1 4 0
      5 0 0
      1 6 0
      1 0 7
      1 4 0
   3) Поиск:
    позиция   прочитал   перешел
       0      s[0]="к"      1
       0      s[0]="о"      2
       0      s[0]="л"      3
       0      s[0]="о"      4
       0      s[0]="к"      5
       0      s[0]="о"      6
       0      s[0]="л"      7
       0      s[0]="ь"      0
       0      s[0]="ч"      0
       0      s[0]="и"      0
       0      s[0]="к"      1
       0      s[0]=" "      0
       0      s[0]="и"      0
       0      s[0]=" "      0
       0      s[0]="к"      1
       0      s[0]="о"      2
       0      s[0]="л"      3
       0      s[0]="о"      4
       0      s[0]="к"      5
       0      s[0]="о"      6
       0      s[0]="л"      7
   4) Позиции: 0, 10