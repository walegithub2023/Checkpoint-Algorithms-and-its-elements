# NAME OF REPOSITORY: Checkpoint-Algorithms-and-its-elements



# DESCRIPTION: A repository for Checkpoint Algorithms and its elements@ gomycode. This repo houses an algorithm which is described below.



# ALGORITHM NAME: read_a_sentence



# An Algorithm to read a sentence, which ends with a point, character by character, and to determine:

  - The length of the sentence (the number of characters).
  - The number of words in the sentence (assuming that the words are separated by a single space).
  - The number of vowels in the sentence.



# Below is a discription of what the alorithm is doing(algorithm steps to solve the problem):

  - Naming the algorithm.

                ALGORITHM PART:.....ALGORITHM read_a_sentence

  
  - Declaration and intialization of the 3 main variables to be used as counters.

		ALGORITHM PART:.....countChar, countWord, countVowel: INTEGER:=0;.......

  
  - Declaration and intialization of other variables.

		ALGORITHM PART:.... sentence: STRING;
    		                    sentenceIndex: INTEGER := 0;
    		                    character: STRING;
    		                    countSpace : INTEGER := 0; 
  
  - Algorithm Begins. Get input of sentence.
		
		ALGORITHM PART:.....BEGIN
				    Read(sentence);


  - Use a while do loop.

		ALGORITHM PART:.....WHILE (sentence NOT '.') DO


  				    - Check if character is a space then count the spaces with the loop.

			                     ALGORITHM PART:......IF (character = " ") THEN
            	                                                  countSpace = countSpace + 1;
        	                                                  END_IF


  		                    - Check if character is a vowel then count.

			                     ALGORITHM PART:......IF (character = 'a' or character = 'e' or character = 'i' or character = 'o' or character = 'u') THEN
            			                                  countVowel = countVowel + 1;
        			                                  END_IF

  		                    - End while loop.

		                             ALGORITHM PART:......END_WHILE



  - Add one to the space to get the number of words.

                ALGORITHM PART:.....countWord = countSpace + 1;

		  
  - Add the point to the number of characters.

                ALGORITHM PART:.....countChar = countChar + 1;

                
  - Print number of characters, words and vowels.

                ALGORITHM PART:.....Write("The number of characters in the sentence is: "+countChar);
                                    Write("The number of words in the sentence is: "+countWord);
                                    Write("The number of vowels in the sentence is: "+countVowel);

  - Algorithm ends.

		ALGORITHM PART:.....END






