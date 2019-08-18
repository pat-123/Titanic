This is a classification problem, to predict if a passenger survived the Titanic or not

Few points worth mentioning regarding directory structure:
--csv is placed under data/raw/
--Processed csv is places under data/processed after computation
--Test predictions are available under data/submitted
--Notebook is present in notebooks folder
--Titanic is a package which load all initial packages(__init__.py) and sets data file paths under config.py
  ++ Abstracts the messy paths in the main notebook to here, so that cleaner view can be provided
--scripts folder is a placeholder for future purposes
--How to run this?
  ++ start Anaconda prompt and go to this folder's parent locationr and type jupyter notebook
  ++ notebook starts with the parent folder as the base location and you can navigate to different projects from there

--Used train_test_splits 

---------------------------------------------------
New additions
--------------------------------------------------
++Use KFolds instead of train_test_splits 
++write a OOPS style framework for running different ML regressor algo on the cleaned data and compare performance and choose the best ML model suited for this model

-------------------------------------------------- 
RESULT
--------------------------------------------------
I have used RandomForest and SVM and SVM performs better with average model score of 82 % run over 5 KFolds
