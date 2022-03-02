# ChatBot (the Danish language)

This telegram chatbot is called Danish Booking Chatbot (@airbnb_help_chatbot).  
  The main idea of this chatbot is to search for suitable accommodation options based on the information provided by the user (where the most important are: city name, arrival date and depature date).  
    You can see all files (text corpus and learning models) in my GoogleDrive folder using this url - https://drive.google.com/drive/folders/1tYm7RvAa0bHLo5e1FewjyevO57ef7_W7?usp=sharing.  
      How the algorithm works:  please look into ChatBot.png - it is a chart, where all steps are presented.  
      I used following models: NER (to find entities), LogisticRegression (to classify intent) and LSTM (to generate text). I trained LogisticRegression on BOT_CONFIG (written manually), trained LSTM on MultiWoz, which was previously translated to Danish from English. I also tried to use TRAX model to generate text, but it works very slowly and inaccurate.   
      Chatbot use Booking API to scrape data from site, and it returns top 5 hotels 9with url, score and price).
    

      
