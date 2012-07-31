## Event

Events are composed of user, action and object.  The user is the subject, the action is the verb and the object is the noun. 

### Time

(*) Server side timestamp. 

### Action 

__name__ (*)
Action type.

__adverbs__
Adverbs describe action.

__start_time__
Time when action begins.

__end_time__
Time when action ended.



### Object

__type__ (*)
Object type.

__title__
Title.

__url__
Url to object.

__tags__
Meta data.



### Action Types

Action types are registered via registerAction in root app.

__name__ (*)
Action type. 

__image__
Image for action.

__template__ 
Handlebars template for rendering event in feed.

__adverbs__ (validator)
List of allowed adverbs.

__objects__ (validator)
List of objects action can act on.



## Problem Set

__problems__
A set of links to problems. Links can be aliased.

__title__

__tags__

__description__

__render__

  *image

  *color_scheme

  	*primary_color

  	*secondary_color


## Problem




