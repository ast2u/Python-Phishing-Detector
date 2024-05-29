# Python-Phishing-Detector
A Python Project that detects if the url that you inputted is a phishing site.

It uses algorithm and Machine Learning to know if the website is a phishing site.
The algorithm use is:
- MultinomialNB
- LogisticRegression

It also shows testing results in graphs and numbers.
- CountVectorizer

# How to run the Detector?
Firstly you will be downloading the files in this repository. The files are in main and in another branch called Environment.
The files inside the Environment is an environment created in VS Code in which it has the downloaded addons, apis, and imports
needed for the project to run. You can run the code the test detector without the files in the Environment, you can download
all the imports by yourself in your computer or on your created environment.

Once you have downloaded the files, you must run it with [VS Code](https://code.visualstudio.com/) or [Google Colab](https://colab.google/)
In the initial run that we did for this project is in VS Code so the steps will be applicable for VS Code.
1. To run the detector, open the folder that has these files
2. Create an environment to download necessary imports for the project OR download the necessary imports directly to your computer
3. Open the file phishsite url.ipynb
4. Run all the command starting from the top to the bottom
5. The last code in the file phishsite url.ipynb, you can edit the url so you can test out other sites
'predict_bad = ['marketplace.axieinfinity.com/']
predict_good = ['www.phishprotection.com/content/phishing-prevention/']
loaded_model = pickle.load(open('phishing.pkl', 'rb'))
#predict_bad = vectorizers.transform(predict_bad)
# predict_good = vectorizer.transform(predict_good)
result = loaded_model.predict(predict_bad)
result2 = loaded_model.predict(predict_good)
print('The 1st website is: ',result)
print()
print("="*50)
print()
print('The 2nd website is: ',result2)'
