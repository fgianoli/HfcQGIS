Corrispondenza fuzzy
===================================

Questo gruppo contiene le funzioni per comparazioni fuzzy fra i valori.

+---------------------------------+------------------------------------+
| Funzione                        | Descrizione                        |
+=================================+====================================+
| `hamming_distance`_             | Restituisce la distanza di Hamming |
|                                 | tra due stringhe. Questa equivale  |
|                                 | al numero di caratteri nelle       |
|                                 | corrispondenti posizioni delle     |
|                                 | stringhe in ingresso dove i        |
|                                 | caratteri sono diversi. Le         |
|                                 | stringhe in ingresso devono avere  |
|                                 | la stessa lunghezza, e il          |
|                                 | confronto è sensibile alle lettere |
|                                 | maiuscole                          |
+---------------------------------+------------------------------------+
| `levenshtein`_                  | Restituisce la distanza di         |
|                                 | Levenshtein tra due stringhe.      |
|                                 | Questa equivale al minimo numero   |
|                                 | di modifiche di caratterere        |
|                                 | (inserimenti, cancellazioni o      |
|                                 | sostituzione) richieste per        |
|                                 | cambiare una stringa in un'altra.  |
|                                 | La distanza di Levenshtein è una   |
|                                 | misura della somiglianza tra due   |
|                                 | stringhe. Distanze più piccole     |
|                                 | corrispondono a stringhe più       |
|                                 | simili, e distanze più grandi      |
|                                 | corrispondono a stringhe più       |
|                                 | differenti. La distanza è          |
|                                 | sensibile alle lettere maiuscole   |
+---------------------------------+------------------------------------+
| `longest_common_substring`_     | Restituisce la sottostringa in     |
|                                 | comune più lunga tra due stringhe. |
|                                 | Questa sottostringa è la stringa   |
|                                 | più lunga che è una sottostringa   |
|                                 | delle due stringhe in ingresso.    |
|                                 | Es: la sottostringa in comune più  |
|                                 | lunga di "ABABC" e "BABCA" è       |
|                                 | "ABC". La sottostringa è sensibile |
|                                 | alle lettere maiuscole             |
+---------------------------------+------------------------------------+
| `soundex`_                      | Restituisce la rappresentazione    |
|                                 | Soundex di una stringa. Soundex è  |
|                                 | un algoritmo di abbinamento        |
|                                 | fonetico, per cui le stringhe con  |
|                                 | suoni simili dovrebbero essere     |
|                                 | rappresentate dallo stesso codice  |
|                                 | Soundex                            |
+---------------------------------+------------------------------------+

|image0|

.. _hamming_distance: hamming_distance.html
.. _levenshtein: levenshtein.html
.. _longest_common_substring: longest_common_substring.html
.. _soundex: soundex.html

.. |image0| image:: /img/corrispondenza_fuzzy/gruppo_corrispondenza_fuzzy1.png


**Elenco funzioni Corrispondenza fuzzy**

.. toctree::
   :maxdepth: 3

   hamming_distance
   levenshtein
   longest_common_substring
   soundex
   
