# Word Cloud
This repo contains python code to create a word cloud from a .csv file that contains a columns of words and a column of desired word frequencies. The follwoing are the default parameters:
WordCloud(
    font_path=None,
    width=400,
    height=200,
    margin=2,
    ranks_only=None,
    prefer_horizontal=0.9,
    mask=None,
    scale=1,
    color_func=None,
    max_words=200,
    min_font_size=4,
    stopwords=None,
    random_state=None,
    background_color='black',
    max_font_size=None,
    font_step=1,
    mode='RGB',
    relative_scaling='auto',
    regexp=None,
    collocations=True,
    colormap=None,
    normalize_plurals=True,
    contour_width=0,
 
 - width/height: You can change the word cloud dimension to your preferred width and height with these.  
- random_state: If you don’t this set this to a number of your choice, you are likely to get a slightly different word cloud every time you run the same script on the same input data. By setting this parameter, you ensure reproducibility of the exact same word cloud. You could play around with random numbers until you find the one that results in the word cloud you like.  
- background_colour: ‘white’ and ‘black’ are common background colours. If you would like to explore more colours, this may come in handy. Please note that some colours may not work. Hope you will find something you fancy.  
- colormap: With this argument, you can set up the colour theme that the words are displayed in. There are many beautiful Matplotlib colormaps to choose from. Some of my favourites are ‘rainbow’, ‘seismic’, ‘Pastel1’ and Pastel2’.  
- collocations: Set this to False to ensure that the word cloud doesn’t appear as if it contains any duplicate words. Otherwise, you may see ‘web’, ‘scraping’ and ‘web scraping’ as a collocation in the word cloud, giving an impression that words have been duplicated.  
- stopwords: Stopwords are common words which provide little to no value to the meaning of the text. ‘We’, ‘are’ and ‘the’ are examples of stopwords. I have explained stopwords in more detail here (scroll to ‘STEP3. REMOVE STOPWORDS’ section). Here, we used STOPWORDS from the wordcloud package. To see the set of stopwords, use print(STOPWORDS) and to add custom stopwords to this set, use this template STOPWORDS.update(['word1', 'word2']), replacing word1 and word2 with your custom stopwords before generating a word cloud.  
