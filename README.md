# Wildlife Tracker 

## Story 1 Branch: animal-crud-actions
-commands used: 
    $rails new rails-api -d postgresql -T
    $cd rails-api 
    $rails db:create
    ##git commands to connect rails app to github repo
    ##initial commit
    $bundle add rspec-rails
    $rails generate rspec:install
    $rails s ##(test if sever is working)
    $rails generate resource Animal name:string binomial:string
    $rails db:migrate
    $rails routes ##(keep routes on this terminal window)
    ##CMD + t (new terminal window)
    $rails s
    ##CMD + t (new terminal window)
    $rails c ##(create instances)
    $Animal.create(name:'Cat' , binomial:'Felis catus')
    $Animal.all 
    ##CMD + t (new terminal window)
    ##this new terminal will be my git terminal
- Steps
    - index: succesfully called all 5 instances on postman
    - create: created Werewolf instance
    - update: updated scientific binomial for Werewolf instance
    - destroy: destroyed an extra Werewolf instance that was accidentally created in update section.


## story 2 Branch: sighting-crud-actions
- commands used: 
    $rails g resource Sighting animal_id:integer latitude:float longitude:float date:date
    $rails db:migrate
    ##toggle over to terminal window with "rails c" running
    ##having trouble creating instance, exited and reentered ruby environment and successfully created instance.
    $Sighting.create(animal_id: 1, latitude: 44.94172, longitude: -123.71163, date: '2023-11-30')
- Steps
    - index: successfully called 5 instances on postman
    - create: created 2 new sighting instances for Werewof
    - update: Updated the date on id#7 Werewolf sighting instance
    - destroy: destroyed id#6 Werewolf sighting instance