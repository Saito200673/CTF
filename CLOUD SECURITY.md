

Since they announced that there was an cloud section in the CTF I knew that it would be in AWS( Amazon Web Services ) but just wasn’t sure what it’s about 

And I had an guess it would be in S3 buckets and as you guys guessed it was about it 

#### **Unlike other challenges you need some stuff first to get started as they mentioned in the challenge :** 

1.S3 browser- 

2.AWS CLI - basically an terminal but just for AWS services and you just install it in the terminal 
And to the windows guys you can do the same in the cmd 

3.An AWS account which just make this all work easier but I don’t think most people have it 
But it’s an option 

And any one of these is enough not sure about the S3 browser tho since I didn’t use it 
I personally used AWS cli for this if you have a bit of experience in the terminal then it’ll be easy 
But for people with windows it might look hard at first but since the commands are less you can learn it just fine 

## **Misconfigured Bucket**

By the title I came to know that the bucket is configured wrong basically it is made public and can be accessed without even an account And  another reason is that they didn’t give any other info on the bucket so that must be only possibility 
AWS is for activating the AWS cli and s3 is for the type of service you’re accessing from the AWS CLI


So started this challenge by copying the bucket name which is and fired up the terminal 
And entered this command which basically finds the bucket and lists its contents on the screen 

and the **—no-sign-request** this is used cause normally this command usually gives the credentials on its own and when you haven’t entered any credentials it throws an error message 
And for an public bucket you don’t need an credentials so we use this to not send any credentials on our own 


Now you can see that there is indeed an file in the bucket
Now let’s copy it to an file in our system the same code but you just change the ls to cp 
###### Here **ls** is for listing the contents of an file
**cp is for copying an given file to another file**

And another change which you would have to do is that add an whack **”/“**
And copy paste the file name to the command after the whack and have to name a file where you want to save this file we took from the bucket 
Then you can use the cat <> or just use the file manager to access the file and you get the flag and submit it 
 
## **S3crets**

As for this I’m not sure if this is the expected way to do the challenge but I got the flag so not really my problem  I think the link it was there just to throw people off since the url wasn’t really necessary 

I just followed the same process which I used for the Misconfigured bucket and got the secrets.txt file did cat on it 
And got the flag and just like any flag submitted it on the website 










