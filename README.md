# Introduction 
YouTube is the most popular and most used video platfrom in the world today. YouTube has a [list of trending videos](https://www.youtube.com/feed/trending) that is updated constantly. Here I have used Python with some packages like Pandas, Matplotlib, Plotly and Seaborn to analyze a dataset that was collected over 205 days. For each of those days, the dataset contains data about the trending videos of that day. It contains data about more than 90,000 trending videos. This data has been analyzed to get insights into YouTube trending videos, to see what is common between these videos. Those insights might also be used by people who want to increase popularity of their videos on YouTube.

The dataset can also be obtained from Kaggle [here](https://www.kaggle.com/datasnaek/youtube-new). It contains data about trending videos for many countries.

# Goals of the analysis
#### We want to answer questions like:

1) What are the various positive and negative words used in the comments?
2) Which are the most popular emojis used in the comment section?
3) Which video category (e.g. Entertainment, Gaming, Comedy, etc.) has the largest number of trending videos?
4) How does the audience engagment vary for different categories?
5) How are view, likes, and dislikes correlate with (relate to) each other?
6) Does Punctuations on video title have impact on the views, likes, and dislikes.
7) How long usually a video can trend in different countries?
8) Videos from which category has longer trend?
9) What are the Most common words(Trending words) in video title?
10) Which category has highest ratio of Likes-Dislikes and Views-Comments?

# Data Storage
To store big data, I have used two methods here:
1) AWS S3 Bucket
2) Git LFS

### AWS S3 Bucket
AWS free tier account gives storage upto 5GB for Standard Storage. Follow the documentation [here](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html) to create a S3 bucket. This bucket can used to store multiple types of files. Here we have used only csv and json files for the project. 

Boto3 package was used this project to intialize the S3 bucket and use the contents stored to read, write, upload, and download. (Refer concatenated_files.ipynb to see the various methods to store a file in different formats) 

[Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) is the Amazon Web Services (AWS) Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of services like Amazon S3 and Amazon EC2. 

It is maintained and published by [Amazon Web Services](https://aws.amazon.com/what-is-aws/).

### Git LFS
GitHub only allows uplto 50MB of data to be stored. For storing files of large size, GIT LFS can be used. 

Git Large File Storage (LFS) replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise. It provides upto 1GB of free storage. 

It offers features like Large file versioning, More repository space, Faster cloning and fetching, Same Git workflow, and Same access controls and permissions.
Git LFS is intilized once per user. Follow this [documentation](https://git-lfs.com/) to download and install Git LFS.  


  
