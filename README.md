# Python-Word-Game
 Python Word Game

Allow the user to play a series of hands

    * Asks the user to input a total number of hands

    * Accumulates the score for each hand into a total score for the 
      entire series
 
    * Each hand given will include a wildcard letter '*'
      which can replace any vowel, but player does not receive any points 
      for using the wildcard (unlike all other letters), though it does
      count as a used or unused letter when scoring.

    * For each hand, before playing, ask the user if they want to substitute
      one letter for another. If the user inputs 'yes', prompt them for their
      desired letter. This can only be done once during the game. Once the
      substitue option is used, the user should not be asked if they want to
      substitute letters in the future.

    * For each hand, ask the user if they would like to replay the hand.
      If the user inputs 'yes', they will replay the hand and keep 
      the better of the two scores for that hand.  This can only be done once 
      during the game. Once the replay option is used, the user should not
      be asked if they want to replay future hands. Replaying the hand does
      not count as one of the total number of hands the user initially
      wanted to play.

            * Note: if you replay a hand, you do not get the option to substitute
                    a letter - you must play whatever hand you just had.
      
    * Returns the total score for the series of hands

    * The score for a word is the **product** of two components:
        - First component: the sum of the points for lettters in the word.
        - Second component: either [7 * ​word_length - 3 * (​n-​word_length)] or 1,
          whichever value is greater, where:
            ▪ word_length is the number of letters used in the word
            ▪ n is the number of letters available in the current hand
    
    * Points for letters:
        '*': 0, 'a': 1, 'b': 3, 'c': 3, 
        'd': 2, 'e': 1, 'f': 4, 'g': 2, 
        'h': 4, 'i': 1, 'j': 8, 'k': 5, 
        'l': 1, 'm': 3, 'n': 1, 'o': 1, 
        'p': 3, 'q': 10, 'r': 1, 's': 1, 
        't': 1, 'u': 1, 'v': 4, 'w': 4, 
        'x': 8, 'y': 4, 'z': 10