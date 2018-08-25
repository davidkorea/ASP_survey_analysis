# ASP_survey_analysis

# Summary
1. 
```python
sentence_list = data_df['col_1'].tolist()
```

2. 
```python
cut_list = []
for sentence in sentence_list():
cut_word = jieba.lcut(sentence):
for word in cut_word:
    cut_list.append(word)
longtext = ' '.join(cut_list)
```

3. 
```python
tfidf_word = jieba.analyse.extract_tags(long_text, topK=20, withWeight=False, allowPOS=('n')) #get only noun```

4. 
```python
text = nltk.text.Text(tfidf_word)
```

5. 
```python
fd = nltk.FreqDiste(text)
```

6. 
```python
fd.most_common(10)
```

7. 
```python
使用 jieba.analyse.extract_tags得到的词list是根据词频排序后的去重单词，以次画出词云，排在list前面的单词显示大。
即由于词频高（tfidf高）排在了列表前面，词云自动认为排在前面的单词重要性高，因此显示字体大
```
