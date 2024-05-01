# Question3
The Diving Bell and the Butterfly by Jean-Domininque Bauby was originally written in French. The first sentence of the book is translated to English below.
through the frayed curtain at my window a warm glow announces the break of day

Estimate how many yes/no questions need to be asked to type out this sentence.
Punctuation and capitalization have been removed. These were added by an editor later.
Think about how your program works and try to estimate the number of questions needed. You should be able to predict the answer without typing out the sentence yourself. You do not need to get the exact answer, but you should not be drastically off.

Write a short reflection on how both your programs worked. Answer the following:
alphabet = " !.abcdefghijklmnopqrstuvwxyz"
29 characters 

1. About how many questions do you estimate are needed to type the sentence using linear search?
  => If I were to use linear search and go character by character, I would on average 15 questions per letter in case the character is in the middle of the alphabet. It would be 29 questions in the worst-case scenario if the characters were at the end. 
We have 71 letters in the sentences and 14 (each space between words).
Average case: 15 * (71+14) = 1275 questions
Worst case: 29 * (71+14) = 2465 questions

2. About how many questions do you estimate are to type the sentence using binary search?
   => In binary search, I divide the search space in half until I find the target. 
   Given the alphabet of length 29, I would need around 5 questions per letter
   Level of binary: log2(N) => log2(29) = 5
   => Average and Worse Case :  (71+14) * 5 = 425
  
3. If you were Jean-Domininque, which program would you rather use?
   => If I were Jean-Dominique, I would choose the Binary Search approach as it drastically reduces the number of questions to determine the characters in the sentence.
      
4. What was the easiest part of implementing this assignment?
   => The linear search algorithm is the easiest part of implementing this assignment because it is more straightforward to understand and implement as it sequentially checks each element with a fixed list.
   
5. What was the most challenging part of implementing this assignment?
   => Although the binary search algorithm significantly improves efficiency, it is more complex to implement.
    This algorithm requires understanding recursion or loop and the logic of halving the search space at each step. Its correctness is crucial, minor mistakes can lead to incorrect results or infinite loops.
