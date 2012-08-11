- [Event](#event)
- [Problem Set](#problem_set)
- [Problem](#problem)
- [Problem Stats](#problem_stats)
- [User-Problem Stats](#user_problem_stats)

<a name="event"/>
## Event

Events are composed of user, action and object.  The user is the subject, the action is the verb and the object is the noun. 

### Time

(*) Server side timestamp. 

### Persist

If true add to the main log and the feeds. (default true)

### Action 

__name__ (*)
Action type.

__adverbs__
Adverbs describe action.

__start_time__
Time when action begins.

__end_time__
Time when action ended.

__context__
Defaults to the url where the action is created.



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


<a name="problem_set"/>
## Problem Set

__problems__(*8)
A set of links to problems. Links can be aliased.

__title__(*)

__tags__

__description__

__grade_prior__
Problem set creator given grade.

__grade__
Our calculated grade.

__render__(*)

  - image
  - color_scheme
  	- primary
  	- secondary

<a name="problem"/>
## Problem

__title__

__image__(*)

__tags__

__template__(*)
Card handlebars template with variables.

__rules__
Template variable rules.

__solution__(*)
Solution defined by variables.

__grade_prior__
Problem creator given grade.

__stats__
Bins K-12. Success count and total count in each bin.

__hint_links__
Links where student can find help.

<a name="problem_stats" />
## Problem Stats

__total_correct__
Total number of correct answers (from all groups)

__total_attempts__
Total number of attempts (from all groups)

__total_time__
Total time spent on this problem (seconds)

__bins[K-12]__
Points split by fraction of progress through school year

- __total_correct__
Total number of correct answers
- __total_attempts__
Total number of attempts
- __total_time__
Total amount of time spent (seconds)

<a name="user_problem_stats" />
## User-Problem Stats

__total_time__
Sum of card durations.

__sucessess__
Number of successes.

__attempts__
Number of attempts.


