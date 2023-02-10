# NLP
This project helps a person memorize WORD DEFINITIONS faster using three steps:
  1. User is asked to input a list of words with their given definitions in .csv format.
  2. The program starts to check if a user has memorized words by asking for input for each given word
     -  Input could be given using Writing or Speech
     - If Speech is used, the program asks the User to record the definition of the word using audio for 10-15 seconds which is transcribed using DeepSpeech library & converted to text input.
     - If Wriitng is used, the program asks the User to write (using Keyboard) the definition of the word which is used as the text input.
    
  3. BERT (bert-base-nli-mean-tokens) model from Sentence-Transformers library checks if the text input vector embeddings match the definition vector embeddings using Cosine Similiarity, and if it reaches a certain threshold, makes the conclusion that word has been memorized, and moves on to the next word in the list. At the end of the program, it prints out all the words NOT MEMORIZED in the same format, that could be used again once user comes back after memorizing those words. 

