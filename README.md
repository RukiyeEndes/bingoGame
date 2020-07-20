# bingoGame

Bingo is a game where players are given a 5x5 dimension board filled with numbers and free space in the middle. Numbers are called until the board achieves a continuous set of five called numbers either vertically, horizontally, or diagonally. The free space counts as one match in every case.
    Your task is to create the bingo game and associated utilities with the end goal being a game runner class which can take any number of boards, which it will randomly generate, and will then call numbers at an interval until one of those boards meets the win condition. At which point it returns the board and stops calling numbers
    Requirements:
        - Create randomized 5x5 boards where there is one free space in the middle and the remaining spaces are filled with non duplicated numbers from 1-75
        - Call numbers which are used to check for a winner, duplicate numbers must not be called, for instance the number 2 cannot be called twice
            - check board with those numbers to assess if it meets the win condition
        - Manager function which takes a number of players (boards) and creates that many boards. Once the boards are created it will call numbers until one is declared a winner and return that board as an object containing a winner property which contains the winning board ex: { winner: <board> }.
