# monster_cat
An educational tool to record participant feedback during workshops


WorkshopsController:
before any action, there has to be a user signed up

index method shows all the workshops on the page

show method lets you search workshops by ID using params

The workshop class has a one to many relationship with the feedback class.
Workshop needs to be initialised with name, desc, and url with validations.
dependent:destroy - when workshop is deleted from database removes feedback entries corresponding to the workshop id.

Feedback resource nested in Workshop resource - handles routing and relationship and communication between feedback and workshop.

NESTED RESOURCE EXPLANATION?
