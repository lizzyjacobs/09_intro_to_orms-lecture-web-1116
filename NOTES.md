# CRUD REVIEW

## Create
- INSERT INTO tweets (username, message) VALUES ()
- save
- tweet = Tweet.new({message: 'Great coffee', username: 'coffeedad'})
- tweet.save
- Tweet.create({message: 'I am so lonely', username: 'coffeedad'})

- What's a good name for a ruby method that would fire that action?
## Read
- all
- SELECT * FROM tweets
- find(id)
- Tweet.find(5)
- SELECT * FROM tweets WHERE id = 5 LIMIT 1;
- Tweet.where({username: 'coffeedad'})
- an array of all of the tweets where the username is 'coffeedad'

- Tweet.find_by(message: 'great # coffee')
- one instance of the tweet class where the message is 'great # coffee'

## Update
- UPDATE tweets SET (message, username) VALUES ('great coffee', "coffeedad") WHERE id = 3
- tweet.update({message: 'A new message'})
## Delete
- DELETE FROM tweets WHERE id = 9
- tweet.destroy
