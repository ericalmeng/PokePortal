# Q0: Why is this error being thrown?
The server is looking for controller name Pokemon, which is not been make yet.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
The pokemon are appearing randomly as "A wild <pokemon> appeared". The common factor is that all these pokemons are generated in the seed file that is provided.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
First, it create a button called "throw a Pokeball". Next, capture_path specifies the path that will be directed. So that, it takes id as parameter that is a request that we need to update the database accordingly. :class is html_options that specifies the class of the button for css styling. :method specifies the mothod since we are doing a update here so we use PATCH here.

# Question 3: What would you name your own Pokemon?
Futata

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed in the trainer_path with current trainer as parameter. This is because ruby automatically grabs the default formatting for the url and then simply applues the id url to it. 

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
This line shows a notification at the top of the non-template view that tells the user that the pokemon name has already been taken.

# Give us feedback on the project and decal below!

# Extra credit: Link your Heroku deployed app
