This is a small project built for learning recommendation system using Machine Learning techniques. 
Team members: Lam Nguyen, Khang Bui, Phan Bui

Pre-process dataset:
 - Download dataset from yelp.ca/dataset
 - Extract the dataset to get 6 json files. We only need file yelp_academic_dataset_user.json and yelp_academic_dataset_review.json so we can delete other files.
 - Run these following commands:
	+ pip install --user simplejson sqlalchemy
	+ python json_to_csv_converter.py yelp_academic_dataset_user.json
	+ python json_to_csv_converter.py yelp_academic_dataset_review.json
	+ python make_review_DB.py
	+ python make_user_DB.py
	+ python update_review_DB.py
	+ python update_user_DB.py
	+ python make_table.py
	+ python query_v2.py
- Now we have a file named review.csv. In this file, there are totally 1500 unique users, 3000 unique businesses and 100000 reviews. 