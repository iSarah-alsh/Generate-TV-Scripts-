# Generate-TV-Scripts-
June 28, 2019
# 1- TV Script Generation:
In this project, you’ll generate your own Seinfeld TV scripts using RNNs. You’ll be using part of the Seinfeld dataset of scripts from 9 seasons. The Neural Network you’ll build will generate a new ,"fake" TV script, based on patterns it recognizes in this training data.
# 1.1 Get the Data:
The data is already provided for you in ./data/Seinfeld_Scripts.txt and you’re encouraged to open that file and look at the text. >* As a first step, we’ll load in this data and look at some samples. * Then, you’ll be tasked with defining and training an RNN to generate a new script!
In [1]: """
        DON'T MODIFY ANYTHING IN THIS CELL
        """
        # load in data
        import helper
        data_dir = './data/Seinfeld_Scripts.txt'
        text = helper.load_data(data_dir)
 # 1.2 Explore the Data:
 Play around with view_line_range to view different parts of the data. This will give you a sense of the data you’ll be working with. You can see, for example, that it is all lowercase text, and each new line of dialogue is separated by a newline character.
 In [2]: view_line_range = (0, 10)
        """
        DON'T MODIFY ANYTHING IN THIS CELL THAT IS BELOW THIS LINE
        """
        import numpy as np
        print('Dataset Stats')
        print('Roughly the number of unique words: {}'.format(len({word: None for word in text.s
        lines = text.split('\n')
        print('Number of lines: {}'.format(len(lines)))
        word_count_line = [len(line.split()) for line in lines]
        print('Average number of words in each line: {}'.format(np.average(word_count_line)))
        print()
        print('The lines {} to {}:'.format(*view_line_range))
        print('\n'.join(text.split('\n')[view_line_range[0]:view_line_range[1]]))
