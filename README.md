# email-spam-classifier-new
End to end code for the email spam classifier project

## Following are the steps to deploy this project on Render

1. Update requirements.txt with the following code:
    
    ```python
    nltk==3.7
    streamlit==1.10.0
    streamlit_lottie==0.0.3
    scikit-learn
    ```
    
2. Add the following lines in [app.py](https://github.com/campusx-official/sms-spam-classifier/blob/main/app.py) file, below all the imports:
    
    ```python
    nltk.download('punkt')
    nltk.download('stopwords')
    ```
    
3. Push the updated code to Github.
4. Go to [render.com](http://render.com) and then click on new and then click on web service.
5. Select the Github repo from the list.
6. Give the name of your choice to the website.
7. Update the Build command to:
    
    ```python
    pip install -r requirements.txt
    ```
    
8. Update the start command to:
    
    ```python
    streamlit run app.py
    ```
    
9. Click on Deploy.
10. Your deployment is complete.
