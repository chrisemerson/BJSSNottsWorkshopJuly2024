# Poker Hands Kata

Your program should accept an input of 2 strings representing a poker hand, and should return the name of the person who won the hand, or the string `==TIE==` in the case that the hands are equal. The format of each string is as follows:

`<name>:<card1>,<card2>,<card3>,<card4>,<card5>`

Each card is a rank (`2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `T`, `J`, `Q`, `K`, `A`) followed by a suit (`S`, `H`, `C`, `D`), and the name can be any alphabetical string (`^[A-Za-z]+$`)

Example Input: `myprogram A:4S,3S,5H,6H,2D B:6D,3C,9C,JD,KS`
Example Output: `A`

## Poker Hands

### Royal Flush

Ace, King, Queen, Jack and Ten all in the same suit. Any two royal flushes are equal and result in a tie.

### Straight Flush

5 consecutively ranked cards all in the same suit - eg, `3S`, `4S`, `5S`, `6S`, `7S`. The highest ranked card in the hand breaks ties, or is a tie if both are equal.

### Four Of A Kind

4 cards of the same rank. In the case of 2 players having four of a kind, the higher ranked card involved in the 4 of a kind of wins.

### Full House

3 cards of 1 rank and 2 cards of a different rank. Ties are broken by the rank of the 3 of a kind, then by the rank of the 2 of a kind. If still equal, it's a tie.

### Flush

5 cards all of the same suit, but any rank. Ties are broken by the highest ranked card in each flush, followed by the 2nd highest, etc. If all 5 cards are the same rank in each flush then the hand is a tie.

### Straight

5 consecutively ranked cards of any suit - eg, `7S`, `8H`, `9S`, `TD`, `JH`. Ties are broken by the rank of the highest involved card, or the hand is a tie if both highest cards are equal.

### Three Of A Kind

3 cards with the same rank and any 2 other cards. Ties are broken by the rank there are 3 of, or hand is a tie if equal.

### Two Pair

2 sets of matching rank cards - eg, `4H`, `4S`, `6C`, `8D`, `8S`. Ties are broken by the rank of the higher pair, followed by the rank of the lower pair, followed by the rank of the 5th card in the hand. If all equal then the hand is tie.

### Pair

A pair of matching rank cards. Ties are broken by the rank of the pair, followed by the rank of the highest other card in the hand, then the rank of the 2nd highest other card, then the 3rd. If all equal, hand is a tie.

### High Card

The highest ranked card in the hand wins. In the case of a tie, the 2nd highest ranked card counts, then 3rd etc. If all ranks are equal then the hand is a tie.

